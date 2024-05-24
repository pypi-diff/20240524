# Comparing `tmp/clonellm-0.0.1.tar.gz` & `tmp/clonellm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonellm-0.0.1.tar", max compression
+gzip compressed data, was "clonellm-0.0.2.tar", max compression
```

## Comparing `clonellm-0.0.1.tar` & `clonellm-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2024-05-23 08:10:53.973305 clonellm-0.0.1/LICENSE
--rw-r--r--   0        0        0     8200 2024-05-23 08:10:53.973305 clonellm-0.0.1/README.md
--rw-r--r--   0        0        0     1273 2024-05-23 08:10:53.977305 clonellm-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      209 2024-05-23 08:10:53.977305 clonellm-0.0.1/src/clonellm/__init__.py
--rw-r--r--   0        0        0      745 2024-05-23 08:10:53.977305 clonellm-0.0.1/src/clonellm/_base.py
--rw-r--r--   0        0        0     2038 2024-05-23 08:10:53.977305 clonellm-0.0.1/src/clonellm/_prompt.py
--rw-r--r--   0        0        0     1119 2024-05-23 08:10:53.977305 clonellm-0.0.1/src/clonellm/_typing.py
--rw-r--r--   0        0        0     8948 2024-05-23 08:10:53.977305 clonellm-0.0.1/src/clonellm/core.py
--rw-r--r--   0        0        0     3190 2024-05-23 08:10:53.977305 clonellm-0.0.1/src/clonellm/embed.py
--rw-r--r--   0        0        0     1205 2024-05-23 08:10:53.977305 clonellm-0.0.1/src/clonellm/memory.py
--rw-r--r--   0        0        0        0 2024-05-23 08:10:53.977305 clonellm-0.0.1/src/clonellm/py.typed
--rw-r--r--   0        0        0     9041 1970-01-01 00:00:00.000000 clonellm-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-24 08:18:44.196305 clonellm-0.0.2/LICENSE
+-rw-r--r--   0        0        0     9668 2024-05-24 08:18:44.200305 clonellm-0.0.2/README.md
+-rw-r--r--   0        0        0     1274 2024-05-24 08:18:44.200305 clonellm-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      209 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/_base.py
+-rw-r--r--   0        0        0     2038 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/_prompt.py
+-rw-r--r--   0        0        0     1119 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/_typing.py
+-rw-r--r--   0        0        0    10078 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/core.py
+-rw-r--r--   0        0        0     3190 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/embed.py
+-rw-r--r--   0        0        0     1205 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/memory.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/py.typed
+-rw-r--r--   0        0        0    10510 1970-01-01 00:00:00.000000 clonellm-0.0.2/PKG-INFO
```

### Comparing `clonellm-0.0.1/LICENSE` & `clonellm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.1/README.md` & `clonellm-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <p align="center">
-    <img src="docs/assets/images/logo.png" alt="Logo" width="250" />
+    <img src="https://raw.githubusercontent.com/msamsami/clonellm/main/docs/assets/images/logo.png" alt="Logo" width="250" />
 </p>
 <h1 align="center">
     CloneLLM
 </h1>
 <p align="center">
     <p align="center">Create an AI clone of yourself using LLMs.</p>
 </p>   
 
 <h4 align="center">
     <a href="https://pypi.org/project/clonellm/" target="_blank">
-        <img src="https://img.shields.io/badge/release-v0.0.1-green" alt="Latest Release">
+        <img src="https://img.shields.io/badge/release-v0.0.2-green" alt="Latest Release">
     </a>
     <a href="https://pypi.org/project/clonellm/" target="_blank">
         <img src="https://img.shields.io/pypi/v/clonellm.svg" alt="PyPI Version">
     </a>
     <a target="_blank">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" alt="Python Versions">
     </a>
@@ -65,15 +65,15 @@
 
 documents = [
     Document(page_content="My name is Mehdi Samsami."),
     open("cv.txt", "r").read(),
 ]
 ```
 
-**Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings` or any other Langchain's embeddings. Then, initialize a clone with your documents, embedding model, and your referred LLM.
+**Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings` or Langchain's embeddings. Then, initialize a clone with your documents, embedding model, and your referred LLM.
 ```python
 from clonellm import CloneLLM, LiteLLMEmbeddings
 
 embedding = LiteLLMEmbeddings(model="text-embedding-ada-002")
 clone = CloneLLM(model="gpt-4-turbo", documents=documents, embedding=embedding)
 ```
 
@@ -83,31 +83,31 @@
 ```
 
 **Step 4**. Fit the clone to the data (documents).
 ```python
 clone.fit()
 ```
 
-**Step 5**. Use completion to ask questions.
+**Step 5**. Invoke the clone to ask questions.
 ```python
-clone.completion("What's your name?")
+clone.invoke("What's your name?")
 
 # Response: My name is Mehdi Samsami. How can I help you?
 ```
 
 ### Models
 At its core, CloneLLM utilizes LiteLLM for interactions with various LLMs. This is why you can choose from many different providers (100+ LLMs) supported by LiteLLM, including Bedrock, Azure, OpenAI, Cohere, Anthropic, Ollama, Sagemaker, HuggingFace, Replicate, etc.
 
 ### Document loaders
 You can use Langchain's document loaders to seamlessly import data from various sources into `Document` format. Take, for example, text and HTML loaders:
 ```python
 # !pip install unstructured
 from langchain_community.document_loaders import TextLoader, UnstructuredHTMLLoader
 
-documents = TextLoader("cv.txt").load() UnstructuredHTMLLoader("linkedin.html").load()
+documents = TextLoader("cv.txt").load() + UnstructuredHTMLLoader("linkedin.html").load()
 ```
 
 Or JSON loader:
 ```python
 # !pip install jq
 from langchain_community.document_loaders import JSONLoader
 
@@ -115,35 +115,38 @@
     file_path='chat.json',
     jq_schema='.messages[].content',
     text_content=False
 ).load()
 ```
 
 ### Embeddings
-With LiteLLMEmbeddings, CloneLLM allows you to utilize embedding models from a variety of providers supported by LiteLLM. Additionally, you can select any preferred embedding model from Langchain's extensive range. Take, for example, the Hugging Face embedding:
+With `LiteLLMEmbeddings`, CloneLLM allows you to utilize embedding models from a variety of providers supported by LiteLLM. Additionally, you can select any preferred embedding model from Langchain's extensive range. Take, for example, the Hugging Face embedding:
 ```python
 # !pip install --upgrade --quiet sentence_transformers
 from langchain_community.embeddings import HuggingFaceEmbeddings
 from clonellm import CloneLLM
 import os
 
-# os.environ["COHERE_API_KEY"] = "cohere-api-key"
+os.environ["COHERE_API_KEY"] = "cohere-api-key"
 
-embedding = HuggingFaceEmbeddings()
+embedding = HuggingFaceEmbeddings(model_name="sentence-transformers/all-mpnet-base-v2")
 clone = CloneLLM(model="command-xlarge-beta", documents=documents, embedding=embedding)
 ```
 
 Or, the Llama-cpp embedding:
 ```python
 # !pip install --upgrade --quiet llama-cpp-python
 from langchain_community.embeddings import LlamaCppEmbeddings
 from clonellm import CloneLLM
+import os
+
+os.environ["OPENAI_API_KEY"] = "openai-api-key"
 
 embedding = LlamaCppEmbeddings(model_path="ggml-model-q4_0.bin")
-clone = CloneLLM(model="gpt-4-turbo", documents=documents, embedding=embedding)
+clone = CloneLLM(model="gpt-3.5-turbo", documents=documents, embedding=embedding)
 ```
 
 ### User profile
 Create a personalized profile using CloneLLM's `UserProfile`, which allows you to feed detailed personal information into your clone for more customized interactions:
 ```python
 from clonellm import UserProfile
 
@@ -162,85 +165,125 @@
     "full_name": "Mehdi Samsami",
     "age": 28,
     "location": "Shiraz, Iran",
     "expertise": ["Data Science", "AI/ML", "Data Analytics"],
 }
 ```
 
-And finnaly:
+Finnaly:
 ```python
 from clonellm import CloneLLM
 import os
 
-# os.environ["ANTHROPIC_API_KEY"] = "anthropic-api-key"
+os.environ["ANTHROPIC_API_KEY"] = "anthropic-api-key"
 
 clone = CloneLLM(
     model="claude-3-opus-20240229",
     documents=documents,
     embedding=embedding,
     user_profile=profile,
 )
 ```
 
-## Conversation history (memory)
+### Conversation history (memory)
 Enable the memory feature to allow your clone to retain a history of past interactions. This "memory" helps the clone to deliver contextually aware responses by referencing previous dialogues. This is simply done by setting `memory` to True when initializing the clone:
 ```python
 from clonellm import CloneLLM
 import os
 
-# os.environ["HUGGINGFACE_API_KEY"] = "huggingface-api-key"
+os.environ["HUGGINGFACE_API_KEY"] = "huggingface-api-key"
 
 clone = CloneLLM(
     model="meta-llama/Llama-2-70b-chat",
     documents=documents,
     embedding=embedding,
     memory=True,
 )
 ```
 
+### Streaming
+CloneLLM supports streaming responses from the LLM, allowing for real-time processing of text as it is being generated, rather than receiving the whole output at once.
+```python
+from clonellm import CloneLLM, LiteLLMEmbeddings
+import os
+
+os.environ["VERTEXAI_PROJECT"] = "hardy-device-28813"
+os.environ["VERTEXAI_LOCATION"] = "us-central1"
+os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "path/to/your/credentials.json"
+
+embedding = LiteLLMEmbeddings(model="textembedding-gecko@001")
+clone = CloneLLM(model="gemini-1.0-pro", documents=documents, embedding=embedding)
+
+for chunk in clone.stream("Describe yourself in 100 words"):
+    print(chunk, end="", flush=True)
+```
+
 ### Async
-CloneLLM provides asynchronous counterparts to its core methods, enhancing performance in asynchronous programming contexts.
+CloneLLM provides asynchronous counterparts to its core methods, `afit`, `ainvoke`, and `astream`, enhancing performance in asynchronous programming contexts.
 
+#### `ainvoke`
 ```python
 import asyncio
 from clonellm import CloneLLM, LiteLLMEmbeddings
 from langchain_core.documents import Document
 import os
 
-# os.environ["OPENAI_API_KEY"] = "openai-api-key"
+os.environ["OPENAI_API_KEY"] = "openai-api-key"
 
 async def main():
-    documents = [Document(page_content="My name is Mehdi Samsami."), open("cv.txt", "r").read()]
+    documents = [...]
     embedding = LiteLLMEmbeddings(model="text-embedding-ada-002")
     clone = CloneLLM(model="gpt-4o", documents=documents, embedding=embedding)
     await clone.afit()
-    response = await clone.acompletion("Tell me about your skills?")
+    response = await clone.ainvoke("Tell me about your skills?")
     return response
 
 response = asyncio.run(main())
 print(response)
 ```
 
+#### `astream`
+```python
+import asyncio
+from clonellm import CloneLLM, LiteLLMEmbeddings
+from langchain_core.documents import Document
+import os
+
+os.environ["OPENAI_API_KEY"] = "openai-api-key"
+
+async def main():
+    documents = [...]
+    embedding = LiteLLMEmbeddings(model="text-embedding-3-small")
+    clone = CloneLLM(model="gpt-4o", documents=documents, embedding=embedding)
+    await clone.afit()
+    async for chunk in clone.astream("How comfortable are you with remote work?"):
+        print(chunk, end="", flush=True)
+
+asyncio.run(main())
+```
+
 ## Support Us
 If you find CloneLLM useful, please consider showing your support in one of the following ways:
 
-- **Star our GitHub repository:** This helps increase the visibility of our project.
-- **Contribute:** Submit pull requests to help improve the codebase, whether it's adding new features, fixing bugs, or improving documentation.
-- **Share:** Post about CloneLLM on LinkedIn or other social platforms.
+- ⭐ **Star our GitHub repository:** This helps increase the visibility of our project.
+- 💡 **Contribute:** Submit pull requests to help improve the codebase, whether it's adding new features, fixing bugs, or improving documentation.
+- 📰 **Share:** Post about CloneLLM on LinkedIn or other social platforms.
 
 Thank you for your interest in CloneLLM. We look forward to seeing what you'll create with your AI clone!
 
 ## TODO
 - [x] Add pre commit configuration file
 - [x] Add setup.py script
 - [x] Add support for conversation history
 - [ ] Add support for RAG with no embedding (ingest the entire context into the prompt)
 - [x] Add support for string documents
 - [x] Fix mypy errors
-- [ ] Add support for streaming completion
+- [x] Rename `completion` methods to `invoke`
+- [x] Add support for streaming completion
 - [ ] Add support for custom system prompts
+- [ ] Add an attribute to return supported models
 - [x] Add initial version of README
 - [ ] Add documents
 - [ ] Add usage examples
 - [ ] Add initial unit tests
 - [x] Add GitHub workflow to run tests on PR
 - [x] Add GitHub workflow to publish to PyPI on release
```

#### html2text {}

```diff
@@ -18,82 +18,101 @@
 the project directory cd clonellm # Install the package pip install . ``` ##
 Usage ### Getting started **Step 1**. Gather documents that contain relavant
 information about you. These documents form the base from which your AI clone
 will learn to mimic your tone, style, and expertise. ```python from
 langchain_core.documents import Document documents = [ Document
 (page_content="My name is Mehdi Samsami."), open("cv.txt", "r").read(), ] ```
 **Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings`
-or any other Langchain's embeddings. Then, initialize a clone with your
-documents, embedding model, and your referred LLM. ```python from clonellm
-import CloneLLM, LiteLLMEmbeddings embedding = LiteLLMEmbeddings(model="text-
+or Langchain's embeddings. Then, initialize a clone with your documents,
+embedding model, and your referred LLM. ```python from clonellm import
+CloneLLM, LiteLLMEmbeddings embedding = LiteLLMEmbeddings(model="text-
 embedding-ada-002") clone = CloneLLM(model="gpt-4-turbo", documents=documents,
 embedding=embedding) ``` **Step 3**. Configure environment variables to store
 API keys for embedding and LLM models. ```bash export OPENAI_API_KEY=sk-... ```
 **Step 4**. Fit the clone to the data (documents). ```python clone.fit() ```
-**Step 5**. Use completion to ask questions. ```python clone.completion("What's
+**Step 5**. Invoke the clone to ask questions. ```python clone.invoke("What's
 your name?") # Response: My name is Mehdi Samsami. How can I help you? ``` ###
 Models At its core, CloneLLM utilizes LiteLLM for interactions with various
 LLMs. This is why you can choose from many different providers (100+ LLMs)
 supported by LiteLLM, including Bedrock, Azure, OpenAI, Cohere, Anthropic,
 Ollama, Sagemaker, HuggingFace, Replicate, etc. ### Document loaders You can
 use Langchain's document loaders to seamlessly import data from various sources
 into `Document` format. Take, for example, text and HTML loaders: ```python #
 !pip install unstructured from langchain_community.document_loaders import
-TextLoader, UnstructuredHTMLLoader documents = TextLoader("cv.txt").load()
+TextLoader, UnstructuredHTMLLoader documents = TextLoader("cv.txt").load() +
 UnstructuredHTMLLoader("linkedin.html").load() ``` Or JSON loader: ```python #
 !pip install jq from langchain_community.document_loaders import JSONLoader
 documents = JSONLoader( file_path='chat.json', jq_schema='.messages[].content',
-text_content=False ).load() ``` ### Embeddings With LiteLLMEmbeddings, CloneLLM
-allows you to utilize embedding models from a variety of providers supported by
-LiteLLM. Additionally, you can select any preferred embedding model from
-Langchain's extensive range. Take, for example, the Hugging Face embedding:
-```python # !pip install --upgrade --quiet sentence_transformers from
-langchain_community.embeddings import HuggingFaceEmbeddings from clonellm
-import CloneLLM import os # os.environ["COHERE_API_KEY"] = "cohere-api-key"
-embedding = HuggingFaceEmbeddings() clone = CloneLLM(model="command-xlarge-
-beta", documents=documents, embedding=embedding) ``` Or, the Llama-cpp
-embedding: ```python # !pip install --upgrade --quiet llama-cpp-python from
-langchain_community.embeddings import LlamaCppEmbeddings from clonellm import
-CloneLLM embedding = LlamaCppEmbeddings(model_path="ggml-model-q4_0.bin") clone
-= CloneLLM(model="gpt-4-turbo", documents=documents, embedding=embedding) ```
-### User profile Create a personalized profile using CloneLLM's `UserProfile`,
-which allows you to feed detailed personal information into your clone for more
-customized interactions: ```python from clonellm import UserProfile profile =
-UserProfile( first_name="Mehdi", last_name="Samsami", city="Shiraz",
-country="Iran", expertise=["Data Science", "AI/ML", "Data Analytics"], ) ``` Or
-simply define your profile using Python dictionaries: ```python profile =
-{ "full_name": "Mehdi Samsami", "age": 28, "location": "Shiraz, Iran",
-"expertise": ["Data Science", "AI/ML", "Data Analytics"], } ``` And finnaly:
-```python from clonellm import CloneLLM import os # os.environ
-["ANTHROPIC_API_KEY"] = "anthropic-api-key" clone = CloneLLM( model="claude-3-
-opus-20240229", documents=documents, embedding=embedding, user_profile=profile,
-) ``` ## Conversation history (memory) Enable the memory feature to allow your
-clone to retain a history of past interactions. This "memory" helps the clone
-to deliver contextually aware responses by referencing previous dialogues. This
-is simply done by setting `memory` to True when initializing the clone:
-```python from clonellm import CloneLLM import os # os.environ
-["HUGGINGFACE_API_KEY"] = "huggingface-api-key" clone = CloneLLM( model="meta-
-llama/Llama-2-70b-chat", documents=documents, embedding=embedding, memory=True,
-) ``` ### Async CloneLLM provides asynchronous counterparts to its core
-methods, enhancing performance in asynchronous programming contexts. ```python
-import asyncio from clonellm import CloneLLM, LiteLLMEmbeddings from
-langchain_core.documents import Document import os # os.environ
-["OPENAI_API_KEY"] = "openai-api-key" async def main(): documents = [Document
-(page_content="My name is Mehdi Samsami."), open("cv.txt", "r").read()]
-embedding = LiteLLMEmbeddings(model="text-embedding-ada-002") clone = CloneLLM
-(model="gpt-4o", documents=documents, embedding=embedding) await clone.afit()
-response = await clone.acompletion("Tell me about your skills?") return
-response response = asyncio.run(main()) print(response) ``` ## Support Us If
-you find CloneLLM useful, please consider showing your support in one of the
-following ways: - **Star our GitHub repository:** This helps increase the
-visibility of our project. - **Contribute:** Submit pull requests to help
-improve the codebase, whether it's adding new features, fixing bugs, or
-improving documentation. - **Share:** Post about CloneLLM on LinkedIn or other
-social platforms. Thank you for your interest in CloneLLM. We look forward to
-seeing what you'll create with your AI clone! ## TODO - [x] Add pre commit
-configuration file - [x] Add setup.py script - [x] Add support for conversation
-history - [ ] Add support for RAG with no embedding (ingest the entire context
-into the prompt) - [x] Add support for string documents - [x] Fix mypy errors -
-[ ] Add support for streaming completion - [ ] Add support for custom system
-prompts - [x] Add initial version of README - [ ] Add documents - [ ] Add usage
-examples - [ ] Add initial unit tests - [x] Add GitHub workflow to run tests on
-PR - [x] Add GitHub workflow to publish to PyPI on release
+text_content=False ).load() ``` ### Embeddings With `LiteLLMEmbeddings`,
+CloneLLM allows you to utilize embedding models from a variety of providers
+supported by LiteLLM. Additionally, you can select any preferred embedding
+model from Langchain's extensive range. Take, for example, the Hugging Face
+embedding: ```python # !pip install --upgrade --quiet sentence_transformers
+from langchain_community.embeddings import HuggingFaceEmbeddings from clonellm
+import CloneLLM import os os.environ["COHERE_API_KEY"] = "cohere-api-key"
+embedding = HuggingFaceEmbeddings(model_name="sentence-transformers/all-mpnet-
+base-v2") clone = CloneLLM(model="command-xlarge-beta", documents=documents,
+embedding=embedding) ``` Or, the Llama-cpp embedding: ```python # !pip install
+--upgrade --quiet llama-cpp-python from langchain_community.embeddings import
+LlamaCppEmbeddings from clonellm import CloneLLM import os os.environ
+["OPENAI_API_KEY"] = "openai-api-key" embedding = LlamaCppEmbeddings
+(model_path="ggml-model-q4_0.bin") clone = CloneLLM(model="gpt-3.5-turbo",
+documents=documents, embedding=embedding) ``` ### User profile Create a
+personalized profile using CloneLLM's `UserProfile`, which allows you to feed
+detailed personal information into your clone for more customized interactions:
+```python from clonellm import UserProfile profile = UserProfile
+( first_name="Mehdi", last_name="Samsami", city="Shiraz", country="Iran",
+expertise=["Data Science", "AI/ML", "Data Analytics"], ) ``` Or simply define
+your profile using Python dictionaries: ```python profile = { "full_name":
+"Mehdi Samsami", "age": 28, "location": "Shiraz, Iran", "expertise": ["Data
+Science", "AI/ML", "Data Analytics"], } ``` Finnaly: ```python from clonellm
+import CloneLLM import os os.environ["ANTHROPIC_API_KEY"] = "anthropic-api-key"
+clone = CloneLLM( model="claude-3-opus-20240229", documents=documents,
+embedding=embedding, user_profile=profile, ) ``` ### Conversation history
+(memory) Enable the memory feature to allow your clone to retain a history of
+past interactions. This "memory" helps the clone to deliver contextually aware
+responses by referencing previous dialogues. This is simply done by setting
+`memory` to True when initializing the clone: ```python from clonellm import
+CloneLLM import os os.environ["HUGGINGFACE_API_KEY"] = "huggingface-api-key"
+clone = CloneLLM( model="meta-llama/Llama-2-70b-chat", documents=documents,
+embedding=embedding, memory=True, ) ``` ### Streaming CloneLLM supports
+streaming responses from the LLM, allowing for real-time processing of text as
+it is being generated, rather than receiving the whole output at once.
+```python from clonellm import CloneLLM, LiteLLMEmbeddings import os os.environ
+["VERTEXAI_PROJECT"] = "hardy-device-28813" os.environ["VERTEXAI_LOCATION"] =
+"us-central1" os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "path/to/your/
+credentials.json" embedding = LiteLLMEmbeddings(model="textembedding-
+gecko@001") clone = CloneLLM(model="gemini-1.0-pro", documents=documents,
+embedding=embedding) for chunk in clone.stream("Describe yourself in 100
+words"): print(chunk, end="", flush=True) ``` ### Async CloneLLM provides
+asynchronous counterparts to its core methods, `afit`, `ainvoke`, and
+`astream`, enhancing performance in asynchronous programming contexts. ####
+`ainvoke` ```python import asyncio from clonellm import CloneLLM,
+LiteLLMEmbeddings from langchain_core.documents import Document import os
+os.environ["OPENAI_API_KEY"] = "openai-api-key" async def main(): documents =
+[...] embedding = LiteLLMEmbeddings(model="text-embedding-ada-002") clone =
+CloneLLM(model="gpt-4o", documents=documents, embedding=embedding) await
+clone.afit() response = await clone.ainvoke("Tell me about your skills?")
+return response response = asyncio.run(main()) print(response) ``` ####
+`astream` ```python import asyncio from clonellm import CloneLLM,
+LiteLLMEmbeddings from langchain_core.documents import Document import os
+os.environ["OPENAI_API_KEY"] = "openai-api-key" async def main(): documents =
+[...] embedding = LiteLLMEmbeddings(model="text-embedding-3-small") clone =
+CloneLLM(model="gpt-4o", documents=documents, embedding=embedding) await
+clone.afit() async for chunk in clone.astream("How comfortable are you with
+remote work?"): print(chunk, end="", flush=True) asyncio.run(main()) ``` ##
+Support Us If you find CloneLLM useful, please consider showing your support in
+one of the following ways: - â­ **Star our GitHub repository:** This helps
+increase the visibility of our project. - ð¡ **Contribute:** Submit pull
+requests to help improve the codebase, whether it's adding new features, fixing
+bugs, or improving documentation. - ð° **Share:** Post about CloneLLM on
+LinkedIn or other social platforms. Thank you for your interest in CloneLLM. We
+look forward to seeing what you'll create with your AI clone! ## TODO - [x] Add
+pre commit configuration file - [x] Add setup.py script - [x] Add support for
+conversation history - [ ] Add support for RAG with no embedding (ingest the
+entire context into the prompt) - [x] Add support for string documents - [x]
+Fix mypy errors - [x] Rename `completion` methods to `invoke` - [x] Add support
+for streaming completion - [ ] Add support for custom system prompts - [ ] Add
+an attribute to return supported models - [x] Add initial version of README -
+[ ] Add documents - [ ] Add usage examples - [ ] Add initial unit tests - [x]
+Add GitHub workflow to run tests on PR - [x] Add GitHub workflow to publish to
+PyPI on release
```

### Comparing `clonellm-0.0.1/pyproject.toml` & `clonellm-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "clonellm"
-version = "0.0.1"
-description = "Python package to create an AI clone of yourself using LLMs"
+version = "0.0.2"
+description = "Python package to create an AI clone of yourself using LLMs."
 packages = [{ from = "src", include = "clonellm" }]
 license = "MIT"
 authors = ["Mehdi Samsami <mehdisamsami@live.com>"]
 readme = "README.md"
 keywords = ["llm", "language models", "nlp", "rag", "ai", "ai clone"]
 repository = "https://github.com/msamsami/clonellm"
```

### Comparing `clonellm-0.0.1/src/clonellm/_base.py` & `clonellm-0.0.2/src/clonellm/_base.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.1/src/clonellm/_prompt.py` & `clonellm-0.0.2/src/clonellm/_prompt.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.1/src/clonellm/_typing.py` & `clonellm-0.0.2/src/clonellm/_typing.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.1/src/clonellm/core.py` & `clonellm-0.0.2/src/clonellm/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import json
 import logging
-from typing import Any, Optional
+from typing import Any, AsyncIterator, Iterator, Optional
 from typing_extensions import Self
 import uuid
 
 from langchain.chains.combine_documents import create_stuff_documents_chain
 from langchain.chains.history_aware_retriever import create_history_aware_retriever
 from langchain.chains.retrieval import create_retrieval_chain
 from langchain.text_splitter import CharacterTextSplitter, TextSplitter
@@ -174,33 +174,59 @@
             get_session_history,
             input_messages_key="input",
             history_messages_key="chat_history",
             output_messages_key="answer",
             output_parser=StrOutputParser(),
         )
 
-    def completion(self, prompt: str) -> str:
+    def invoke(self, prompt: str) -> str:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             response = rag_chain_with_history.invoke({"input": prompt}, config={"configurable": {"session_id": self._session_id}})
             return response["answer"]  # type: ignore[no-any-return]
         rag_chain = self._get_rag_chain()
         return rag_chain.invoke(prompt)
 
-    async def acompletion(self, prompt: str) -> str:
+    async def ainvoke(self, prompt: str) -> str:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             response = await rag_chain_with_history.ainvoke(
                 {"input": prompt}, config={"configurable": {"session_id": self._session_id}}
             )
             return response["answer"]  # type: ignore[no-any-return]
         rag_chain = self._get_rag_chain()
         return await rag_chain.ainvoke(prompt)
 
+    def stream(self, prompt: str) -> Iterator[str]:
+        self._check_is_fitted()
+        if self.memory:
+            rag_chain_with_history = self._get_rag_chain_with_history()
+            iterator = rag_chain_with_history.stream({"input": prompt}, config={"configurable": {"session_id": self._session_id}})
+            for chunk in iterator:
+                if "answer" in chunk:
+                    yield chunk["answer"]
+                else:
+                    yield ""
+        rag_chain = self._get_rag_chain()
+        for chunk in rag_chain.stream(prompt):
+            yield chunk
+
+    async def astream(self, prompt: str) -> AsyncIterator[str]:
+        self._check_is_fitted()
+        if self.memory:
+            rag_chain_with_history = self._get_rag_chain_with_history()
+            async for chunk in rag_chain_with_history.astream(
+                {"input": prompt}, config={"configurable": {"session_id": self._session_id}}
+            ):
+                yield chunk["answer"]
+        rag_chain = self._get_rag_chain()
+        async for chunk in rag_chain.astream(prompt):
+            yield chunk
+
     def clear_memory(self) -> None:
         clear_session_history(self._session_id)
         self._session_id = str(uuid.uuid4())
 
     def __repr__(self) -> str:
         return f"CloneLLM<(model='{self.model}', memory={self.memory})>"
```

### Comparing `clonellm-0.0.1/src/clonellm/embed.py` & `clonellm-0.0.2/src/clonellm/embed.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.1/src/clonellm/memory.py` & `clonellm-0.0.2/src/clonellm/memory.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.1/PKG-INFO` & `clonellm-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: clonellm
-Version: 0.0.1
-Summary: Python package to create an AI clone of yourself using LLMs
+Version: 0.0.2
+Summary: Python package to create an AI clone of yourself using LLMs.
 Home-page: https://github.com/msamsami/clonellm
 License: MIT
 Keywords: llm,language models,nlp,rag,ai,ai clone
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -17,26 +17,26 @@
 Requires-Dist: langchain (>=0.1.17,<0.2.0)
 Requires-Dist: langchain-chroma
 Requires-Dist: litellm (>=1.36.0,<2.0.0)
 Project-URL: Repository, https://github.com/msamsami/clonellm
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="docs/assets/images/logo.png" alt="Logo" width="250" />
+    <img src="https://raw.githubusercontent.com/msamsami/clonellm/main/docs/assets/images/logo.png" alt="Logo" width="250" />
 </p>
 <h1 align="center">
     CloneLLM
 </h1>
 <p align="center">
     <p align="center">Create an AI clone of yourself using LLMs.</p>
 </p>   
 
 <h4 align="center">
     <a href="https://pypi.org/project/clonellm/" target="_blank">
-        <img src="https://img.shields.io/badge/release-v0.0.1-green" alt="Latest Release">
+        <img src="https://img.shields.io/badge/release-v0.0.2-green" alt="Latest Release">
     </a>
     <a href="https://pypi.org/project/clonellm/" target="_blank">
         <img src="https://img.shields.io/pypi/v/clonellm.svg" alt="PyPI Version">
     </a>
     <a target="_blank">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" alt="Python Versions">
     </a>
@@ -87,15 +87,15 @@
 
 documents = [
     Document(page_content="My name is Mehdi Samsami."),
     open("cv.txt", "r").read(),
 ]
 ```
 
-**Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings` or any other Langchain's embeddings. Then, initialize a clone with your documents, embedding model, and your referred LLM.
+**Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings` or Langchain's embeddings. Then, initialize a clone with your documents, embedding model, and your referred LLM.
 ```python
 from clonellm import CloneLLM, LiteLLMEmbeddings
 
 embedding = LiteLLMEmbeddings(model="text-embedding-ada-002")
 clone = CloneLLM(model="gpt-4-turbo", documents=documents, embedding=embedding)
 ```
 
@@ -105,31 +105,31 @@
 ```
 
 **Step 4**. Fit the clone to the data (documents).
 ```python
 clone.fit()
 ```
 
-**Step 5**. Use completion to ask questions.
+**Step 5**. Invoke the clone to ask questions.
 ```python
-clone.completion("What's your name?")
+clone.invoke("What's your name?")
 
 # Response: My name is Mehdi Samsami. How can I help you?
 ```
 
 ### Models
 At its core, CloneLLM utilizes LiteLLM for interactions with various LLMs. This is why you can choose from many different providers (100+ LLMs) supported by LiteLLM, including Bedrock, Azure, OpenAI, Cohere, Anthropic, Ollama, Sagemaker, HuggingFace, Replicate, etc.
 
 ### Document loaders
 You can use Langchain's document loaders to seamlessly import data from various sources into `Document` format. Take, for example, text and HTML loaders:
 ```python
 # !pip install unstructured
 from langchain_community.document_loaders import TextLoader, UnstructuredHTMLLoader
 
-documents = TextLoader("cv.txt").load() UnstructuredHTMLLoader("linkedin.html").load()
+documents = TextLoader("cv.txt").load() + UnstructuredHTMLLoader("linkedin.html").load()
 ```
 
 Or JSON loader:
 ```python
 # !pip install jq
 from langchain_community.document_loaders import JSONLoader
 
@@ -137,35 +137,38 @@
     file_path='chat.json',
     jq_schema='.messages[].content',
     text_content=False
 ).load()
 ```
 
 ### Embeddings
-With LiteLLMEmbeddings, CloneLLM allows you to utilize embedding models from a variety of providers supported by LiteLLM. Additionally, you can select any preferred embedding model from Langchain's extensive range. Take, for example, the Hugging Face embedding:
+With `LiteLLMEmbeddings`, CloneLLM allows you to utilize embedding models from a variety of providers supported by LiteLLM. Additionally, you can select any preferred embedding model from Langchain's extensive range. Take, for example, the Hugging Face embedding:
 ```python
 # !pip install --upgrade --quiet sentence_transformers
 from langchain_community.embeddings import HuggingFaceEmbeddings
 from clonellm import CloneLLM
 import os
 
-# os.environ["COHERE_API_KEY"] = "cohere-api-key"
+os.environ["COHERE_API_KEY"] = "cohere-api-key"
 
-embedding = HuggingFaceEmbeddings()
+embedding = HuggingFaceEmbeddings(model_name="sentence-transformers/all-mpnet-base-v2")
 clone = CloneLLM(model="command-xlarge-beta", documents=documents, embedding=embedding)
 ```
 
 Or, the Llama-cpp embedding:
 ```python
 # !pip install --upgrade --quiet llama-cpp-python
 from langchain_community.embeddings import LlamaCppEmbeddings
 from clonellm import CloneLLM
+import os
+
+os.environ["OPENAI_API_KEY"] = "openai-api-key"
 
 embedding = LlamaCppEmbeddings(model_path="ggml-model-q4_0.bin")
-clone = CloneLLM(model="gpt-4-turbo", documents=documents, embedding=embedding)
+clone = CloneLLM(model="gpt-3.5-turbo", documents=documents, embedding=embedding)
 ```
 
 ### User profile
 Create a personalized profile using CloneLLM's `UserProfile`, which allows you to feed detailed personal information into your clone for more customized interactions:
 ```python
 from clonellm import UserProfile
 
@@ -184,86 +187,126 @@
     "full_name": "Mehdi Samsami",
     "age": 28,
     "location": "Shiraz, Iran",
     "expertise": ["Data Science", "AI/ML", "Data Analytics"],
 }
 ```
 
-And finnaly:
+Finnaly:
 ```python
 from clonellm import CloneLLM
 import os
 
-# os.environ["ANTHROPIC_API_KEY"] = "anthropic-api-key"
+os.environ["ANTHROPIC_API_KEY"] = "anthropic-api-key"
 
 clone = CloneLLM(
     model="claude-3-opus-20240229",
     documents=documents,
     embedding=embedding,
     user_profile=profile,
 )
 ```
 
-## Conversation history (memory)
+### Conversation history (memory)
 Enable the memory feature to allow your clone to retain a history of past interactions. This "memory" helps the clone to deliver contextually aware responses by referencing previous dialogues. This is simply done by setting `memory` to True when initializing the clone:
 ```python
 from clonellm import CloneLLM
 import os
 
-# os.environ["HUGGINGFACE_API_KEY"] = "huggingface-api-key"
+os.environ["HUGGINGFACE_API_KEY"] = "huggingface-api-key"
 
 clone = CloneLLM(
     model="meta-llama/Llama-2-70b-chat",
     documents=documents,
     embedding=embedding,
     memory=True,
 )
 ```
 
+### Streaming
+CloneLLM supports streaming responses from the LLM, allowing for real-time processing of text as it is being generated, rather than receiving the whole output at once.
+```python
+from clonellm import CloneLLM, LiteLLMEmbeddings
+import os
+
+os.environ["VERTEXAI_PROJECT"] = "hardy-device-28813"
+os.environ["VERTEXAI_LOCATION"] = "us-central1"
+os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "path/to/your/credentials.json"
+
+embedding = LiteLLMEmbeddings(model="textembedding-gecko@001")
+clone = CloneLLM(model="gemini-1.0-pro", documents=documents, embedding=embedding)
+
+for chunk in clone.stream("Describe yourself in 100 words"):
+    print(chunk, end="", flush=True)
+```
+
 ### Async
-CloneLLM provides asynchronous counterparts to its core methods, enhancing performance in asynchronous programming contexts.
+CloneLLM provides asynchronous counterparts to its core methods, `afit`, `ainvoke`, and `astream`, enhancing performance in asynchronous programming contexts.
 
+#### `ainvoke`
 ```python
 import asyncio
 from clonellm import CloneLLM, LiteLLMEmbeddings
 from langchain_core.documents import Document
 import os
 
-# os.environ["OPENAI_API_KEY"] = "openai-api-key"
+os.environ["OPENAI_API_KEY"] = "openai-api-key"
 
 async def main():
-    documents = [Document(page_content="My name is Mehdi Samsami."), open("cv.txt", "r").read()]
+    documents = [...]
     embedding = LiteLLMEmbeddings(model="text-embedding-ada-002")
     clone = CloneLLM(model="gpt-4o", documents=documents, embedding=embedding)
     await clone.afit()
-    response = await clone.acompletion("Tell me about your skills?")
+    response = await clone.ainvoke("Tell me about your skills?")
     return response
 
 response = asyncio.run(main())
 print(response)
 ```
 
+#### `astream`
+```python
+import asyncio
+from clonellm import CloneLLM, LiteLLMEmbeddings
+from langchain_core.documents import Document
+import os
+
+os.environ["OPENAI_API_KEY"] = "openai-api-key"
+
+async def main():
+    documents = [...]
+    embedding = LiteLLMEmbeddings(model="text-embedding-3-small")
+    clone = CloneLLM(model="gpt-4o", documents=documents, embedding=embedding)
+    await clone.afit()
+    async for chunk in clone.astream("How comfortable are you with remote work?"):
+        print(chunk, end="", flush=True)
+
+asyncio.run(main())
+```
+
 ## Support Us
 If you find CloneLLM useful, please consider showing your support in one of the following ways:
 
-- **Star our GitHub repository:** This helps increase the visibility of our project.
-- **Contribute:** Submit pull requests to help improve the codebase, whether it's adding new features, fixing bugs, or improving documentation.
-- **Share:** Post about CloneLLM on LinkedIn or other social platforms.
+- ⭐ **Star our GitHub repository:** This helps increase the visibility of our project.
+- 💡 **Contribute:** Submit pull requests to help improve the codebase, whether it's adding new features, fixing bugs, or improving documentation.
+- 📰 **Share:** Post about CloneLLM on LinkedIn or other social platforms.
 
 Thank you for your interest in CloneLLM. We look forward to seeing what you'll create with your AI clone!
 
 ## TODO
 - [x] Add pre commit configuration file
 - [x] Add setup.py script
 - [x] Add support for conversation history
 - [ ] Add support for RAG with no embedding (ingest the entire context into the prompt)
 - [x] Add support for string documents
 - [x] Fix mypy errors
-- [ ] Add support for streaming completion
+- [x] Rename `completion` methods to `invoke`
+- [x] Add support for streaming completion
 - [ ] Add support for custom system prompts
+- [ ] Add an attribute to return supported models
 - [x] Add initial version of README
 - [ ] Add documents
 - [ ] Add usage examples
 - [ ] Add initial unit tests
 - [x] Add GitHub workflow to run tests on PR
 - [x] Add GitHub workflow to publish to PyPI on release
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: clonellm Version: 0.0.1 Summary: Python package to
-create an AI clone of yourself using LLMs Home-page: https://github.com/
+Metadata-Version: 2.1 Name: clonellm Version: 0.0.2 Summary: Python package to
+create an AI clone of yourself using LLMs. Home-page: https://github.com/
 msamsami/clonellm License: MIT Keywords: llm,language models,nlp,rag,ai,ai
 clone Author: Mehdi Samsami Author-email: mehdisamsami@live.com Requires-
 Python: >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: langchain (>=0.1.17,<0.2.0) Requires-
@@ -30,82 +30,101 @@
 the project directory cd clonellm # Install the package pip install . ``` ##
 Usage ### Getting started **Step 1**. Gather documents that contain relavant
 information about you. These documents form the base from which your AI clone
 will learn to mimic your tone, style, and expertise. ```python from
 langchain_core.documents import Document documents = [ Document
 (page_content="My name is Mehdi Samsami."), open("cv.txt", "r").read(), ] ```
 **Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings`
-or any other Langchain's embeddings. Then, initialize a clone with your
-documents, embedding model, and your referred LLM. ```python from clonellm
-import CloneLLM, LiteLLMEmbeddings embedding = LiteLLMEmbeddings(model="text-
+or Langchain's embeddings. Then, initialize a clone with your documents,
+embedding model, and your referred LLM. ```python from clonellm import
+CloneLLM, LiteLLMEmbeddings embedding = LiteLLMEmbeddings(model="text-
 embedding-ada-002") clone = CloneLLM(model="gpt-4-turbo", documents=documents,
 embedding=embedding) ``` **Step 3**. Configure environment variables to store
 API keys for embedding and LLM models. ```bash export OPENAI_API_KEY=sk-... ```
 **Step 4**. Fit the clone to the data (documents). ```python clone.fit() ```
-**Step 5**. Use completion to ask questions. ```python clone.completion("What's
+**Step 5**. Invoke the clone to ask questions. ```python clone.invoke("What's
 your name?") # Response: My name is Mehdi Samsami. How can I help you? ``` ###
 Models At its core, CloneLLM utilizes LiteLLM for interactions with various
 LLMs. This is why you can choose from many different providers (100+ LLMs)
 supported by LiteLLM, including Bedrock, Azure, OpenAI, Cohere, Anthropic,
 Ollama, Sagemaker, HuggingFace, Replicate, etc. ### Document loaders You can
 use Langchain's document loaders to seamlessly import data from various sources
 into `Document` format. Take, for example, text and HTML loaders: ```python #
 !pip install unstructured from langchain_community.document_loaders import
-TextLoader, UnstructuredHTMLLoader documents = TextLoader("cv.txt").load()
+TextLoader, UnstructuredHTMLLoader documents = TextLoader("cv.txt").load() +
 UnstructuredHTMLLoader("linkedin.html").load() ``` Or JSON loader: ```python #
 !pip install jq from langchain_community.document_loaders import JSONLoader
 documents = JSONLoader( file_path='chat.json', jq_schema='.messages[].content',
-text_content=False ).load() ``` ### Embeddings With LiteLLMEmbeddings, CloneLLM
-allows you to utilize embedding models from a variety of providers supported by
-LiteLLM. Additionally, you can select any preferred embedding model from
-Langchain's extensive range. Take, for example, the Hugging Face embedding:
-```python # !pip install --upgrade --quiet sentence_transformers from
-langchain_community.embeddings import HuggingFaceEmbeddings from clonellm
-import CloneLLM import os # os.environ["COHERE_API_KEY"] = "cohere-api-key"
-embedding = HuggingFaceEmbeddings() clone = CloneLLM(model="command-xlarge-
-beta", documents=documents, embedding=embedding) ``` Or, the Llama-cpp
-embedding: ```python # !pip install --upgrade --quiet llama-cpp-python from
-langchain_community.embeddings import LlamaCppEmbeddings from clonellm import
-CloneLLM embedding = LlamaCppEmbeddings(model_path="ggml-model-q4_0.bin") clone
-= CloneLLM(model="gpt-4-turbo", documents=documents, embedding=embedding) ```
-### User profile Create a personalized profile using CloneLLM's `UserProfile`,
-which allows you to feed detailed personal information into your clone for more
-customized interactions: ```python from clonellm import UserProfile profile =
-UserProfile( first_name="Mehdi", last_name="Samsami", city="Shiraz",
-country="Iran", expertise=["Data Science", "AI/ML", "Data Analytics"], ) ``` Or
-simply define your profile using Python dictionaries: ```python profile =
-{ "full_name": "Mehdi Samsami", "age": 28, "location": "Shiraz, Iran",
-"expertise": ["Data Science", "AI/ML", "Data Analytics"], } ``` And finnaly:
-```python from clonellm import CloneLLM import os # os.environ
-["ANTHROPIC_API_KEY"] = "anthropic-api-key" clone = CloneLLM( model="claude-3-
-opus-20240229", documents=documents, embedding=embedding, user_profile=profile,
-) ``` ## Conversation history (memory) Enable the memory feature to allow your
-clone to retain a history of past interactions. This "memory" helps the clone
-to deliver contextually aware responses by referencing previous dialogues. This
-is simply done by setting `memory` to True when initializing the clone:
-```python from clonellm import CloneLLM import os # os.environ
-["HUGGINGFACE_API_KEY"] = "huggingface-api-key" clone = CloneLLM( model="meta-
-llama/Llama-2-70b-chat", documents=documents, embedding=embedding, memory=True,
-) ``` ### Async CloneLLM provides asynchronous counterparts to its core
-methods, enhancing performance in asynchronous programming contexts. ```python
-import asyncio from clonellm import CloneLLM, LiteLLMEmbeddings from
-langchain_core.documents import Document import os # os.environ
-["OPENAI_API_KEY"] = "openai-api-key" async def main(): documents = [Document
-(page_content="My name is Mehdi Samsami."), open("cv.txt", "r").read()]
-embedding = LiteLLMEmbeddings(model="text-embedding-ada-002") clone = CloneLLM
-(model="gpt-4o", documents=documents, embedding=embedding) await clone.afit()
-response = await clone.acompletion("Tell me about your skills?") return
-response response = asyncio.run(main()) print(response) ``` ## Support Us If
-you find CloneLLM useful, please consider showing your support in one of the
-following ways: - **Star our GitHub repository:** This helps increase the
-visibility of our project. - **Contribute:** Submit pull requests to help
-improve the codebase, whether it's adding new features, fixing bugs, or
-improving documentation. - **Share:** Post about CloneLLM on LinkedIn or other
-social platforms. Thank you for your interest in CloneLLM. We look forward to
-seeing what you'll create with your AI clone! ## TODO - [x] Add pre commit
-configuration file - [x] Add setup.py script - [x] Add support for conversation
-history - [ ] Add support for RAG with no embedding (ingest the entire context
-into the prompt) - [x] Add support for string documents - [x] Fix mypy errors -
-[ ] Add support for streaming completion - [ ] Add support for custom system
-prompts - [x] Add initial version of README - [ ] Add documents - [ ] Add usage
-examples - [ ] Add initial unit tests - [x] Add GitHub workflow to run tests on
-PR - [x] Add GitHub workflow to publish to PyPI on release
+text_content=False ).load() ``` ### Embeddings With `LiteLLMEmbeddings`,
+CloneLLM allows you to utilize embedding models from a variety of providers
+supported by LiteLLM. Additionally, you can select any preferred embedding
+model from Langchain's extensive range. Take, for example, the Hugging Face
+embedding: ```python # !pip install --upgrade --quiet sentence_transformers
+from langchain_community.embeddings import HuggingFaceEmbeddings from clonellm
+import CloneLLM import os os.environ["COHERE_API_KEY"] = "cohere-api-key"
+embedding = HuggingFaceEmbeddings(model_name="sentence-transformers/all-mpnet-
+base-v2") clone = CloneLLM(model="command-xlarge-beta", documents=documents,
+embedding=embedding) ``` Or, the Llama-cpp embedding: ```python # !pip install
+--upgrade --quiet llama-cpp-python from langchain_community.embeddings import
+LlamaCppEmbeddings from clonellm import CloneLLM import os os.environ
+["OPENAI_API_KEY"] = "openai-api-key" embedding = LlamaCppEmbeddings
+(model_path="ggml-model-q4_0.bin") clone = CloneLLM(model="gpt-3.5-turbo",
+documents=documents, embedding=embedding) ``` ### User profile Create a
+personalized profile using CloneLLM's `UserProfile`, which allows you to feed
+detailed personal information into your clone for more customized interactions:
+```python from clonellm import UserProfile profile = UserProfile
+( first_name="Mehdi", last_name="Samsami", city="Shiraz", country="Iran",
+expertise=["Data Science", "AI/ML", "Data Analytics"], ) ``` Or simply define
+your profile using Python dictionaries: ```python profile = { "full_name":
+"Mehdi Samsami", "age": 28, "location": "Shiraz, Iran", "expertise": ["Data
+Science", "AI/ML", "Data Analytics"], } ``` Finnaly: ```python from clonellm
+import CloneLLM import os os.environ["ANTHROPIC_API_KEY"] = "anthropic-api-key"
+clone = CloneLLM( model="claude-3-opus-20240229", documents=documents,
+embedding=embedding, user_profile=profile, ) ``` ### Conversation history
+(memory) Enable the memory feature to allow your clone to retain a history of
+past interactions. This "memory" helps the clone to deliver contextually aware
+responses by referencing previous dialogues. This is simply done by setting
+`memory` to True when initializing the clone: ```python from clonellm import
+CloneLLM import os os.environ["HUGGINGFACE_API_KEY"] = "huggingface-api-key"
+clone = CloneLLM( model="meta-llama/Llama-2-70b-chat", documents=documents,
+embedding=embedding, memory=True, ) ``` ### Streaming CloneLLM supports
+streaming responses from the LLM, allowing for real-time processing of text as
+it is being generated, rather than receiving the whole output at once.
+```python from clonellm import CloneLLM, LiteLLMEmbeddings import os os.environ
+["VERTEXAI_PROJECT"] = "hardy-device-28813" os.environ["VERTEXAI_LOCATION"] =
+"us-central1" os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "path/to/your/
+credentials.json" embedding = LiteLLMEmbeddings(model="textembedding-
+gecko@001") clone = CloneLLM(model="gemini-1.0-pro", documents=documents,
+embedding=embedding) for chunk in clone.stream("Describe yourself in 100
+words"): print(chunk, end="", flush=True) ``` ### Async CloneLLM provides
+asynchronous counterparts to its core methods, `afit`, `ainvoke`, and
+`astream`, enhancing performance in asynchronous programming contexts. ####
+`ainvoke` ```python import asyncio from clonellm import CloneLLM,
+LiteLLMEmbeddings from langchain_core.documents import Document import os
+os.environ["OPENAI_API_KEY"] = "openai-api-key" async def main(): documents =
+[...] embedding = LiteLLMEmbeddings(model="text-embedding-ada-002") clone =
+CloneLLM(model="gpt-4o", documents=documents, embedding=embedding) await
+clone.afit() response = await clone.ainvoke("Tell me about your skills?")
+return response response = asyncio.run(main()) print(response) ``` ####
+`astream` ```python import asyncio from clonellm import CloneLLM,
+LiteLLMEmbeddings from langchain_core.documents import Document import os
+os.environ["OPENAI_API_KEY"] = "openai-api-key" async def main(): documents =
+[...] embedding = LiteLLMEmbeddings(model="text-embedding-3-small") clone =
+CloneLLM(model="gpt-4o", documents=documents, embedding=embedding) await
+clone.afit() async for chunk in clone.astream("How comfortable are you with
+remote work?"): print(chunk, end="", flush=True) asyncio.run(main()) ``` ##
+Support Us If you find CloneLLM useful, please consider showing your support in
+one of the following ways: - â­ **Star our GitHub repository:** This helps
+increase the visibility of our project. - ð¡ **Contribute:** Submit pull
+requests to help improve the codebase, whether it's adding new features, fixing
+bugs, or improving documentation. - ð° **Share:** Post about CloneLLM on
+LinkedIn or other social platforms. Thank you for your interest in CloneLLM. We
+look forward to seeing what you'll create with your AI clone! ## TODO - [x] Add
+pre commit configuration file - [x] Add setup.py script - [x] Add support for
+conversation history - [ ] Add support for RAG with no embedding (ingest the
+entire context into the prompt) - [x] Add support for string documents - [x]
+Fix mypy errors - [x] Rename `completion` methods to `invoke` - [x] Add support
+for streaming completion - [ ] Add support for custom system prompts - [ ] Add
+an attribute to return supported models - [x] Add initial version of README -
+[ ] Add documents - [ ] Add usage examples - [ ] Add initial unit tests - [x]
+Add GitHub workflow to run tests on PR - [x] Add GitHub workflow to publish to
+PyPI on release
```

