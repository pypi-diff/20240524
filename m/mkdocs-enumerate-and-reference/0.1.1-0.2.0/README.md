# Comparing `tmp/mkdocs_enumerate_and_reference-0.1.1.tar.gz` & `tmp/mkdocs_enumerate_and_reference-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_enumerate_and_reference-0.1.1.tar", max compression
+gzip compressed data, was "mkdocs_enumerate_and_reference-0.2.0.tar", max compression
```

## Comparing `mkdocs_enumerate_and_reference-0.1.1.tar` & `mkdocs_enumerate_and_reference-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1902 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/__init__.py
--rw-r--r--   0        0        0     2153 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/enumerate.py
--rw-r--r--   0        0        0     4076 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/plugin.py
--rw-r--r--   0        0        0     1239 2024-05-05 10:55:11.707388 mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/reference.py
--rw-r--r--   0        0        0      908 2024-05-05 10:55:11.711388 mkdocs_enumerate_and_reference-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 mkdocs_enumerate_and_reference-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-24 09:47:51.089192 mkdocs_enumerate_and_reference-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2011 2024-05-24 09:47:51.089192 mkdocs_enumerate_and_reference-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 09:47:51.089192 mkdocs_enumerate_and_reference-0.2.0/mkdocs_enumerate_and_reference/__init__.py
+-rw-r--r--   0        0        0     2330 2024-05-24 09:47:51.089192 mkdocs_enumerate_and_reference-0.2.0/mkdocs_enumerate_and_reference/enumerate.py
+-rw-r--r--   0        0        0     4534 2024-05-24 09:47:51.089192 mkdocs_enumerate_and_reference-0.2.0/mkdocs_enumerate_and_reference/plugin.py
+-rw-r--r--   0        0        0     1226 2024-05-24 09:47:51.089192 mkdocs_enumerate_and_reference-0.2.0/mkdocs_enumerate_and_reference/reference.py
+-rw-r--r--   0        0        0     2067 2024-05-24 09:47:51.093191 mkdocs_enumerate_and_reference-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 mkdocs_enumerate_and_reference-0.2.0/PKG-INFO
```

### Comparing `mkdocs_enumerate_and_reference-0.1.1/LICENSE.txt` & `mkdocs_enumerate_and_reference-0.2.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `mkdocs_enumerate_and_reference-0.1.1/README.md` & `mkdocs_enumerate_and_reference-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-enumerate-and-reference)
 ![PyPI](https://img.shields.io/pypi/v/mkdocs-enumerate-and-reference)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-enumerate-and-reference)
 ![GitHub contributors](https://img.shields.io/github/contributors/raphael-mammeri/mkdocs-enumerate-and-reference)
 ![PyPI - License](https://img.shields.io/pypi/l/mkdocs-enumerate-and-reference)
+![](https://github.com/raphael-mammeri/mkdocs-enumerate-and-reference/actions/workflows/tests.yml/badge.svg)
 
 # Mkdocs Plugin for Enhanced Referencing and Enumeration
 An [Mkdocs](https://www.mkdocs.org) plugin for referencing within documentation, section numbering, and page heading numbering.
 
 ## Features
 1. Referencing: This is the main feature of the plugin. Using a tag system, it allows referencing specific points on pages without having to specify the page path.
 2. Navigation numbering: navigation sections are automatically numbered
```

### Comparing `mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/enumerate.py` & `mkdocs_enumerate_and_reference-0.2.0/mkdocs_enumerate_and_reference/enumerate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 import re
+from typing import Literal
+
+EnumerationValues = Literal["cumulative", "simple"]
+
 
 def cumulative_number(item):
-    anc_numbers = []
-    for a in item.ancestors:
-        if hasattr(a, "number"):
-            anc_numbers.append(a.number)
+    anc_numbers = [
+        a.number for a in item.ancestors[::-1] if hasattr(a, "number")
+    ]
     anc_numbers.append(item.number)
     cnumber = ".".join(anc_numbers)
     item.cnumber = cnumber
     return cnumber
 
 
-def enumerate_navigation(nav, cumulative: bool=True):
+def enumerate_navigation(nav, enumeration_type: EnumerationValues) -> None:
     for i, item in enumerate(nav.items):
-        item.number = str(i+1)
+        item.number = str(i + 1)
+        item.cnumber = str(i + 1)
         if item.title is not None:
-            item.title = ". ".join([item.number, item.title])
-        enumerate_children(item, cumulative)
+            item.title = f"{item.number}. {item.title}"
+        enumerate_children(item, enumeration_type)
 
 
-def enumerate_children(item, cumulative: bool):
-    if item.children is not None: 
+def enumerate_children(item, enumeration_type: EnumerationValues) -> None:
+    if item.children is not None:
         for i, child in enumerate(item.children):
-            number = str(i+1)
+            number = str(i + 1)
             child.number = number
-            if cumulative:
+            if enumeration_type == "cumulative":
                 number = cumulative_number(child)
             if child.title is not None:
-                child.title = " - ".join([number, child.title])
-            enumerate_children(child, cumulative)
+                child.title = f"{number} - {child.title}"
+            enumerate_children(child, enumeration_type)
 
-def add_section_numbers(markdown, lowest_level: int=1):
+
+def add_section_numbers(markdown, lowest_level: int = 1):
     # Initialize section numbers for each level
     section_number = {1: 0, 2: 0, 3: 0, 4: 0, 5: 0, 6: 0}
 
     # Define a function to replace each heading match with its numbered version
-    def replace_heading(match):
+    def replace_heading(match) -> str:
         level = len(match.group(1))
         title = match.group(2)
 
         # Restart subsection numbering when a new section starts
         for i in range(level + 1, 7):
             section_number[i] = 0
 
         # Increment section number for the current level
         section_number[level] += 1
 
         # Add a dot at the end of the numbers for all sections and subsections
-        title_number = ".".join([str(section_number[i]) for i in range(lowest_level, level + 1)])
-        numbered_title = f"{title_number}. {title}" if len(title_number) else title
+        title_number = ".".join(
+            [str(section_number[i]) for i in range(lowest_level, level + 1)],
+        )
+        numbered_title = (
+            f"{title_number}. {title}" if len(title_number) else title
+        )
 
         return f"{'#' * level} {numbered_title}\n"
 
     # Define the regex pattern for detecting headings
-    heading_pattern = re.compile(r'^(\#{1,6})\s+(.+?)\s*$', re.MULTILINE)
+    heading_pattern = re.compile(r"^(\#{1,6})\s+(.+?)\s*$", re.MULTILINE)
 
     # Increment section numbers and replace headings
-    numbered_markdown = heading_pattern.sub(replace_heading, markdown)
-
-    return numbered_markdown
+    return heading_pattern.sub(replace_heading, markdown)
```

### Comparing `mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/plugin.py` & `mkdocs_enumerate_and_reference-0.2.0/mkdocs_enumerate_and_reference/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,138 @@
+import re
+from functools import partial
+from os.path import relpath
+from pathlib import Path
+
 from mkdocs.config import config_options as c
 from mkdocs.config.base import Config
 from mkdocs.plugins import BasePlugin
-from mkdocs_enumerate_and_reference.enumerate import enumerate_navigation, add_section_numbers
+
+from mkdocs_enumerate_and_reference.enumerate import (
+    add_section_numbers,
+    enumerate_navigation,
+)
 from mkdocs_enumerate_and_reference.reference import refactor_admonitions
-import re
-from os.path import relpath
-from functools import partial
 
-class EnumerateOptions(Config):
-    enabled = c.Type(bool, default=True)
-    cumulative = c.Type(bool, default=False)
-
-class NumberHeadingsOptions(Config):
-    enabled = c.Type(bool, default=True)
-    activated = c.Type(bool, default=True)
-    lowest_level = c.Type(int, default=1)
 
 class PluginConfig(Config):
-    enumerate = c.SubConfig(EnumerateOptions)
-    number_headings = c.SubConfig(NumberHeadingsOptions)
+    enumerate_sections = c.Choice(
+        ("ignore", "simple", "cumulative"),
+        default="cumulative",
+    )
+    enumerate_markdown = c.Type(bool, default=True)
+    start_level = c.Type(int, default=1)
+    enumerate_admonitions = c.Choice(
+        ("ignore", "simple", "cumulative"),
+        default="ignore",
+    )
     reference = c.Type(bool, default=True)
-    tags_paths = c.Type(dict, default=dict())
-    tagged_adms = c.Type(dict, default=dict())
-    sources = c.Type(dict, default=dict())
+    tags_paths = c.Type(dict, default={})
+    tagged_adms = c.Type(dict, default={})
+    sources = c.Type(dict, default={})
+
 
 class EnumerateAndReference(BasePlugin[PluginConfig]):
-    def on_nav(self, nav, **kwargs):
-        if self.config.enumerate.enabled:
-            enumerate_navigation(nav, self.config.enumerate.cumulative)
+    def on_nav(self, nav, **kwargs) -> None:
+        # enumerate navigation sections
+        if self.config.enumerate_sections != "ignore":
+            enumerate_navigation(
+                nav,
+                self.config.enumerate_sections,
+            )
+
+        # collect all tags and save their page url in a dict
         for page in nav.pages:
             source = read_source(page)
-            tag_ids = re.findall(r'@tag\((.+?)\)', source)
-            self.config.tags_paths.update({k: page.url for k in tag_ids})
-            # next line is to prevent reading source twice
-            # config.sources.update({page.file.src_path: source})
-    
-    def on_page_markdown(self, markdown, page, config,  **kwargs):
-        if self.config.number_headings.enabled:
-            activated, lowest_level = self.get_number_headings_params(page.meta)
-            if activated:
-                markdown = add_section_numbers(markdown, lowest_level=lowest_level)
+            tag_ids = re.findall(r"@tag\((.+?)\)", source)
+            self.config.tags_paths.update({"#" + k: page.url for k in tag_ids})
 
-        cnumber = page.cnumber if hasattr(page, "cnumber") else None
-        markdown = refactor_admonitions(markdown, cnumber)
+    def on_page_markdown(self, markdown, page, config, **kwargs):
+        # retrieve page specific enumerate markdown params or defaut if None
+        enumerate_markdown, start_level = self.get_enumerate_markdown_params(
+            page.meta,
+        )
+        # refactor markdow to add enumeration
+        if enumerate_markdown:
+            markdown = add_section_numbers(markdown, lowest_level=start_level)
+
+        # enumerate admonitions params
+        if self.config.enumerate_admonitions == "cumulative" and hasattr(
+            page,
+            "cnumber",
+        ):
+            cnumber = page.cnumber
+        else:
+            cnumber = None
+        counter = None if self.config.enumerate_admonitions == "ignore" else 1
+
+        # refactor adminition titles with numbering and tags
+        markdown = refactor_admonitions(markdown, cnumber, counter)
         span = r'<span id="\1"></span>'
-        markdown = re.sub(r'(?<!-)@tag\((.+?)\)', span, markdown)
-        return re.sub(r'-(@tag\(.+?\))', r'\1', markdown)
+        markdown = re.sub(r"(?<!-)@tag\((.+?)\)", span, markdown)
+        return re.sub(r"-(@tag\(.+?\))", r"\1", markdown)
 
-    def get_number_headings_params(self, meta: dict):
+    def get_enumerate_markdown_params(self, meta: dict):
+        try:
+            enumerate_markdown = meta["enumerate-and-reference"][
+                "enumerate_markdown"
+            ]
+        except KeyError:
+            enumerate_markdown = self.config.enumerate_markdown
         try:
-            headings_params = meta["enumerate-and-reference"]["number_headings"]
-            activated = headings_params.get("activated", self.config.number_headings.activated)
-            lowest_level = headings_params.get("lowest_level", self.config.number_headings.lowest_level)
+            start_level = meta["enumerate-and-reference"]["start_level"]
         except KeyError:
-            activated = self.config.number_headings.activated
-            lowest_level = self.config.number_headings.lowest_level
-        return activated, lowest_level
+            start_level = self.config.start_level
+
+        return enumerate_markdown, start_level
 
     def on_page_read_source(self, page, **kwargs):
         try:
             # Only navigation sources read on nav
             source = self.config.sources[page.file.src_path]
         except KeyError:
             source = None
         return source
-    
+
     def on_page_content(self, html, page, **kwargs):
         rel_tr = partial(transform, self.config.tags_paths, page.url)
 
-        def on_match(m):
+        def on_match(m) -> str:
             tag_id = m.group(1)
             return f'<a href="{rel_tr(tag_id)}">'
+
         return re.sub('<a href="(.+?)">', on_match, html)
 
+
 def read_source(page):
     try:
-        with open(page.file.abs_src_path, encoding='utf-8-sig', errors='strict') as f:
+        with Path.open(
+            page.file.abs_src_path,
+            encoding="utf-8-sig",
+            errors="strict",
+        ) as f:
             source = f.read()
-    except OSError:
-        raise OSError(f'File not found: {page.file.src_path}')
-    except ValueError:
-        raise ValueError(f'Encoding error reading file: {page.file.src_path}')
+    except OSError as exc:
+        msg = f"File not found: {page.file.src_path}"
+        raise OSError(msg) from exc
+    except ValueError as exc:
+        msg = f"Encoding error reading file: {page.file.src_path}"
+        raise ValueError(msg) from exc
     return source
 
+
 def transform(tags_paths: dict, url: str, tag_id: str):
-    """Create the link to the referenced tag
+    """Create the link to the referenced tag.
 
     Create the relative path between url of page containing the reference
     and page containing the tag then add the tag to that relative path
     """
     if tag_id in tags_paths:
         rel_path = relpath(tags_paths[tag_id], url)
-        r = f"{rel_path}/#{tag_id}"
-        return f"{rel_path}/#{tag_id}"
-    else:
-        return tag_id
+        return f"{rel_path}/{tag_id}"
+    return tag_id
+
 
 if __name__ == "__main__":
     from mkdocs.commands.serve import serve
-    serve("docs/mkdocs.yml")
+
+    serve("docs/mkdocs.yml")
```

### Comparing `mkdocs_enumerate_and_reference-0.1.1/mkdocs_enumerate_and_reference/reference.py` & `mkdocs_enumerate_and_reference-0.2.0/mkdocs_enumerate_and_reference/reference.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,47 @@
+from __future__ import annotations
+
 import re
 
-def transform(token, name: str, counter, title=None, tag=None):
+
+def transform(token, name: str, counter, title=None, tag=None) -> str:
     if global_cnumber is not None:
         counter = ".".join([global_cnumber, str(counter)])
-    full_title = f"{name.capitalize()} {counter}"
+    if counter is not None:
+        full_title = f"{name.capitalize()} {counter}"
+    else:
+        full_title = f"{name.capitalize()}"
     if title is not None and len(title):
         full_title = " ".join([full_title, f"({title})"])
     if tag is not None:
         full_title = " ".join([full_title, f"@tag({tag})"])
-    return f'{token} {name} "{full_title} :"'
+    return f'{token} {name} "{full_title}"'
+
 
 counter = 1
 global_cnumber = None
+
+
 def on_match(m):
     global counter
-    admonition = m.group(0)
+    # admonition has the group 0
     token = m.group(2)
     name = m.group(3)
     title = m.group(5)
     tag = m.group(7)
-    #print(f"{m.group(0)} --- {m.group(2)} --- {m.group(3)} --- {m.group(5)}--- {m.group(7)} --- \n ")
-    if True:
-        new_admonition = transform(token, name, counter, title, tag)
+    new_admonition = transform(token, name, counter, title, tag)
+    if counter is not None:
         counter += 1
-        return new_admonition
-    else:
-        return admonition
+    return new_admonition
 
-def refactor_admonitions(markdown, cnumber: str = None):
+
+def refactor_admonitions(
+    markdown,
+    cnumber: str | None = None,
+    ncounter=None,
+):
     pattern = r'( *(!!!\+?|\?{3}\+?) *(\w+) *("(.*)")? *(@tag\((.+)\))?)'
     global counter
-    counter = 1
+    counter = ncounter
     global global_cnumber
     global_cnumber = cnumber
-    #rel_tr = partial(transform, config.tags_paths, page.url)
-
-    return re.sub(pattern, on_match, markdown)
+    return re.sub(pattern, on_match, markdown)
```

### Comparing `mkdocs_enumerate_and_reference-0.1.1/PKG-INFO` & `mkdocs_enumerate_and_reference-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-enumerate-and-reference
-Version: 0.1.1
+Version: 0.2.0
 Summary: Mkdocs plugin for numbering and referencing
 License: MIT
 Author: Raphaël Mammeri
 Author-email: raphael.mammeri@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-enumerate-and-reference)
 ![PyPI](https://img.shields.io/pypi/v/mkdocs-enumerate-and-reference)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-enumerate-and-reference)
 ![GitHub contributors](https://img.shields.io/github/contributors/raphael-mammeri/mkdocs-enumerate-and-reference)
 ![PyPI - License](https://img.shields.io/pypi/l/mkdocs-enumerate-and-reference)
+![](https://github.com/raphael-mammeri/mkdocs-enumerate-and-reference/actions/workflows/tests.yml/badge.svg)
 
 # Mkdocs Plugin for Enhanced Referencing and Enumeration
 An [Mkdocs](https://www.mkdocs.org) plugin for referencing within documentation, section numbering, and page heading numbering.
 
 ## Features
 1. Referencing: This is the main feature of the plugin. Using a tag system, it allows referencing specific points on pages without having to specify the page path.
 2. Navigation numbering: navigation sections are automatically numbered
```

