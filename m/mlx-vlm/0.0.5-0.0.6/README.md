# Comparing `tmp/mlx_vlm-0.0.5.tar.gz` & `tmp/mlx_vlm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_vlm-0.0.5.tar", last modified: Tue May  7 08:42:06 2024, max compression
+gzip compressed data, was "mlx_vlm-0.0.6.tar", last modified: Fri May 24 15:59:32 2024, max compression
```

## Comparing `mlx_vlm-0.0.5.tar` & `mlx_vlm-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.835632 mlx_vlm-0.0.5/mlx_vlm/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/chat_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.835632 mlx_vlm-0.0.5/mlx_vlm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.835632 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/idefics2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/idefics2/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/mlx_vlm/models/llava/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/llava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/llava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/llava/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/llava/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/nanoLlava.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/vision.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/prompt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/sample_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/mlx_vlm/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/tokenizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26042 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/mlx_vlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/mlx_vlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 08:42:06.000000 mlx_vlm-0.0.5/mlx_vlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:42:06.839632 mlx_vlm-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 08:42:01.000000 mlx_vlm-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/chat_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/idefics2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/models/llava/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/llava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/llava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/llava/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/llava/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/nanoLlava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/paligemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/prompt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/sample_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/mlx_vlm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/tokenizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/mlx_vlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/setup.py
```

### Comparing `mlx_vlm-0.0.5/LICENSE` & `mlx_vlm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.5/PKG-INFO` & `mlx_vlm-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-vlm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Vision LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/Blaizzy/mlx-vlm
 Author: Prince Canuma
 Author-email: prince.gdt@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 ```python
 import mlx.core as mx
 from mlx_vlm import load, generate
 
 model_path = "mlx-community/llava-1.5-7b-4bit"
 model, processor = load(model_path)
 
-prompt = processor.apply_chat_template(
+prompt = processor.tokenizer.apply_chat_template(
     [{"role": "user", "content": f"<image>\nWhat are these?"}],
     tokenize=False,
     add_generation_prompt=True,
 )
 
 output = generate(model, processor, "http://images.cocodataset.org/val2017/000000039769.jpg", prompt, verbose=False)
 ```
```

### Comparing `mlx_vlm-0.0.5/README.md` & `mlx_vlm-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ```python
 import mlx.core as mx
 from mlx_vlm import load, generate
 
 model_path = "mlx-community/llava-1.5-7b-4bit"
 model, processor = load(model_path)
 
-prompt = processor.apply_chat_template(
+prompt = processor.tokenizer.apply_chat_template(
     [{"role": "user", "content": f"<image>\nWhat are these?"}],
     tokenize=False,
     add_generation_prompt=True,
 )
 
 output = generate(model, processor, "http://images.cocodataset.org/val2017/000000039769.jpg", prompt, verbose=False)
-```
+```
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/chat_ui.py` & `mlx_vlm-0.0.6/mlx_vlm/chat_ui.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,28 +50,32 @@
 ):
 
     if image_processor is not None:
         tokenizer = processor
     else:
         tokenizer = processor.tokenizer
 
-    input_ids, pixel_values = prepare_inputs(image_processor, processor, image, prompt)
-    logits, cache = model(input_ids, pixel_values)
+    image_token_index = model.config.image_token_index
+    input_ids, pixel_values, mask = prepare_inputs(
+        image_processor, processor, image, prompt, image_token_index
+    )
+    logits, cache = model(input_ids, pixel_values, mask=mask)
     logits = logits[:, -1, :]
     y, _ = sample(logits, temp, top_p)
 
     detokenizer = processor.detokenizer
     detokenizer.reset()
 
     detokenizer.add_token(y.item())
 
     for (token, _), n in zip(
         generate_step(
             model.language_model,
             logits,
+            mask,
             cache,
             temp,
             repetition_penalty,
             repetition_context_size,
             top_p,
         ),
         range(max_tokens),
@@ -85,42 +89,42 @@
         detokenizer.finalize()
         yield detokenizer.last_segment
 
 
 def chat(message, history, temperature, max_tokens):
 
     chat = []
-    for item in history:
-        chat.append(get_message_json(config["model_type"], item[0]))
-        if item[1] is not None:
-            chat.append({"role": "assistant", "content": item[1]})
-
-    if message["files"]:
+    if len(message["files"]) >= 1:
         chat.append(get_message_json(config["model_type"], message["text"]))
     else:
-        raise Exception("Please upload an image. Text only chat is not supported.")
+        raise gr.Error("Please upload an image. Text only chat is not supported.")
 
+    files = message["files"][-1]
     if "chat_template" in processor.__dict__.keys():
         messages = processor.apply_chat_template(
             chat,
             tokenize=False,
             add_generation_prompt=True,
         )
 
     elif "tokenizer" in processor.__dict__.keys():
-        messages = processor.tokenizer.apply_chat_template(
-            chat,
-            tokenize=False,
-            add_generation_prompt=True,
-        )
+        if model.config.model_type != "paligemma":
+            messages = processor.tokenizer.apply_chat_template(
+                chat,
+                tokenize=False,
+                add_generation_prompt=True,
+            )
+        else:
+            messages = message["text"]
+
     response = ""
     for chunk in generate(
         model,
         processor,
-        message["files"][0],
+        files,
         messages,
         image_processor,
         temperature,
         max_tokens,
     ):
         response += chunk
         yield response
@@ -130,15 +134,15 @@
     fn=chat,
     title="MLX-VLM Chat UI",
     additional_inputs_accordion=gr.Accordion(
         label="⚙️ Parameters", open=False, render=False
     ),
     additional_inputs=[
         gr.Slider(
-            minimum=0, maximum=1, step=0.1, value=0.9, label="Temperature", render=False
+            minimum=0, maximum=1, step=0.1, value=0.1, label="Temperature", render=False
         ),
         gr.Slider(
             minimum=128,
             maximum=4096,
             step=1,
             value=200,
             label="Max new tokens",
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/convert.py` & `mlx_vlm-0.0.6/mlx_vlm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.5/mlx_vlm/generate.py` & `mlx_vlm-0.0.6/mlx_vlm/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,19 +74,20 @@
         prompt = processor.apply_chat_template(
             [get_message_json(config["model_type"], prompt)],
             tokenize=False,
             add_generation_prompt=True,
         )
 
     elif "tokenizer" in processor.__dict__.keys():
-        prompt = processor.tokenizer.apply_chat_template(
-            [get_message_json(config["model_type"], prompt)],
-            tokenize=False,
-            add_generation_prompt=True,
-        )
+        if model.config.model_type != "paligemma":
+            prompt = processor.tokenizer.apply_chat_template(
+                [get_message_json(config["model_type"], prompt)],
+                tokenize=False,
+                add_generation_prompt=True,
+            )
 
     else:
         ValueError(
             "Error: processor does not have 'chat_template' or 'tokenizer' attribute."
         )
 
     output = generate(
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/base.py` & `mlx_vlm-0.0.6/mlx_vlm/models/base.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/idefics2/idefics2.py` & `mlx_vlm-0.0.6/mlx_vlm/models/idefics2/idefics2.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,17 @@
         image_token_positions = mx.array(np.where(special_image_token_mask)[1])
 
         # Advanced indexing to place reshaped image features at the corresponding positions
         inputs_embeds[0, image_token_positions, :] = reshaped_image_hidden_states
 
         return inputs_embeds
 
-    def __call__(self, input_ids: mx.array, pixel_values: mx.array, cache=None):
+    def __call__(
+        self, input_ids: mx.array, pixel_values: mx.array, mask: mx.array, cache=None
+    ):
         input_embeddings = self.get_input_embeddings(input_ids, pixel_values)
         logits, cache = self.language_model(
             inputs=input_ids, cache=cache, inputs_embeds=input_embeddings
         )
         return logits, cache
 
     @staticmethod
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/idefics2/language.py` & `mlx_vlm-0.0.6/mlx_vlm/models/idefics2/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         self.lm_head = nn.Linear(args.hidden_size, args.vocab_size, bias=False)
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
         inputs_embeds=None,
+        mask: Optional[mx.array] = None,
     ):
         # for passing merged input embeddings
         if inputs_embeds is None:
             h = self.embed_tokens(inputs)
         else:
             h = inputs_embeds
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/idefics2/vision.py` & `mlx_vlm-0.0.6/mlx_vlm/models/idefics2/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/llava/language.py` & `mlx_vlm-0.0.6/mlx_vlm/models/llava/language.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         self.lm_head = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
         inputs_embeds=None,
+        mask: Optional[mx.array] = None,
     ):
         out, cache = self.model(inputs, cache, inputs_embeds)
         return self.lm_head(out), cache
 
     @staticmethod
     def sanitize(weights):
         # Remove unused precomputed rotary freqs
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/llava/llava.py` & `mlx_vlm-0.0.6/mlx_vlm/models/llava/llava.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .vision import VisionConfig, VisionModel
 
 
 @dataclass
 class ModelConfig:
     text_config: TextConfig
     vision_config: VisionConfig
+    model_type: str
     ignore_index: int = -100
     image_token_index: int = 32000
     vision_feature_select_strategy: str = "default"
     vision_feature_layer: int = -2
     vocab_size: int = 32000
 
     @classmethod
@@ -126,15 +127,17 @@
         final_embeddings = [v for p in zip(text_segments, image_embeddings) for v in p]
         final_embeddings += [inputs_embeds[:, start_idx:]]
 
         # Create a final embedding of shape
         # (1, num_image_patches*num_images + sequence_len, embed_dim)
         return mx.concatenate(final_embeddings, axis=1)
 
-    def __call__(self, input_ids: mx.array, pixel_values: mx.array, cache=None):
+    def __call__(
+        self, input_ids: mx.array, pixel_values: mx.array, mask: mx.array, cache=None
+    ):
         input_embddings = self.get_input_embeddings(input_ids, pixel_values)
         logits, cache = self.language_model(
             input_ids, cache=cache, inputs_embeds=input_embddings
         )
         return logits, cache
 
     @staticmethod
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/llava/vision.py` & `mlx_vlm-0.0.6/mlx_vlm/models/llava/vision.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import math
 from dataclasses import dataclass
 from typing import Optional
 
 import mlx.core as mx
 import mlx.nn as nn
+import numpy as np
 
 
 @dataclass
 class VisionConfig:
     model_type: str
     num_hidden_layers: int = 24
     hidden_size: int = 1024
@@ -168,16 +169,18 @@
         batch_size = x.shape[0]
         patch_embeddings = self.patch_embedding(x)
         patch_embeddings = mx.flatten(patch_embeddings, start_axis=1, end_axis=2)
         embed_dim = patch_embeddings.shape[-1]
         cls_embeddings = mx.broadcast_to(
             self.class_embedding, (batch_size, 1, embed_dim)
         )
+        position_ids = mx.array(np.arange(self.num_positions)[None, :])
+
         embeddings = mx.concatenate((cls_embeddings, patch_embeddings), axis=1)
-        embeddings += self.position_embedding.weight
+        embeddings += self.position_embedding(position_ids)
         return embeddings
 
 
 class ClipVisionModel(nn.Module):
     def __init__(self, config: VisionConfig):
         super().__init__()
         self.embeddings = VisionEmbeddings(config)
@@ -215,16 +218,15 @@
         self.vision_model = ClipVisionModel(config)
 
     def __call__(
         self, x: mx.array, output_hidden_states: Optional[bool] = None
     ) -> mx.array:
         return self.vision_model(x, output_hidden_states)
 
-    @staticmethod
-    def sanitize(weights):
+    def sanitize(self, weights):
         sanitized_weights = {}
         for k, v in weights.items():
             if "position_ids" in k:
                 # Remove unused position_ids
                 continue
             elif "patch_embedding.weight" in k:
                 # PyTorch conv2d weight tensors have shape:
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/language.py` & `mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
         self.model = Qwen2Model(args)
 
     def __call__(
         self,
         inputs: mx.array,
         cache=None,
         inputs_embeds=None,
+        mask: Optional[mx.array] = None,
     ):
         out, cache = self.model(inputs, cache, inputs_embeds=inputs_embeds)
         return out, cache
 
     def sanitize(self, weights):
         if (
             self.args.tie_word_embeddings
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/nanoLlava.py` & `mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/nanoLlava.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,21 @@
         final_embeddings = [v for p in zip(text_segments, image_embeddings) for v in p]
         final_embeddings += [inputs_embeds[:, start_idx:]]
 
         # Create a final embedding of shape
         # (1, num_image_patches*num_images + sequence_len, embed_dim)
         return mx.concatenate(final_embeddings, axis=1)
 
-    def __call__(self, input_ids: mx.array, pixel_values: mx.array, cache=None):
+    def __call__(
+        self,
+        input_ids: mx.array,
+        pixel_values: mx.array,
+        mask: Optional[mx.array] = None,
+        cache=None,
+    ):
         input_embeddings = self.get_input_embeddings(input_ids, pixel_values)
         logits, cache = self.language_model(
             inputs=input_ids, cache=cache, inputs_embeds=input_embeddings
         )
         return logits, cache
 
     @staticmethod
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/models/nanoLlava/vision.py` & `mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/vision.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 from dataclasses import dataclass
 from typing import Optional
 
 import mlx.core as mx
 import mlx.nn as nn
+import numpy as np
 
 
 @dataclass
 class VisionConfig:
     model_type: str
     num_hidden_layers: int = 27
     hidden_size: int = 1152
@@ -202,17 +203,17 @@
         self.num_positions = self.num_patches
         self.position_embedding = nn.Embedding(self.num_positions, self.embed_dim)
 
     def __call__(self, x: mx.array) -> mx.array:
         batch_size = x.shape[0]
         patch_embeddings = self.patch_embedding(x)
         patch_embeddings = mx.flatten(patch_embeddings, start_axis=1, end_axis=2)
-
+        self.position_ids = mx.array(np.arange(self.num_positions)[None, :])
         embeddings = patch_embeddings
-        embeddings += self.position_embedding.weight
+        embeddings += self.position_embedding(self.position_ids)
         return embeddings
 
 
 class SigLipVisionModel(nn.Module):
     def __init__(self, config: VisionConfig):
         super().__init__()
         self.embeddings = VisionEmbeddings(config)
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/prompt_utils.py` & `mlx_vlm-0.0.6/mlx_vlm/prompt_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,11 +12,13 @@
     if model_name == "idefics2":
         message = {
             "role": "user",
             "content": [{"type": "image"}, {"type": "text", "text": prompt}],
         }
     elif model_name in ["llava-qwen2", "llava"]:
         message = {"role": "user", "content": f"<image>\n{prompt}"}
+    elif model_name == "paligemma":
+        message = prompt
     else:
         raise ValueError(f"Unsupported model: {model_name}")
 
     return message
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/sample_utils.py` & `mlx_vlm-0.0.6/mlx_vlm/sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.5/mlx_vlm/tests/test_models.py` & `mlx_vlm-0.0.6/mlx_vlm/tests/test_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -171,14 +171,15 @@
             num_channels=3,
             layer_norm_eps=1e-6,
         )
 
         args = llava.ModelConfig(
             text_config=text_config,
             vision_config=vision_config,
+            model_type="llava",
             ignore_index=-100,
             image_token_index=32000,
             vocab_size=32000,
             vision_feature_layer=-2,
             vision_feature_select_strategy="default",
         )
 
@@ -264,10 +265,72 @@
             model.vision_model,
             args.vision_config.model_type,
             args.vision_config.hidden_size,
             args.vision_config.num_channels,
             (args.vision_config.image_size, args.vision_config.image_size),
         )
 
+    def test_paligemma(self):
+        from mlx_vlm.models import paligemma
+
+        text_config = paligemma.TextConfig(
+            model_type="gemma",
+            hidden_size=2048,
+            num_hidden_layers=18,
+            intermediate_size=16384,
+            num_attention_heads=8,
+            rms_norm_eps=1e-6,
+            vocab_size=257216,
+            num_key_value_heads=1,
+            rope_theta=10000.0,
+            rope_traditional=False,
+        )
+
+        vision_config = paligemma.VisionConfig(
+            model_type="siglip_vision_model",
+            num_hidden_layers=27,
+            hidden_size=1152,
+            intermediate_size=4304,
+            num_attention_heads=16,
+            image_size=224,
+            patch_size=14,
+            projection_dim=2048,
+            num_channels=3,
+            layer_norm_eps=1e-6,
+        )
+
+        args = paligemma.ModelConfig(
+            text_config=text_config,
+            vision_config=vision_config,
+            model_type="paligemma",
+            ignore_index=-100,
+            image_token_index=257152,
+            hidden_size=2048,
+            vocab_size=257216,
+        )
+
+        model = paligemma.Model(args)
+
+        self.language_test_runner(
+            model.language_model,
+            args.text_config.model_type,
+            args.text_config.vocab_size,
+            args.text_config.num_hidden_layers,
+        )
+
+        self.mm_projector_test_runner(
+            model.multi_modal_projector,
+            args.vision_config.hidden_size,
+            args.text_config.hidden_size,
+        )
+
+        self.vision_test_runner(
+            model.vision_tower,
+            args.vision_config.model_type,
+            args.vision_config.hidden_size,
+            args.vision_config.num_channels,
+            (args.vision_config.image_size, args.vision_config.image_size),
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm/tokenizer_utils.py` & `mlx_vlm-0.0.6/mlx_vlm/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.5/mlx_vlm/utils.py` & `mlx_vlm-0.0.6/mlx_vlm/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -153,17 +153,19 @@
         text_config = text_config.to_dict()
         config["vision_config"] = vision_config["vision_config"]
         config["text_config"] = text_config
     if model_type == "idefics2":
         config = AutoConfig.from_pretrained(model_path).to_dict()
 
     model_config = model_class.ModelConfig.from_dict(config)
+
     model_config.vision_config = model_class.VisionConfig.from_dict(
         config["vision_config"]
     )
+
     model_config.text_config = model_class.TextConfig.from_dict(config["text_config"])
 
     if hasattr(model_config, "perceiver_config"):
         model_config.perceiver_config = model_class.PerceiverConfig.from_dict(
             config["perceiver_config"]
         )
     model = model_class.Model(model_config)
@@ -474,21 +476,64 @@
         q_bits (int): Bits per weight for quantization.
 
     Returns:
         Tuple: Tuple containing quantized weights and config.
     """
     quantized_config = copy.deepcopy(config)
     vision_intermediate_size = model.config.vision_config.intermediate_size
-    class_predicate = lambda path, m: isinstance(m, nn.Linear) and (
-        path.split(".")[0] not in ["vision_model", "vision_tower"]
-        if any(vision_intermediate_size % size != 0 for size in [64, 128])
-        else not isinstance(m, nn.Embedding)
+    divisor = 64
+    if any(vision_intermediate_size % size != 0 for size in [64, 128]):
+        for name, module in model.named_modules():
+            if (
+                isinstance(module, nn.Linear)
+                or isinstance(module, nn.Embedding)
+                and ("vision_model" in name or "vision_tower" in name)
+            ):
+                out_features, in_features = module.weight.shape
+
+                # Calculate the padding needed for each dimension
+                new_out_features = (
+                    ((out_features // divisor) + 1) * divisor
+                    if out_features % divisor != 0
+                    else out_features
+                )
+                new_in_features = (
+                    ((in_features // divisor) + 1) * divisor
+                    if in_features % divisor != 0
+                    else in_features
+                )
+                if (
+                    out_features == vision_intermediate_size
+                    or in_features == vision_intermediate_size
+                ):
+
+                    # If padding is needed, proceed
+                    if (
+                        new_out_features != out_features
+                        or new_in_features != in_features
+                    ):
+                        # Create new weight and bias tensors
+                        new_weight = mx.zeros((new_out_features, new_in_features))
+                        new_bias = mx.zeros((new_out_features))
+
+                        # Copy existing weights and biases to the new tensors
+                        new_weight[:out_features, :in_features] = module.weight
+                        module.weight = new_weight
+
+                        if hasattr(module, "bias"):
+                            new_bias[:out_features] = module.bias
+                            module.bias = new_bias
+
+    quantized_config["vision_config"]["intermediate_size"] = (
+        ((vision_intermediate_size // divisor) + 1) * divisor
+        if vision_intermediate_size % divisor != 0
+        else vision_intermediate_size
     )
 
-    nn.quantize(model, q_group_size, q_bits, class_predicate=class_predicate)
+    nn.quantize(model, q_group_size, q_bits)
     quantized_config["quantization"] = {"group_size": q_group_size, "bits": q_bits}
     quantized_weights = dict(tree_flatten(model.parameters()))
 
     return quantized_weights, quantized_config
 
 
 def save_config(
@@ -617,30 +662,32 @@
             raise ValueError(f"Failed to load image {image_source} with error: {e}")
     else:
         raise ValueError(
             f"The image {image_source} must be a valid URL or existing file."
         )
 
 
-def prepare_inputs(image_processor, processor, image, prompt):
+def prepare_inputs(image_processor, processor, image, prompt, image_token_index):
     from transformers.image_utils import load_image
 
+    mask = None
     if isinstance(image, str):
         image = load_image(image)
 
     if image_processor is not None:
         text_chunks = [processor(chunk).input_ids for chunk in prompt.split("<image>")]
-        input_ids = mx.array([text_chunks[0] + [-200] + text_chunks[1]])
+        input_ids = mx.array([text_chunks[0] + [image_token_index] + text_chunks[1]])
         pixel_values = image_processor.preprocess(images=[image])[0]
         pixel_values = mx.array(np.expand_dims(pixel_values, axis=0))
     else:
         inputs = processor(prompt, image, return_tensors="np")
         pixel_values = mx.array(inputs["pixel_values"])
         input_ids = mx.array(inputs["input_ids"])
-    return input_ids, pixel_values
+        mask = mx.array(inputs["attention_mask"])
+    return input_ids, pixel_values, mask
 
 
 def sample(logits: mx.array, temp: float, top_p: float) -> Tuple[mx.array, float]:
     softmax_logits = mx.softmax(logits)
 
     if temp == 0:
         token = mx.argmax(logits, axis=-1)
@@ -653,14 +700,15 @@
     prob = softmax_logits[0, token]
     return token, prob
 
 
 def generate_step(
     model: nn.Module,
     prompt: mx.array,
+    mask: mx.array,
     cache=None,
     temp: float = 0.0,
     repetition_penalty: Optional[float] = None,
     repetition_context_size: Optional[int] = 20,
     top_p: float = 1.0,
 ) -> Generator[Tuple[mx.array, mx.array], None, None]:
     """
@@ -690,15 +738,15 @@
 
     repetition_context = prompt.tolist()
 
     if repetition_context_size:
         repetition_context = repetition_context[-repetition_context_size:]
 
     while True:
-        logits, cache = model(y[None], cache=cache)
+        logits, cache = model(y[None], mask=mask, cache=cache)
         logits = logits[:, -1, :]
 
         if repetition_penalty:
             logits = apply_repetition_penalty(
                 logits, repetition_context, repetition_penalty
             )
             y, prob = sample(logits, temp, top_p)
@@ -750,29 +798,33 @@
     if image_processor is not None:
         prompt_tokens = mx.array(processor.encode(prompt))
         tokenizer = processor
     else:
         prompt_tokens = mx.array(processor.tokenizer.encode(prompt))
         tokenizer = processor.tokenizer
 
-    input_ids, pixel_values = prepare_inputs(image_processor, processor, image, prompt)
-    logits, cache = model(input_ids, pixel_values)
+    image_token_index = model.config.image_token_index
+    input_ids, pixel_values, mask = prepare_inputs(
+        image_processor, processor, image, prompt, image_token_index
+    )
+    logits, cache = model(input_ids, pixel_values, mask)
     logits = logits[:, -1, :]
     y, _ = sample(logits, temp, top_p)
 
     tic = time.perf_counter()
     detokenizer = processor.detokenizer
     detokenizer.reset()
 
     detokenizer.add_token(y.item())
 
     for (token, prob), n in zip(
         generate_step(
             model.language_model,
             logits,
+            mask,
             cache,
             temp,
             repetition_penalty,
             repetition_context_size,
             top_p,
         ),
         range(max_tokens),
```

### Comparing `mlx_vlm-0.0.5/mlx_vlm.egg-info/PKG-INFO` & `mlx_vlm-0.0.6/mlx_vlm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-vlm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Vision LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/Blaizzy/mlx-vlm
 Author: Prince Canuma
 Author-email: prince.gdt@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 ```python
 import mlx.core as mx
 from mlx_vlm import load, generate
 
 model_path = "mlx-community/llava-1.5-7b-4bit"
 model, processor = load(model_path)
 
-prompt = processor.apply_chat_template(
+prompt = processor.tokenizer.apply_chat_template(
     [{"role": "user", "content": f"<image>\nWhat are these?"}],
     tokenize=False,
     add_generation_prompt=True,
 )
 
 output = generate(model, processor, "http://images.cocodataset.org/val2017/000000039769.jpg", prompt, verbose=False)
 ```
```

### Comparing `mlx_vlm-0.0.5/setup.py` & `mlx_vlm-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,8 +28,14 @@
     author_email="prince.gdt@gmail.com",
     author="Prince Canuma",
     url="https://github.com/Blaizzy/mlx-vlm",
     license="MIT",
     install_requires=requirements,
     packages=find_packages(where=root_dir),
     python_requires=">=3.8",
+    entry_points={
+        "console_scripts": [
+            "mlx_vlm.convert = mlx_vlm.convert:main",
+            "mlx_vlm.generate = mlx_vlm.generate:main",
+        ]
+    },
 )
```

