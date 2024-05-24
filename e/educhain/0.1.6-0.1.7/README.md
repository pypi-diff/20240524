# Comparing `tmp/educhain-0.1.6.tar.gz` & `tmp/educhain-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educhain-0.1.6.tar", last modified: Tue Apr  9 08:15:45 2024, max compression
+gzip compressed data, was "educhain-0.1.7.tar", last modified: Thu May 23 20:01:47 2024, max compression
```

## Comparing `educhain-0.1.6.tar` & `educhain-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-04-09 08:15:45.873461 educhain-0.1.6/
--rw-r--r--   0 satvikp    (501) staff       (20)     1066 2024-03-22 08:48:24.000000 educhain-0.1.6/LICENSE
--rw-r--r--   0 satvikp    (501) staff       (20)     3824 2024-04-09 08:15:45.873175 educhain-0.1.6/PKG-INFO
--rw-r--r--   0 satvikp    (501) staff       (20)     2934 2024-04-09 07:28:28.000000 educhain-0.1.6/README.md
-drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-04-09 08:15:45.870324 educhain-0.1.6/educhain/
--rw-r--r--   0 satvikp    (501) staff       (20)      211 2024-04-09 07:28:28.000000 educhain-0.1.6/educhain/__init__.py
--rw-r--r--   0 satvikp    (501) staff       (20)      857 2024-04-01 15:53:35.000000 educhain-0.1.6/educhain/content_engine.py
--rw-r--r--   0 satvikp    (501) staff       (20)      668 2024-04-09 07:28:28.000000 educhain-0.1.6/educhain/models.py
--rw-r--r--   0 satvikp    (501) staff       (20)     1518 2024-04-09 08:00:49.000000 educhain-0.1.6/educhain/qna_engine.py
--rw-r--r--   0 satvikp    (501) staff       (20)     3047 2024-04-09 07:28:28.000000 educhain-0.1.6/educhain/utils.py
-drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-04-09 08:15:45.871692 educhain-0.1.6/educhain.egg-info/
--rw-r--r--   0 satvikp    (501) staff       (20)     3824 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/PKG-INFO
--rw-r--r--   0 satvikp    (501) staff       (20)      293 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/SOURCES.txt
--rw-r--r--   0 satvikp    (501) staff       (20)        1 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/dependency_links.txt
--rw-r--r--   0 satvikp    (501) staff       (20)       85 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/requires.txt
--rw-r--r--   0 satvikp    (501) staff       (20)        9 2024-04-09 08:15:45.000000 educhain-0.1.6/educhain.egg-info/top_level.txt
--rw-r--r--   0 satvikp    (501) staff       (20)       38 2024-04-09 08:15:45.873545 educhain-0.1.6/setup.cfg
--rw-r--r--   0 satvikp    (501) staff       (20)     1040 2024-04-09 08:08:01.000000 educhain-0.1.6/setup.py
+drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-05-23 20:01:47.579896 educhain-0.1.7/
+-rw-r--r--   0 satvikp    (501) staff       (20)     1066 2024-03-22 08:48:24.000000 educhain-0.1.7/LICENSE
+-rw-r--r--   0 satvikp    (501) staff       (20)     3824 2024-05-23 20:01:47.579552 educhain-0.1.7/PKG-INFO
+-rw-r--r--   0 satvikp    (501) staff       (20)     2934 2024-04-09 07:28:28.000000 educhain-0.1.7/README.md
+drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-05-23 20:01:47.578071 educhain-0.1.7/educhain/
+-rw-r--r--   0 satvikp    (501) staff       (20)      211 2024-04-09 07:28:28.000000 educhain-0.1.7/educhain/__init__.py
+-rw-r--r--   0 satvikp    (501) staff       (20)      857 2024-04-01 15:53:35.000000 educhain-0.1.7/educhain/content_engine.py
+-rw-r--r--   0 satvikp    (501) staff       (20)      668 2024-04-09 07:28:28.000000 educhain-0.1.7/educhain/models.py
+-rw-r--r--   0 satvikp    (501) staff       (20)     3259 2024-05-23 19:29:22.000000 educhain-0.1.7/educhain/qna_engine.py
+-rw-r--r--   0 satvikp    (501) staff       (20)     3047 2024-04-09 07:28:28.000000 educhain-0.1.7/educhain/utils.py
+drwxr-xr-x   0 satvikp    (501) staff       (20)        0 2024-05-23 20:01:47.579242 educhain-0.1.7/educhain.egg-info/
+-rw-r--r--   0 satvikp    (501) staff       (20)     3824 2024-05-23 20:01:47.000000 educhain-0.1.7/educhain.egg-info/PKG-INFO
+-rw-r--r--   0 satvikp    (501) staff       (20)      293 2024-05-23 20:01:47.000000 educhain-0.1.7/educhain.egg-info/SOURCES.txt
+-rw-r--r--   0 satvikp    (501) staff       (20)        1 2024-05-23 20:01:47.000000 educhain-0.1.7/educhain.egg-info/dependency_links.txt
+-rw-r--r--   0 satvikp    (501) staff       (20)       85 2024-05-23 20:01:47.000000 educhain-0.1.7/educhain.egg-info/requires.txt
+-rw-r--r--   0 satvikp    (501) staff       (20)        9 2024-05-23 20:01:47.000000 educhain-0.1.7/educhain.egg-info/top_level.txt
+-rw-r--r--   0 satvikp    (501) staff       (20)       38 2024-05-23 20:01:47.579958 educhain-0.1.7/setup.cfg
+-rw-r--r--   0 satvikp    (501) staff       (20)     1040 2024-05-23 20:00:37.000000 educhain-0.1.7/setup.py
```

### Comparing `educhain-0.1.6/LICENSE` & `educhain-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `educhain-0.1.6/PKG-INFO` & `educhain-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educhain
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for generating educational content using Generative AI
 Home-page: https://github.com/satvik314/educhain
 Author: Satvik Paramkusham
 Author-email: satvik@buildfastwithai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `educhain-0.1.6/README.md` & `educhain-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `educhain-0.1.6/educhain/content_engine.py` & `educhain-0.1.7/educhain/content_engine.py`

 * *Files identical despite different names*

### Comparing `educhain-0.1.6/educhain/models.py` & `educhain-0.1.7/educhain/models.py`

 * *Files identical despite different names*

### Comparing `educhain-0.1.6/educhain/qna_engine.py` & `educhain-0.1.7/educhain/qna_engine.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,46 +4,99 @@
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.output_parsers import PydanticOutputParser
 from .models import MCQList ###
 
 
 
-def generate_mcq(topic, level, num=1, llm=None, prompt_template=None, **kwargs):
-    parser = PydanticOutputParser(pydantic_object=MCQList)
-    format_instructions = parser.get_format_instructions()
+def generate_mcq(topic, num=1, llm=None, response_model=None , prompt_template=None, **kwargs):
+
+    if response_model == None:
+      parser = PydanticOutputParser(pydantic_object = MCQList)
+      format_instructions = parser.get_format_instructions()
+    else:
+      parser = PydanticOutputParser(pydantic_object = response_model)
+      format_instructions = parser.get_format_instructions()
 
     if prompt_template is None:
         prompt_template = """
         Generate {num} multiple-choice question (MCQ) based on the given topic and level.
         provide the question, four answer options, and the correct answer.
 
         Topic: {topic}
-        Level: {level}
         """
 
     # Append the JSON format instruction line to the custom prompt template
     prompt_template += "\nThe response should be in JSON format. \n {format_instructions}"
 
     MCQ_prompt = PromptTemplate(
-        input_variables=["num", "topic", "level"],
+        input_variables=["num", "topic"],
         template=prompt_template,
         partial_variables={"format_instructions": format_instructions}
     )
 
     if llm:
         llm = llm
     else:
-        llm = ChatOpenAI(model="gpt-3.5-turbo-0125")
+        llm = ChatOpenAI(model="gpt-3.5-turbo")
 
-    MCQ_chain = LLMChain(llm=llm, prompt=MCQ_prompt)
+    # MCQ_chain = LLMChain(llm=llm, prompt=MCQ_prompt)
+    MCQ_chain = MCQ_prompt | llm
 
     results = MCQ_chain.invoke(
-        {"num": num, "topic": topic, "level": level, **kwargs},
-        return_only_outputs=True
+        {"num": num, "topic": topic, **kwargs},
+        # return_only_outputs=True
+
     )
 
-    results = results["text"]
+    results = results.content
     structured_output = parser.parse(results)
 
     return structured_output
 
+
+
+# def generate_mcq(topic, level = "Intermediate", num=1, llm=None, response_model=None , prompt_template=None, **kwargs):
+
+#     if response_model == None:
+#       parser = PydanticOutputParser(pydantic_object = MCQList)
+#       format_instructions = parser.get_format_instructions()
+#     else:
+#       parser = PydanticOutputParser(pydantic_object = response_model)
+#       format_instructions = parser.get_format_instructions()
+
+#     if prompt_template is None:
+#         prompt_template = """
+#         Generate {num} multiple-choice question (MCQ) based on the given topic and level.
+#         provide the question, four answer options, and the correct answer.
+
+#         Topic: {topic}
+#         Level: {level}
+#         """
+
+#     # Append the JSON format instruction line to the custom prompt template
+#     prompt_template += "\nThe response should be in JSON format. \n {format_instructions}"
+
+#     MCQ_prompt = PromptTemplate(
+#         input_variables=["num", "topic", "level"],
+#         template=prompt_template,
+#         partial_variables={"format_instructions": format_instructions}
+#     )
+
+#     if llm:
+#         llm = llm
+#     else:
+#         llm = ChatOpenAI(model="gpt-3.5-turbo")
+
+#     # MCQ_chain = LLMChain(llm=llm, prompt=MCQ_prompt)
+#     MCQ_chain = MCQ_prompt | llm
+
+#     results = MCQ_chain.invoke(
+#         {"num": num, "topic": topic, "level": level, **kwargs},
+#         # return_only_outputs=True
+
+#     )
+
+#     results = results.content
+#     structured_output = parser.parse(results)
+
+#     return structured_output
```

### Comparing `educhain-0.1.6/educhain/utils.py` & `educhain-0.1.7/educhain/utils.py`

 * *Files identical despite different names*

### Comparing `educhain-0.1.6/educhain.egg-info/PKG-INFO` & `educhain-0.1.7/educhain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educhain
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for generating educational content using Generative AI
 Home-page: https://github.com/satvik314/educhain
 Author: Satvik Paramkusham
 Author-email: satvik@buildfastwithai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `educhain-0.1.6/setup.py` & `educhain-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="educhain",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=[
         "langchain",
         "langchain-community",
         "langchain-openai",
         "openai",
         "python-dotenv",
```

