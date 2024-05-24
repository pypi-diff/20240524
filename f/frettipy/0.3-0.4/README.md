# Comparing `tmp/frettipy-0.3.tar.gz` & `tmp/frettipy-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frettipy-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "frettipy-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `frettipy-0.3.tar` & `frettipy-0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      643 2024-01-13 10:08:42.528259 frettipy-0.3/LICENSE
--rw-r--r--   0        0        0     1350 2024-01-13 10:08:42.528259 frettipy-0.3/README.md
--rwxr-xr-x   0        0        0     7975 2024-03-07 13:27:47.500002 frettipy-0.3/frettipy.py
--rw-r--r--   0        0        0      503 2024-03-07 13:12:09.200245 frettipy-0.3/pyproject.toml
--rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 frettipy-0.3/PKG-INFO
+-rw-r--r--   0        0        0      643 2024-01-13 10:08:42.528259 frettipy-0.4/LICENSE
+-rw-r--r--   0        0        0     1424 2024-05-24 13:02:39.678186 frettipy-0.4/README.md
+-rwxr-xr-x   0        0        0     8637 2024-05-24 13:11:57.591643 frettipy-0.4/frettipy.py
+-rw-r--r--   0        0        0      503 2024-03-07 13:12:09.200245 frettipy-0.4/pyproject.toml
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 frettipy-0.4/PKG-INFO
```

### Comparing `frettipy-0.3/LICENSE` & `frettipy-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `frettipy-0.3/README.md` & `frettipy-0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 * Block initiation: no space before colon
 * Space after comma (but not before)
 * No double spaces
 * Single space between non-whitespace character and comment
 * No space before opening bracket (except after keyword)
 * Indentation with four spaces instead of tabs
 * No trailing whitespace
-* No double blank lines
+* No double blank lines (except before class or function)
 * No blank line at end of file
 * No blank line at beginning of file
+* Newline character at end of last line
 
 ## Synopsis
 
 This script formats Python source code following the above style conventions.
 
     frettipy [-f] FILE
```

### Comparing `frettipy-0.3/frettipy.py` & `frettipy-0.4/frettipy.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,43 +6,61 @@
 
 If `-f` is present, `FILE` **is modified in place!** Keep a copy or use version
 control. Otherwise the intended modifications are shown without changing `FILE`.
 
 If `FILE` is a directory, **all .py files in the directory tree are processed!**
 """
 
-__version__ = '0.3'
+__version__ = '0.4'
 
 import os
 import re
 import sys
 
+def info(error=None):
+    if error is not None:
+        print('Error: %s.\n' % error)
+
+    print(__doc__)
+
+    with open(__file__) as self:
+        for rule in re.findall(r'# ([^a-z]+):', self.read()):
+            print('* ' + rule.capitalize())
+
+    sys.exit(error and 1)
+
 def main():
     # parse arguments:
 
     modify = False
+    filename = None
+
+    if len(sys.argv) < 2:
+        info()
 
     for arg in sys.argv[1:]:
         if arg == '-f':
             modify = True
+        elif arg.startswith('-'):
+            info('Invalid argument %s' % arg)
         else:
-            filename = arg
-            break
-    else:
-        print(__doc__)
+            if filename is None:
+                filename = arg
+            else:
+                info('Two filenames specified')
 
-        with open(__file__) as self:
-            for rule in re.findall(r'# ([^a-z]+):', self.read()):
-                print('*', rule.capitalize())
+    if filename is None:
+        info('No filename specified')
 
-        return
+    elif not os.path.exists(filename):
+        info('File "%s" does not exist' % filename)
 
-    # process all Python files in directory tree:
+    elif os.path.isdir(filename):
+        # process all Python files in directory tree:
 
-    if os.path.isdir(filename):
         for path, folders, documents in os.walk(filename):
             folders[:] = [folder for folder in folders
                 if not folder.startswith('.')]
 
             for document in documents:
                 if document.startswith('.'):
                     continue
@@ -211,23 +229,27 @@
 
     # INDENTATION WITH FOUR SPACES INSTEAD OF TABS:
     code = re.sub(r'\t', ' ' * 4, code)
 
     # NO TRAILING WHITESPACE:
     code = re.sub(' +$', '', code, flags=re.MULTILINE)
 
-    # NO DOUBLE BLANK LINES:
-    code = re.sub(r'\n{3,}', '\n' * 2, code)
+    # NO DOUBLE BLANK LINES (EXCEPT BEFORE CLASS OR FUNCTION):
+    code = re.sub(r'\n{4,}(?=class|def)', '\n' * 3, code)
+    code = re.sub(r'\n{3,}(?!class|def)', '\n' * 2, code)
 
     # NO BLANK LINE AT END OF FILE:
     code = re.sub(r'\n{2,}\Z', '\n' * 1, code)
 
     # NO BLANK LINE AT BEGINNING OF FILE:
     code = re.sub(r'\A\n{1,}', '\n' * 0, code)
 
+    # NEWLINE CHARACTER AT END OF LAST LINE:
+    code = re.sub(r'(?<=[^\n])\Z', '\n', code)
+
     return code
 
 def prettifile(filename, modify=True):
     # read file:
 
     with open(filename) as codefile:
         orig = codefile.read()
```

### Comparing `frettipy-0.3/PKG-INFO` & `frettipy-0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frettipy
-Version: 0.3
+Version: 0.4
 Summary: No fretting about pretty Python
 Author: Jan Berges
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Zero-Clause BSD (0BSD)
 Classifier: Programming Language :: Python
 Project-URL: Homepage, https://github.com/janberges/frettipy
@@ -26,17 +26,18 @@
 * Block initiation: no space before colon
 * Space after comma (but not before)
 * No double spaces
 * Single space between non-whitespace character and comment
 * No space before opening bracket (except after keyword)
 * Indentation with four spaces instead of tabs
 * No trailing whitespace
-* No double blank lines
+* No double blank lines (except before class or function)
 * No blank line at end of file
 * No blank line at beginning of file
+* Newline character at end of last line
 
 ## Synopsis
 
 This script formats Python source code following the above style conventions.
 
     frettipy [-f] FILE
```

