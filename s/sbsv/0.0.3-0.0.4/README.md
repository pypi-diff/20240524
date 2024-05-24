# Comparing `tmp/sbsv-0.0.3.tar.gz` & `tmp/sbsv-0.0.4.tar.gz`

## Comparing `sbsv-0.0.3.tar` & `sbsv-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 sbsv-0.0.3/sbsv/__init__.py
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 sbsv-0.0.3/sbsv/sbsv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sbsv-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 sbsv-0.0.3/tests/test_schema.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sbsv-0.0.3/tests/resources/test_schema.sbsv
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 sbsv-0.0.3/tests/resources/test_schema_sub.sbsv
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sbsv-0.0.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sbsv-0.0.3/LICENSE
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 sbsv-0.0.3/README.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 sbsv-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 sbsv-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 sbsv-0.0.4/sbsv/__init__.py
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 sbsv-0.0.4/sbsv/sbsv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sbsv-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 sbsv-0.0.4/tests/test_lexer.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 sbsv-0.0.4/tests/test_schema.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sbsv-0.0.4/tests/resources/test_lexer_escape.sbsv
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sbsv-0.0.4/tests/resources/test_schema.sbsv
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 sbsv-0.0.4/tests/resources/test_schema_sub.sbsv
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sbsv-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sbsv-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 sbsv-0.0.4/README.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 sbsv-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 sbsv-0.0.4/PKG-INFO
```

### Comparing `sbsv-0.0.3/sbsv/sbsv.py` & `sbsv-0.0.4/sbsv/sbsv.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,37 +2,72 @@
 
 
 class lexer:
     def __init__(self):
         pass
 
     @staticmethod
+    def replace_escape_sequences(s: str) -> str:
+        escape_dict = {
+            "\\b": "\b",
+            "\\t": "\t",
+            "\\n": "\n",
+            "\\f": "\f",
+            "\\r": "\r",
+            '\\"': '"',
+            "\\/": "/",
+            "\\\\": "\\",
+            "\\[": "[",
+            "\\]": "]",
+        }
+        for key, value in escape_dict.items():
+            s = s.replace(key, value)
+        return s
+
+    @staticmethod
+    def update_token(result: List[str], current: str, should_replace: bool):
+        current = current.strip()
+        if should_replace:
+            current = lexer.replace_escape_sequences(current)
+        result.append(current)
+
+    @staticmethod
     def tokenize(line: str) -> List[str]:
         result = list()
         level = 0
         current = ""
+        escape = False
+        should_replace = False
         for c in range(len(line)):
             char = line[c]
+            if escape:
+                escape = False
+                current += "\\" + char
+                continue
+            if char == "\\":
+                escape = True
+                should_replace = True
+                continue
             if char == "[":
                 level += 1
                 if level == 1:
                     if len(current.strip()) > 0:
-                        result.append(current.strip())
+                        lexer.update_token(result, current, should_replace)
+                        should_replace = False
                     current = ""
                     continue
             elif char == "]":
                 level -= 1
                 if level == 0:
-                    result.append(current.strip())
+                    lexer.update_token(result, current, should_replace)
+                    should_replace = False
                     current = ""
                     continue
             if level > 0:
                 current += char
-        if len(current.strip()) > 0:
-            result.append(current.strip())
         return result
 
     @staticmethod
     def token_split(token: str, delimiter: str) -> Tuple[str, str]:
         tokens = token.split(delimiter, maxsplit=1)
         if len(tokens) == 0:
             return "", ""
```

### Comparing `sbsv-0.0.3/tests/test_schema.py` & `sbsv-0.0.4/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `sbsv-0.0.3/LICENSE` & `sbsv-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sbsv-0.0.3/README.md` & `sbsv-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,19 @@
 ```
 
 ```python
 parser.add_schema("[car] [id?: int] [data: obj[speed: int, power: int, price?: int]]")
 ```
 
 
+### Escape sequences for string
+```
+[car] [id 1] [name "\[name with square bracket\]"]
+```
+
 ## Contribute
 ```shell
 python3 -m pip install --upgrade pip
 python3 -m pip install black
 ```
 You should run `black` linter before commit.
 ```shell
```

### Comparing `sbsv-0.0.3/pyproject.toml` & `sbsv-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sbsv"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Seungheon Han", email="shhan814@gmail.com" },
 ]
 description = "SBSV: Square Brackets Separated Values"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `sbsv-0.0.3/PKG-INFO` & `sbsv-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sbsv
-Version: 0.0.3
+Version: 0.0.4
 Summary: SBSV: Square Brackets Separated Values
 Project-URL: Homepage, https://github.com/hsh814/sbsv
 Project-URL: Issues, https://github.com/hsh814/sbsv/issues
 Author-email: Seungheon Han <shhan814@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -133,14 +133,19 @@
 ```
 
 ```python
 parser.add_schema("[car] [id?: int] [data: obj[speed: int, power: int, price?: int]]")
 ```
 
 
+### Escape sequences for string
+```
+[car] [id 1] [name "\[name with square bracket\]"]
+```
+
 ## Contribute
 ```shell
 python3 -m pip install --upgrade pip
 python3 -m pip install black
 ```
 You should run `black` linter before commit.
 ```shell
```

