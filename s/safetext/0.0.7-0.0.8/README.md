# Comparing `tmp/safetext-0.0.7.tar.gz` & `tmp/safetext-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safetext-0.0.7.tar", last modified: Thu Dec 21 13:43:40 2023, max compression
+gzip compressed data, was "safetext-0.0.8.tar", last modified: Fri May 24 07:45:15 2024, max compression
```

## Comparing `safetext-0.0.7.tar` & `safetext-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.009587 safetext-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-21 13:43:32.000000 safetext-0.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-21 13:43:32.000000 safetext-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-21 13:43:32.000000 safetext-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2023-12-21 13:43:40.009587 safetext-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2023-12-21 13:43:32.000000 safetext-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-21 13:43:32.000000 safetext-0.0.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.005587 safetext-0.0.7/safetext/
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2023-12-21 13:43:32.000000 safetext-0.0.7/safetext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.005587 safetext-0.0.7/safetext/languages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.005587 safetext-0.0.7/safetext/languages/de/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-21 13:43:32.000000 safetext-0.0.7/safetext/languages/de/words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.005587 safetext-0.0.7/safetext/languages/en/
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2023-12-21 13:43:32.000000 safetext-0.0.7/safetext/languages/en/words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.005587 safetext-0.0.7/safetext/languages/es/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-21 13:43:32.000000 safetext-0.0.7/safetext/languages/es/words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.005587 safetext-0.0.7/safetext/languages/pt/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-12-21 13:43:32.000000 safetext-0.0.7/safetext/languages/pt/words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.005587 safetext-0.0.7/safetext/languages/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2023-12-21 13:43:32.000000 safetext-0.0.7/safetext/languages/tr/words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2023-12-21 13:43:32.000000 safetext-0.0.7/safetext/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 13:43:40.005587 safetext-0.0.7/safetext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2023-12-21 13:43:39.000000 safetext-0.0.7/safetext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-21 13:43:39.000000 safetext-0.0.7/safetext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 13:43:39.000000 safetext-0.0.7/safetext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-21 13:43:39.000000 safetext-0.0.7/safetext.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-12-21 13:43:39.000000 safetext-0.0.7/safetext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-21 13:43:39.000000 safetext-0.0.7/safetext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-21 13:43:40.009587 safetext-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-21 13:43:32.000000 safetext-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.911794 safetext-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-24 07:45:08.000000 safetext-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 07:45:08.000000 safetext-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-24 07:45:08.000000 safetext-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 07:45:15.911794 safetext-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-24 07:45:08.000000 safetext-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-24 07:45:08.000000 safetext-0.0.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.907794 safetext-0.0.8/safetext/
+-rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-05-24 07:45:08.000000 safetext-0.0.8/safetext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.903794 safetext-0.0.8/safetext/languages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.907794 safetext-0.0.8/safetext/languages/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-24 07:45:08.000000 safetext-0.0.8/safetext/languages/de/words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.907794 safetext-0.0.8/safetext/languages/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-24 07:45:08.000000 safetext-0.0.8/safetext/languages/en/words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.907794 safetext-0.0.8/safetext/languages/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-24 07:45:08.000000 safetext-0.0.8/safetext/languages/es/words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.907794 safetext-0.0.8/safetext/languages/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-24 07:45:08.000000 safetext-0.0.8/safetext/languages/pt/words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.907794 safetext-0.0.8/safetext/languages/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-24 07:45:08.000000 safetext-0.0.8/safetext/languages/tr/words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-24 07:45:08.000000 safetext-0.0.8/safetext/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:45:15.907794 safetext-0.0.8/safetext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 07:45:15.000000 safetext-0.0.8/safetext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-24 07:45:15.000000 safetext-0.0.8/safetext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:45:15.000000 safetext-0.0.8/safetext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 07:45:15.000000 safetext-0.0.8/safetext.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-24 07:45:15.000000 safetext-0.0.8/safetext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 07:45:15.000000 safetext-0.0.8/safetext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-24 07:45:15.911794 safetext-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-24 07:45:08.000000 safetext-0.0.8/setup.py
```

### Comparing `safetext-0.0.7/CONTRIBUTING.md` & `safetext-0.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/LICENSE` & `safetext-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/PKG-INFO` & `safetext-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetext
-Version: 0.0.7
+Version: 0.0.8
 Summary: Rule-based profanity checking tool for English and Turkish.
 Home-page: https://github.com/deepsafe/safetext
 Author: 
 License: MIT
 Keywords: text,profanity,filtering,turkish,english
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `safetext-0.0.7/README.md` & `safetext-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/safetext/__init__.py` & `safetext-0.0.8/safetext/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from typing import Dict, List, Optional
 
 import requests
 
 from safetext.utils import detect_language_from_srt, detect_language_from_text
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 
 class SafeText:
     """A class to provide text analysis for profanity detection using the built-in ProfanityChecker and
     optionally validating the results against the ModerateContentAPI.
     """
 
@@ -173,38 +173,61 @@
         Initializes the ProfanityChecker with a specified language.
 
         Args:
             language (str): The language code for the profanity list.
         """
         self.language = language
         self._profanity_words = self._load_profanity_list()
+        self._whitelist = self._load_whitelist()
 
     def _load_profanity_list(self) -> List[str]:
         """
         Loads the profanity words list from the corresponding file.
 
         Returns:
             List[str]: A list of profanity words and phrases.
         """
         words_filepath = os.path.join(os.path.dirname(__file__), f"languages/{self.language}/words.txt")
         with open(words_filepath, encoding="utf8") as file:
             return file.read().splitlines()
 
+    def _load_whitelist(self) -> set:
+        """
+        Loads the whitelist of words for the current language.
+
+        Returns:
+            set: A set of words that are whitelisted.
+        """
+        whitelist_filepath = os.path.join(
+            os.path.dirname(__file__), f"languages/{self.language}/whitelist.txt")
+        try:
+            with open(whitelist_filepath, encoding="utf8") as file:
+                return set(file.read().splitlines())
+        except FileNotFoundError:
+            logging.warning(
+                f"Whitelist file not found for language '{self.language}'. Using an empty whitelist.")
+            return set()
+
     def _find_profanities(self, text: str) -> List[Dict]:
         """
         Finds profanities in the given text.
 
         Args:
             text (str): The text to scan for profanities.
 
         Returns:
             List[Dict]: A list of dictionaries, each containing information about a found profanity.
         """
         profanity_infos = []
         lower_text = text.lower()
+
+        # Remove whitelisted words and phrases from the text
+        for white_item in self._whitelist:
+            lower_text = lower_text.replace(white_item.lower(), '')
+
         words = re.findall(r'\b\w+\b', lower_text)
 
         for profanity in self._profanity_words:
             if ' ' in profanity:
                 self._find_profanity_phrase(profanity, lower_text, profanity_infos)
             else:
                 self._find_profanity_word(profanity, words, text, profanity_infos)
```

### Comparing `safetext-0.0.7/safetext/languages/de/words.txt` & `safetext-0.0.8/safetext/languages/de/words.txt`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/safetext/languages/en/words.txt` & `safetext-0.0.8/safetext/languages/en/words.txt`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/safetext/languages/es/words.txt` & `safetext-0.0.8/safetext/languages/es/words.txt`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/safetext/languages/pt/words.txt` & `safetext-0.0.8/safetext/languages/pt/words.txt`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/safetext/languages/tr/words.txt` & `safetext-0.0.8/safetext/languages/tr/words.txt`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/safetext/utils.py` & `safetext-0.0.8/safetext/utils.py`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/safetext.egg-info/PKG-INFO` & `safetext-0.0.8/safetext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetext
-Version: 0.0.7
+Version: 0.0.8
 Summary: Rule-based profanity checking tool for English and Turkish.
 Home-page: https://github.com/deepsafe/safetext
 Author: 
 License: MIT
 Keywords: text,profanity,filtering,turkish,english
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `safetext-0.0.7/setup.cfg` & `safetext-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `safetext-0.0.7/setup.py` & `safetext-0.0.8/setup.py`

 * *Files identical despite different names*

