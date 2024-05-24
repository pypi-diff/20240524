# Comparing `tmp/PyDocSmith-0.1.2.tar.gz` & `tmp/pydocsmith-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDocSmith-0.1.2.tar", last modified: Wed Feb 28 11:52:57 2024, max compression
+gzip compressed data, was "pydocsmith-0.1.3.tar", last modified: Fri May 24 15:54:42 2024, max compression
```

## Comparing `PyDocSmith-0.1.2.tar` & `pydocsmith-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:52:57.763342 PyDocSmith-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-02-28 11:52:57.763342 PyDocSmith-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:52:57.759343 PyDocSmith-0.1.2/PyDocSmith/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/attrdoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/epydoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16077 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/google.py
--rw-r--r--   0 runner    (1001) docker     (127)    17474 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:52:57.763342 PyDocSmith-0.1.2/PyDocSmith/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/_pydoctor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/test_epydoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    37986 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/test_google.py
--rw-r--r--   0 runner    (1001) docker     (127)    31662 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/test_numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/test_parse_from_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/PyDocSmith/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:52:57.763342 PyDocSmith-0.1.2/PyDocSmith.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-02-28 11:52:57.000000 PyDocSmith-0.1.2/PyDocSmith.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-28 11:52:57.000000 PyDocSmith-0.1.2/PyDocSmith.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 11:52:57.000000 PyDocSmith-0.1.2/PyDocSmith.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-28 11:52:57.000000 PyDocSmith-0.1.2/PyDocSmith.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 11:52:57.763342 PyDocSmith-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-28 11:52:47.000000 PyDocSmith-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:54:42.522449 pydocsmith-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-24 15:54:42.522449 pydocsmith-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:54:42.518448 pydocsmith-0.1.3/PyDocSmith/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/attrdoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/epydoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16077 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17474 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:54:42.522449 pydocsmith-0.1.3/PyDocSmith/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/_pydoctor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/test_epydoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39457 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31662 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/test_numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/test_parse_from_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/PyDocSmith/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:54:42.522449 pydocsmith-0.1.3/PyDocSmith.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-24 15:54:42.000000 pydocsmith-0.1.3/PyDocSmith.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-24 15:54:42.000000 pydocsmith-0.1.3/PyDocSmith.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:54:42.000000 pydocsmith-0.1.3/PyDocSmith.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 15:54:42.000000 pydocsmith-0.1.3/PyDocSmith.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:54:42.522449 pydocsmith-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-24 15:54:33.000000 pydocsmith-0.1.3/setup.py
```

### Comparing `PyDocSmith-0.1.2/LICENSE.md` & `pydocsmith-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PKG-INFO` & `pydocsmith-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: PyDocSmith
-Version: 0.1.2
+Version: 0.1.3
 Summary: It parses and composes docstrings in Google, Numpydoc, ReST and Epydoc.
 Home-page: https://github.com/SingularityX-ai/PyDocSmith
 Author: Suman Saurabh
 Author-email: ss.sumansaurabh92@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 The project is a fork from the original project - https://github.com/rr-/docstring_parser/
 
-I have updated it based on use case for - https://www.snorkell.ai/
+
 
 # PyDocSmith
 
 PyDocSmith is a versatile Python package designed for parsing, detecting, and composing docstrings in various styles. It supports multiple docstring conventions, including reStructuredText (reST), Google, NumPydoc, and Epydoc, providing flexibility in documentation practices for Python developers.
 
 ## Features
 
@@ -81,11 +81,13 @@
 ## Things that have been modified wrt to docstring_parser
 
 1. Better heuristics to detect docstring style
 2. Google Docstring has been modified to accommodate Notes, Examples
 3. Sometime GoogleDoc string doesn't have proper indentation specially when generated from LLMs like GPT or Mistral. PyDocSmith can fix those bad docstrings.
 4. Additional test-cases were added to accommodate a different style of GoogleDocstring
 
+I have updated it based on use case for - https://www.penify.dev
+
 ## Contributing
 
 Contributions are welcome! Please submit pull requests or report issues on the project's GitHub page.
```

### Comparing `PyDocSmith-0.1.2/PyDocSmith/__init__.py` & `pydocsmith-0.1.3/PyDocSmith/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/attrdoc.py` & `pydocsmith-0.1.3/PyDocSmith/attrdoc.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/common.py` & `pydocsmith-0.1.3/PyDocSmith/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Common methods for parsing."""
 import enum
+import textwrap
 import typing as T
 
 PARAM_KEYWORDS = {
     "param",
     "parameter",
     "arg",
     "argument",
@@ -173,15 +174,15 @@
         style=None,  # type: T.Optional[DocstringStyle]
     ) -> None:
         """Initialize self."""
         self.short_description = None  # type: T.Optional[str]
         self.long_description = None  # type: T.Optional[str]
         self.blank_after_short_description = False
         self.blank_after_long_description = False
-        self.meta = []  # type: T.List[DocstringMeta]
+        self.meta: T.List[DocstringMeta] = []  # type: T.List[DocstringMeta]
         self.style = style  # type: T.Optional[DocstringStyle]
 
     @property
     def params(self) -> T.List[DocstringParam]:
         """Return a list of information on function params."""
         return [item for item in self.meta if isinstance(item, DocstringParam)]
 
@@ -227,7 +228,24 @@
             item for item in self.meta if isinstance(item, DocstringExample)
         ]
 
     @property
     def notes(self) -> T.List[DocstringNote]:
         """Return a list of information on function notes."""
         return [item for item in self.meta if isinstance(item, DocstringNote)]
+    
+def format_docstring_to_pep257(docstring: Docstring, width: int = 72) -> Docstring:
+    if docstring.short_description:
+        docstring.short_description = textwrap.fill(docstring.short_description.strip(), width)
+    if docstring.long_description:
+        docstring.long_description = textwrap.fill(docstring.long_description.strip(), width)
+
+    for meta in docstring.meta:
+        if meta.description:
+            # Ensure meta descriptions are wrapped according to PEP 8
+            meta.description = textwrap.fill(meta.description.strip(), width)
+        if meta.args:
+            # Clean up args to ensure they are stripped of extra spaces
+            meta.args = [arg.strip() for arg in meta.args if arg.strip()]
+
+    return docstring
+
```

### Comparing `PyDocSmith-0.1.2/PyDocSmith/epydoc.py` & `pydocsmith-0.1.3/PyDocSmith/epydoc.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/google.py` & `pydocsmith-0.1.3/PyDocSmith/google.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/numpydoc.py` & `pydocsmith-0.1.3/PyDocSmith/numpydoc.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/parser.py` & `pydocsmith-0.1.3/PyDocSmith/parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from PyDocSmith import epydoc, google, numpydoc, rest
 from PyDocSmith.attrdoc import add_attribute_docstrings
 from PyDocSmith.common import (
     Docstring,
     DocstringStyle,
     ParseError,
     RenderingStyle,
+    format_docstring_to_pep257,
 )
 
 _STYLE_MAP = {
     DocstringStyle.REST: rest,
     DocstringStyle.GOOGLE: google,
     DocstringStyle.NUMPYDOC: numpydoc,
     DocstringStyle.EPYDOC: epydoc,
@@ -112,21 +113,26 @@
 
 
 def compose(
     docstring: Docstring,
     style: DocstringStyle = DocstringStyle.AUTO,
     rendering_style: RenderingStyle = RenderingStyle.COMPACT,
     indent: str = "    ",
+    line_width: int = 72
 ) -> str:
     """Render a parsed docstring into docstring text.
 
     :param docstring: parsed docstring representation
     :param style: docstring style to render
     :param indent: the characters used as indentation in the docstring string
     :returns: docstring text
     """
     module = _STYLE_MAP[
         docstring.style if style == DocstringStyle.AUTO else style
     ]
+
+    if line_width >= 72:
+        docstring = format_docstring_to_pep257(docstring, width=line_width)
+
     return module.compose(
         docstring, rendering_style=rendering_style, indent=indent
     )
```

### Comparing `PyDocSmith-0.1.2/PyDocSmith/rest.py` & `pydocsmith-0.1.3/PyDocSmith/rest.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/tests/_pydoctor.py` & `pydocsmith-0.1.3/PyDocSmith/tests/_pydoctor.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/tests/test_epydoc.py` & `pydocsmith-0.1.3/PyDocSmith/tests/test_epydoc.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/tests/test_google.py` & `pydocsmith-0.1.3/PyDocSmith/tests/test_google.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tests for Google-style docstring routines."""
 
 import typing as T
 
 import pytest
-from PyDocSmith.common import Docstring, ParseError, RenderingStyle
+from PyDocSmith.common import Docstring, ParseError, RenderingStyle, format_docstring_to_pep257
 from PyDocSmith.google import (
     GoogleParser,
     Section,
     SectionType,
     compose,
     parse,
 )
@@ -978,14 +978,43 @@
     )
 
     assert docstring.params[0].arg_name == "arg0"
     assert docstring.params[0].description == "desc0"
     assert docstring.params[1].arg_name == "arg1"
     assert docstring.params[1].description == "desc1"
 
+def test_very_long_content_for_format_docstring_to_pep257() -> None:
+    # currently failing
+    """Test parsing unknown meta. This is failing"""
+    docstring = parse(
+        """A sample function
+
+        A function the demonstrates docstrings with very long content that should be wrapped to the next line. Additionally, the function has a very long description that should be wrapped to the next line.
+
+        Args:
+            arg1 (int): The firsty arg
+            arg2 (str): The second arg
+            arg3 (float, optional): The third arg. Defaults to 1.0.
+            arg4 (Optional[Dict[str, Any]], optional): The last arg. Defaults to None.
+            arg5 (str, optional): The fifth arg. Defaults to DEFAULT_ARG5.
+
+        Returns:
+            The args packed in a mapping
+        """
+    )
+    docstring = format_docstring_to_pep257(docstring)
+    
+    assert docstring.short_description == "A sample function"
+    assert docstring.long_description == 'A function the demonstrates docstrings with very long content that\nshould be wrapped to the next line. Additionally, the function has a\nvery long description that should be wrapped to the next line.'
+
+    assert docstring.params[0].arg_name == "arg1"
+    assert docstring.params[0].description == "The firsty arg"
+    assert docstring.params[1].arg_name == "arg2"
+    assert docstring.params[1].description == "The second arg"
+
 
 def test_unformatted_valid_docstring() -> None:
     """
     Test parsing a valid docstring without formatting.
     """
 
     docstring = parse(
@@ -998,14 +1027,15 @@
     Raises:
     helo: gejjj
 
     Returns:
     None
     """
     )
+    composed_docstring = compose(docstring)
     assert (
         docstring.short_description == "Set the RPM controller for the object."
     )
     assert len(docstring.params) == 1
     assert docstring.params[0].arg_name == "rpm_controller"
     assert len(docstring.raises) == 1
     assert docstring.raises[0].type_name == "helo"
```

### Comparing `PyDocSmith-0.1.2/PyDocSmith/tests/test_numpydoc.py` & `pydocsmith-0.1.3/PyDocSmith/tests/test_numpydoc.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/tests/test_parse_from_object.py` & `pydocsmith-0.1.3/PyDocSmith/tests/test_parse_from_object.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/tests/test_parser.py` & `pydocsmith-0.1.3/PyDocSmith/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/tests/test_rest.py` & `pydocsmith-0.1.3/PyDocSmith/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/tests/test_util.py` & `pydocsmith-0.1.3/PyDocSmith/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith/util.py` & `pydocsmith-0.1.3/PyDocSmith/util.py`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/PyDocSmith.egg-info/PKG-INFO` & `pydocsmith-0.1.3/PyDocSmith.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: PyDocSmith
-Version: 0.1.2
+Version: 0.1.3
 Summary: It parses and composes docstrings in Google, Numpydoc, ReST and Epydoc.
 Home-page: https://github.com/SingularityX-ai/PyDocSmith
 Author: Suman Saurabh
 Author-email: ss.sumansaurabh92@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 The project is a fork from the original project - https://github.com/rr-/docstring_parser/
 
-I have updated it based on use case for - https://www.snorkell.ai/
+
 
 # PyDocSmith
 
 PyDocSmith is a versatile Python package designed for parsing, detecting, and composing docstrings in various styles. It supports multiple docstring conventions, including reStructuredText (reST), Google, NumPydoc, and Epydoc, providing flexibility in documentation practices for Python developers.
 
 ## Features
 
@@ -81,11 +81,13 @@
 ## Things that have been modified wrt to docstring_parser
 
 1. Better heuristics to detect docstring style
 2. Google Docstring has been modified to accommodate Notes, Examples
 3. Sometime GoogleDoc string doesn't have proper indentation specially when generated from LLMs like GPT or Mistral. PyDocSmith can fix those bad docstrings.
 4. Additional test-cases were added to accommodate a different style of GoogleDocstring
 
+I have updated it based on use case for - https://www.penify.dev
+
 ## Contributing
 
 Contributions are welcome! Please submit pull requests or report issues on the project's GitHub page.
```

### Comparing `PyDocSmith-0.1.2/PyDocSmith.egg-info/SOURCES.txt` & `pydocsmith-0.1.3/PyDocSmith.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/README.md` & `pydocsmith-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The project is a fork from the original project - https://github.com/rr-/docstring_parser/
 
-I have updated it based on use case for - https://www.snorkell.ai/
+
 
 # PyDocSmith
 
 PyDocSmith is a versatile Python package designed for parsing, detecting, and composing docstrings in various styles. It supports multiple docstring conventions, including reStructuredText (reST), Google, NumPydoc, and Epydoc, providing flexibility in documentation practices for Python developers.
 
 ## Features
 
@@ -67,11 +67,13 @@
 ## Things that have been modified wrt to docstring_parser
 
 1. Better heuristics to detect docstring style
 2. Google Docstring has been modified to accommodate Notes, Examples
 3. Sometime GoogleDoc string doesn't have proper indentation specially when generated from LLMs like GPT or Mistral. PyDocSmith can fix those bad docstrings.
 4. Additional test-cases were added to accommodate a different style of GoogleDocstring
 
+I have updated it based on use case for - https://www.penify.dev
+
 ## Contributing
 
 Contributions are welcome! Please submit pull requests or report issues on the project's GitHub page.
```

### Comparing `PyDocSmith-0.1.2/pyproject.toml` & `pydocsmith-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyDocSmith-0.1.2/setup.py` & `pydocsmith-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="PyDocSmith",
-    version="0.1.2",
+    version="0.1.3",
     description="It parses and composes docstrings in Google, Numpydoc, ReST and Epydoc.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Suman Saurabh",
     author_email="ss.sumansaurabh92@gmail.com",
     url="https://github.com/SingularityX-ai/PyDocSmith",
     packages=find_packages(),
```

