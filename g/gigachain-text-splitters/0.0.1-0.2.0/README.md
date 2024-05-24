# Comparing `tmp/gigachain_text_splitters-0.0.1.tar.gz` & `tmp/gigachain_text_splitters-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_text_splitters-0.0.1.tar", max compression
+gzip compressed data, was "gigachain_text_splitters-0.2.0.tar", max compression
```

## Comparing `gigachain_text_splitters-0.0.1.tar` & `gigachain_text_splitters-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1400 2024-03-04 13:38:06.380329 gigachain_text_splitters-0.0.1/README.md
--rw-r--r--   0        0        0     2005 2024-03-04 13:38:06.380645 gigachain_text_splitters-0.0.1/langchain_text_splitters/__init__.py
--rw-r--r--   0        0        0    11313 2024-03-04 13:38:06.381029 gigachain_text_splitters-0.0.1/langchain_text_splitters/base.py
--rw-r--r--   0        0        0    18768 2024-03-04 13:38:06.381284 gigachain_text_splitters-0.0.1/langchain_text_splitters/character.py
--rw-r--r--   0        0        0     5771 2024-03-04 13:38:06.381572 gigachain_text_splitters-0.0.1/langchain_text_splitters/html.py
--rw-r--r--   0        0        0     4149 2024-03-04 13:38:06.381823 gigachain_text_splitters-0.0.1/langchain_text_splitters/json.py
--rw-r--r--   0        0        0      985 2024-03-04 13:38:06.382031 gigachain_text_splitters-0.0.1/langchain_text_splitters/konlpy.py
--rw-r--r--   0        0        0      546 2024-03-04 13:38:06.382239 gigachain_text_splitters-0.0.1/langchain_text_splitters/latex.py
--rw-r--r--   0        0        0     8989 2024-03-04 13:38:06.382644 gigachain_text_splitters-0.0.1/langchain_text_splitters/markdown.py
--rw-r--r--   0        0        0     1042 2024-03-04 13:38:06.382913 gigachain_text_splitters-0.0.1/langchain_text_splitters/nltk.py
--rw-r--r--   0        0        0        0 2024-03-04 13:38:06.383015 gigachain_text_splitters-0.0.1/langchain_text_splitters/py.typed
--rw-r--r--   0        0        0      539 2024-03-04 13:38:06.383278 gigachain_text_splitters-0.0.1/langchain_text_splitters/python.py
--rw-r--r--   0        0        0     2872 2024-03-04 13:38:06.383487 gigachain_text_splitters-0.0.1/langchain_text_splitters/sentence_transformers.py
--rw-r--r--   0        0        0     1762 2024-03-04 13:38:06.383696 gigachain_text_splitters-0.0.1/langchain_text_splitters/spacy.py
--rw-r--r--   0        0        0     6033 2024-03-04 13:38:06.384076 gigachain_text_splitters-0.0.1/langchain_text_splitters/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0     2690 2024-03-04 13:49:40.226364 gigachain_text_splitters-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 gigachain_text_splitters-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1400 2024-04-19 07:38:34.454251 gigachain_text_splitters-0.2.0/README.md
+-rw-r--r--   0        0        0     2070 2024-04-19 07:38:34.454537 gigachain_text_splitters-0.2.0/langchain_text_splitters/__init__.py
+-rw-r--r--   0        0        0    11337 2024-04-19 07:38:34.454983 gigachain_text_splitters-0.2.0/langchain_text_splitters/base.py
+-rw-r--r--   0        0        0    20580 2024-04-19 07:38:34.455265 gigachain_text_splitters-0.2.0/langchain_text_splitters/character.py
+-rw-r--r--   0        0        0    11558 2024-04-19 07:38:34.455916 gigachain_text_splitters-0.2.0/langchain_text_splitters/html.py
+-rw-r--r--   0        0        0     4416 2024-04-19 07:38:34.456237 gigachain_text_splitters-0.2.0/langchain_text_splitters/json.py
+-rw-r--r--   0        0        0      985 2024-04-19 07:38:34.456542 gigachain_text_splitters-0.2.0/langchain_text_splitters/konlpy.py
+-rw-r--r--   0        0        0      546 2024-04-19 07:38:34.456791 gigachain_text_splitters-0.2.0/langchain_text_splitters/latex.py
+-rw-r--r--   0        0        0     9172 2024-05-06 14:45:39.179265 gigachain_text_splitters-0.2.0/langchain_text_splitters/markdown.py
+-rw-r--r--   0        0        0     1042 2024-04-19 07:38:34.457606 gigachain_text_splitters-0.2.0/langchain_text_splitters/nltk.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:38:34.457721 gigachain_text_splitters-0.2.0/langchain_text_splitters/py.typed
+-rw-r--r--   0        0        0      539 2024-04-19 07:38:34.457987 gigachain_text_splitters-0.2.0/langchain_text_splitters/python.py
+-rw-r--r--   0        0        0     2872 2024-04-19 07:38:34.458211 gigachain_text_splitters-0.2.0/langchain_text_splitters/sentence_transformers.py
+-rw-r--r--   0        0        0     1762 2024-04-19 07:38:34.458463 gigachain_text_splitters-0.2.0/langchain_text_splitters/spacy.py
+-rw-r--r--   0        0        0     1073 2024-04-19 07:38:34.458797 gigachain_text_splitters-0.2.0/langchain_text_splitters/xsl/converting_to_header.xslt
+-rw-r--r--   0        0        0     6033 2024-04-19 07:38:34.459093 gigachain_text_splitters-0.2.0/langchain_text_splitters/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0     2775 2024-05-24 11:13:19.720507 gigachain_text_splitters-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2238 1970-01-01 00:00:00.000000 gigachain_text_splitters-0.2.0/PKG-INFO
```

### Comparing `gigachain_text_splitters-0.0.1/README.md` & `gigachain_text_splitters-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![Downloads](https://static.pepy.tech/badge/langchain_text_splitters/month)](https://pepy.tech/project/langchain_text_splitters)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Quick Install
 
 ```bash
-pip install langchain-text-splitters
+pip install gigachain-text-splitters
 ```
 
 ## What is it?
 
 LangChain Text Splitters contains utilities for splitting into chunks a wide variety of text documents.
 
 For full documentation see the [API reference](https://api.python.langchain.com/en/stable/text_splitters_api_reference.html)
```

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/__init__.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,19 @@
     TokenTextSplitter,
     split_text_on_tokens,
 )
 from langchain_text_splitters.character import (
     CharacterTextSplitter,
     RecursiveCharacterTextSplitter,
 )
-from langchain_text_splitters.html import ElementType, HTMLHeaderTextSplitter
+from langchain_text_splitters.html import (
+    ElementType,
+    HTMLHeaderTextSplitter,
+    HTMLSectionSplitter,
+)
 from langchain_text_splitters.json import RecursiveJsonSplitter
 from langchain_text_splitters.konlpy import KonlpyTextSplitter
 from langchain_text_splitters.latex import LatexTextSplitter
 from langchain_text_splitters.markdown import (
     HeaderType,
     LineType,
     MarkdownHeaderTextSplitter,
@@ -61,11 +65,12 @@
     "NLTKTextSplitter",
     "split_text_on_tokens",
     "SentenceTransformersTokenTextSplitter",
     "ElementType",
     "HeaderType",
     "LineType",
     "HTMLHeaderTextSplitter",
+    "HTMLSectionSplitter",
     "MarkdownHeaderTextSplitter",
     "MarkdownTextSplitter",
     "CharacterTextSplitter",
 ]
```

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/base.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,14 +287,15 @@
     HTML = "html"
     SOL = "sol"
     CSHARP = "csharp"
     COBOL = "cobol"
     C = "c"
     LUA = "lua"
     PERL = "perl"
+    HASKELL = "haskell"
 
 
 @dataclass(frozen=True)
 class Tokenizer:
     """Tokenizer data class."""
 
     chunk_overlap: int
```

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/character.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/character.py`

 * *Files 2% similar despite different names*

```diff
@@ -567,13 +567,68 @@
                 "\nDISPLAY ",
                 "\nSTOP RUN.",
                 # Split by the normal type of lines
                 "\n",
                 " ",
                 "",
             ]
-
+        elif language == Language.LUA:
+            return [
+                # Split along variable and table definitions
+                "\nlocal ",
+                # Split along function definitions
+                "\nfunction ",
+                # Split along control flow statements
+                "\nif ",
+                "\nfor ",
+                "\nwhile ",
+                "\nrepeat ",
+                # Split by the normal type of lines
+                "\n\n",
+                "\n",
+                " ",
+                "",
+            ]
+        elif language == Language.HASKELL:
+            return [
+                # Split along function definitions
+                "\nmain :: ",
+                "\nmain = ",
+                "\nlet ",
+                "\nin ",
+                "\ndo ",
+                "\nwhere ",
+                "\n:: ",
+                "\n= ",
+                # Split along type declarations
+                "\ndata ",
+                "\nnewtype ",
+                "\ntype ",
+                "\n:: ",
+                # Split along module declarations
+                "\nmodule ",
+                # Split along import statements
+                "\nimport ",
+                "\nqualified ",
+                "\nimport qualified ",
+                # Split along typeclass declarations
+                "\nclass ",
+                "\ninstance ",
+                # Split along case expressions
+                "\ncase ",
+                # Split along guards in function definitions
+                "\n| ",
+                # Split along record field declarations
+                "\ndata ",
+                "\n= {",
+                "\n, ",
+                # Split by the normal type of lines
+                "\n\n",
+                "\n",
+                " ",
+                "",
+            ]
         else:
             raise ValueError(
                 f"Language {language} is not supported! "
                 f"Please choose from {list(Language)}"
             )
```

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/json.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,20 +44,22 @@
         else:
             # Base case: the item is neither a dict nor a list, so return it unchanged
             return data
 
     def _json_split(
         self,
         data: Dict[str, Any],
-        current_path: List[str] = [],
-        chunks: List[Dict] = [{}],
+        current_path: Optional[List[str]] = None,
+        chunks: Optional[List[Dict]] = None,
     ) -> List[Dict]:
         """
         Split json into maximum size dictionaries while preserving structure.
         """
+        current_path = current_path or []
+        chunks = chunks or [{}]
         if isinstance(data, dict):
             for key, value in data.items():
                 new_path = current_path + [key]
                 chunk_size = self._json_size(chunks[-1])
                 size = self._json_size({key: value})
                 remaining = self.max_chunk_size - chunk_size
 
@@ -90,31 +92,37 @@
 
         # Remove the last chunk if it's empty
         if not chunks[-1]:
             chunks.pop()
         return chunks
 
     def split_text(
-        self, json_data: Dict[str, Any], convert_lists: bool = False
+        self,
+        json_data: Dict[str, Any],
+        convert_lists: bool = False,
+        ensure_ascii: bool = True,
     ) -> List[str]:
         """Splits JSON into a list of JSON formatted strings"""
 
         chunks = self.split_json(json_data=json_data, convert_lists=convert_lists)
 
         # Convert to string
-        return [json.dumps(chunk) for chunk in chunks]
+        return [json.dumps(chunk, ensure_ascii=ensure_ascii) for chunk in chunks]
 
     def create_documents(
         self,
         texts: List[Dict],
         convert_lists: bool = False,
+        ensure_ascii: bool = True,
         metadatas: Optional[List[dict]] = None,
     ) -> List[Document]:
         """Create documents from a list of json objects (Dict)."""
         _metadatas = metadatas or [{}] * len(texts)
         documents = []
         for i, text in enumerate(texts):
-            for chunk in self.split_text(json_data=text, convert_lists=convert_lists):
+            for chunk in self.split_text(
+                json_data=text, convert_lists=convert_lists, ensure_ascii=ensure_ascii
+            ):
                 metadata = copy.deepcopy(_metadatas[i])
                 new_doc = Document(page_content=chunk, metadata=metadata)
                 documents.append(new_doc)
         return documents
```

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/konlpy.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/konlpy.py`

 * *Files identical despite different names*

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/latex.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/latex.py`

 * *Files identical despite different names*

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/markdown.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,17 @@
         initial_metadata: Dict[str, str] = {}
 
         in_code_block = False
         opening_fence = ""
 
         for line in lines:
             stripped_line = line.strip()
-
+            # Remove all non-printable characters from the string, keeping only visible
+            # text.
+            stripped_line = "".join(filter(str.isprintable, stripped_line))
             if not in_code_block:
                 # Exclude inline code spans
                 if stripped_line.startswith("```") and stripped_line.count("```") == 1:
                     in_code_block = True
                     opening_fence = "```"
                 elif stripped_line.startswith("~~~"):
                     in_code_block = True
```

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/nltk.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/nltk.py`

 * *Files identical despite different names*

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/python.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/python.py`

 * *Files identical despite different names*

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/sentence_transformers.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/spacy.py` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/spacy.py`

 * *Files identical despite different names*

### Comparing `gigachain_text_splitters-0.0.1/langchain_text_splitters/xsl/html_chunks_with_headers.xslt` & `gigachain_text_splitters-0.2.0/langchain_text_splitters/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `gigachain_text_splitters-0.0.1/pyproject.toml` & `gigachain_text_splitters-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+
 [tool.poetry]
 name = "gigachain-text-splitters"
-version = "0.0.1"
+version = "0.2.0"
 description = "GigaChain text splitting utilities"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigachain"
 packages = [
     {include = "langchain_text_splitters"}
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gigachain-core = "^0.1.28"
-lxml = {version = "^5.1.0", optional = true}
+gigachain-core = "^0.2.0"
+lxml = {version = ">=4.9.3,<6.0", optional = true}
+beautifulsoup4 = {version = "^4.12.3", optional = true}
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 gigachain-core = {path = "../core", develop = true}
@@ -57,30 +59,30 @@
 
 [tool.poetry.group.test_integration]
 optional = true
 dependencies = {}
 
 [tool.poetry.extras]
 extended_testing = [
-  "lxml",
+  "lxml", "beautifulsoup4"
 ]
 
 [tool.ruff.lint]
 select = [
   "E",  # pycodestyle
   "F",  # pyflakes
   "I",  # isort
   "T201", # print
 ]
 
 [tool.mypy]
 disallow_untyped_defs = "True"
 
 [[tool.mypy.overrides]]
-module = ["transformers", "sentence_transformers", "nltk.tokenize", "konlpy.tag"]
+module = ["transformers", "sentence_transformers", "nltk.tokenize", "konlpy.tag", "bs4"]
 ignore_missing_imports = "True"
 
 [tool.coverage.run]
 omit = ["tests/*", ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
@@ -99,8 +101,7 @@
 # https://docs.pytest.org/en/7.1.x/example/markers.html#registering-markers
 markers = [
   "requires: mark tests as requiring a specific library",
   "asyncio: mark tests as requiring asyncio",
   "compile: mark placeholder test used to compile integration tests without running them",
 ]
 asyncio_mode = "auto"
-
```

### Comparing `gigachain_text_splitters-0.0.1/PKG-INFO` & `gigachain_text_splitters-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: gigachain-text-splitters
-Version: 0.0.1
+Version: 0.2.0
 Summary: GigaChain text splitting utilities
 Home-page: https://github.com/ai-forever/gigachain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: extended-testing
-Requires-Dist: gigachain-core (>=0.1.28,<0.2.0)
-Requires-Dist: lxml (>=5.1.0,<6.0.0) ; extra == "extended-testing"
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0) ; extra == "extended-testing"
+Requires-Dist: gigachain-core (>=0.2.0,<0.3.0)
+Requires-Dist: lxml (>=4.9.3,<6.0) ; extra == "extended-testing"
 Project-URL: Repository, https://github.com/ai-forever/gigachain
 Description-Content-Type: text/markdown
 
 # 🦜✂️ LangChain Text Splitters
 
 [![Downloads](https://static.pepy.tech/badge/langchain_text_splitters/month)](https://pepy.tech/project/langchain_text_splitters)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Quick Install
 
 ```bash
-pip install langchain-text-splitters
+pip install gigachain-text-splitters
 ```
 
 ## What is it?
 
 LangChain Text Splitters contains utilities for splitting into chunks a wide variety of text documents.
 
 For full documentation see the [API reference](https://api.python.langchain.com/en/stable/text_splitters_api_reference.html)
```

