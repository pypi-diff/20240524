# Comparing `tmp/corpusparser-0.0.1.tar.gz` & `tmp/corpusparser-0.0.2.tar.gz`

## Comparing `corpusparser-0.0.1.tar` & `corpusparser-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 corpusparser-0.0.1/sandbox.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 corpusparser-0.0.1/test_import_document.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 corpusparser-0.0.1/.vscode/launch.json
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 corpusparser-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 corpusparser-0.0.1/corpusparser/__init__.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 corpusparser-0.0.1/corpusparser/corpus.py
--rw-r--r--   0        0        0    21459 2020-02-02 00:00:00.000000 corpusparser-0.0.1/corpusparser/corpus_element.py
--rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 corpusparser-0.0.1/corpusparser/document.py
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 corpusparser-0.0.1/corpusparser/sentence.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 corpusparser-0.0.1/corpusparser/word.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 corpusparser-0.0.1/tests/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 corpusparser-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 corpusparser-0.0.1/tests/context.py
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 corpusparser-0.0.1/tests/test_corpusparser.py
--rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 corpusparser-0.0.1/tests/data/input.xml
--rw-r--r--   0        0        0    40215 2020-02-02 00:00:00.000000 corpusparser-0.0.1/tests/data/output.xml
--rw-r--r--   0        0        0     8945 2020-02-02 00:00:00.000000 corpusparser-0.0.1/tests/data/sents.txt
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 corpusparser-0.0.1/tests/data/stage1.xml
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 corpusparser-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 corpusparser-0.0.1/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 corpusparser-0.0.1/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 corpusparser-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 corpusparser-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 corpusparser-0.0.2/sandbox.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 corpusparser-0.0.2/test_import_document.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 corpusparser-0.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 corpusparser-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 corpusparser-0.0.2/corpusparser/__init__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 corpusparser-0.0.2/corpusparser/corpus.py
+-rw-r--r--   0        0        0    23235 2020-02-02 00:00:00.000000 corpusparser-0.0.2/corpusparser/corpus_element.py
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 corpusparser-0.0.2/corpusparser/document.py
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 corpusparser-0.0.2/corpusparser/sentence.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 corpusparser-0.0.2/corpusparser/word.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 corpusparser-0.0.2/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 corpusparser-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 corpusparser-0.0.2/tests/context.py
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 corpusparser-0.0.2/tests/test_corpusparser.py
+-rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 corpusparser-0.0.2/tests/data/input.xml
+-rw-r--r--   0        0        0    40215 2020-02-02 00:00:00.000000 corpusparser-0.0.2/tests/data/output.xml
+-rw-r--r--   0        0        0     8945 2020-02-02 00:00:00.000000 corpusparser-0.0.2/tests/data/sents.txt
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 corpusparser-0.0.2/tests/data/stage1.xml
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 corpusparser-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 corpusparser-0.0.2/LICENSE
+-rw-r--r--   0        0        0    12860 2020-02-02 00:00:00.000000 corpusparser-0.0.2/README.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 corpusparser-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13464 2020-02-02 00:00:00.000000 corpusparser-0.0.2/PKG-INFO
```

### Comparing `corpusparser-0.0.1/sandbox.py` & `corpusparser-0.0.2/sandbox.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,60 @@
 import xml.etree.ElementTree as ET
-from corpusparser.document import Document
-from corpusparser.sentence import Sentence
+import corpusparser
 
-filename = 'tests/data/input.xml'
+filename = 'tests/data/Melusine.xml'
 format = 'colmep'
-d = Document.create_from_nonstandard_file(filename, format)
-d.set_id('AYMON')
-# print(d.tag)
-d.transform_tokenise_sentences()
-# NB make sure to update spellings before adding text to sentences
-d.transform_remove_asterisks()
-d.transform_v_to_u()
-d.transform_u_to_v()
-d.transform_ye_caret_to_the()
-d.transform_add_convenience_text_to_sentences()
-d.transform_number_sentences()
-# d.transform_parse(add_parse_string=True, restructure=True, id=d.get_id())
-# d.transform_pos_tag(id=d.get_id())
-d.print_info()
+d = corpusparser.Document.create_from_nonstandard_file(filename, format)
+d.set_id('ARTHUR')
+
+print('Number of words: ', d.count_words())
+print('Most frequent words: ', d.word_frequency_no_punctuation().most_common(30))
+print('Most frequent punctuation: ', d.word_frequency_contains_punctuation().most_common(30))
+
+
+# # print(d.tag)
+d.transform_tokenise_sentences(tokenisation_model="period_and_capital")
+d.transform_common_spellings()
+d.update_spellings('ħ', 'h')
+d.update_spellings('þ', 'th')
+
+print('Number of words: ', d.count_words())
+print('Number of sentences: ', d.count_sentences())
+print('Longest sentence: ', d.longest_sentence_length())
+print('Shortest sentence: ', d.shortest_sentence_length())
+print('Average sentence length: ', d.average_sentence_length())
+
+print('Most frequent words: ', d.word_frequency_no_punctuation(correctedText=True).most_common(30))
+print('Most frequent punctuation: ', d.word_frequency_contains_punctuation(correctedText=True).most_common(30))
+print("XML tags: ", d.get_xml_tags())
+
+
+out_file = 'tests/data/Melusine-output.xml'
+d.to_xml_file(out_file, indent=2)
+
+sents = d.get_sentences_as_text_list(correctedText=True)
+sents_filename = "tests/data/Melusine-sentences.txt"
+try:
+    with open(sents_filename, 'w') as f:
+        for s in sents:
+            f.write(f"{s}\n")
+except IOError:
+    print("IOError: Could not write to file " + sents_filename)
+
+
+# # NB make sure to update spellings before adding text to sentences
+# d.transform_remove_asterisks()
+# d.transform_v_to_u()
+# d.transform_u_to_v()
+# d.transform_ye_caret_to_the()
+# d.transform_add_convenience_text_to_sentences()
+# d.transform_number_sentences()
+# # d.transform_parse(add_parse_string=True, restructure=True, id=d.get_id())
+# # d.transform_pos_tag(id=d.get_id())
+# d.print_info()
 
 # get sentences
 # sents = d.get_sentences()
 # s = sents[0]
 # s.parse(add_parse_string=True, restructure=True)
 # sents = d.get_sentences_as_text_list()
 # for s in sents:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `corpusparser-0.0.1/test_import_document.py` & `corpusparser-0.0.2/test_import_document.py`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/corpusparser/corpus_element.py` & `corpusparser-0.0.2/corpusparser/corpus_element.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,18 +168,24 @@
     # get sentence length - longest, shortest, average
     def get_sentence_lengths(self) -> list:
         sent_lengths = []
         for s in self.get_sentences_as_elements():
             sent_lengths.append(len(list(s.iter('w'))))
         return sent_lengths
     def longest_sentence_length(self) -> int:
+        if self.count_sentences() == 0:
+            return 0
         return max(self.get_sentence_lengths())
     def shortest_sentence_length(self) -> int:
+        if self.count_sentences() == 0:
+            return 0
         return min(self.get_sentence_lengths())
     def average_sentence_length(self) -> int:
+        if self.count_sentences() == 0:
+            return 0
         lengths = self.get_sentence_lengths()
         return round(sum(lengths) / len(lengths))
     
     # print some basic data about the element
     def print_info(self) -> None:
         print('Number of sentences: ', self.count_sentences())
         print('Number of words: ', self.count_words())
@@ -198,29 +204,29 @@
     # return a dictonary with the frequency of each word in the element
     def word_frequency(self, pattern='', correctedText=False) -> dict:
         words = self.get_words_as_text_list(correctedText)
         if pattern != '':
             words = [w.lower() for w in words if re.match(pattern, w)]
         return collections.Counter(words)
     
-    def word_frequency_starts_with(self, letter: str) -> dict:
+    def word_frequency_starts_with(self, letter: str, correctedText=False) -> dict:
         pattern = '[' + str.upper(letter) + str.lower(letter) + '].*'
-        return self.word_frequency(pattern)
+        return self.word_frequency(pattern, correctedText)
     
-    def word_frequency_contains(self, text: str) -> dict:
+    def word_frequency_contains(self, text: str, correctedText=False) -> dict:
         pattern = '.*' + text + '.*'
-        return self.word_frequency(pattern)
+        return self.word_frequency(pattern, correctedText)
     
-    def word_frequency_contains_punctuation(self) -> dict:
+    def word_frequency_contains_punctuation(self, correctedText=False) -> dict:
         pattern = '.*[^A-Za-z0-9].*'
-        return self.word_frequency(pattern)
+        return self.word_frequency(pattern, correctedText)
     
-    def word_frequency_no_punctuation(self) -> dict:
+    def word_frequency_no_punctuation(self, correctedText=False) -> dict:
         pattern = '.*[A-Za-z0-9].*'
-        return self.word_frequency(pattern)
+        return self.word_frequency(pattern, correctedText)
     
     # get list of XML tags used
     def get_xml_tags(self) -> list:
         tag_list = []
         for elem in self.iter():
             if elem.tag not in tag_list:
                 tag_list.append(elem.tag)
@@ -348,14 +354,18 @@
         for i in range(0, len(word_elem_list)):
 
             # choose the tokenisation model
             if tokenisation_model == 'period':
                 if _period_tokenisation_model(word_elem_list, i):
                     word_elem_list[i].set('sent-break', '1')
 
+            if tokenisation_model == 'period_and_pause':
+                if _period_and_pause_tokenisation_model(word_elem_list, i):
+                    word_elem_list[i].set('sent-break', '1')
+
             if tokenisation_model == 'period_and_capital':
                 if _period_and_capital_tokenisation_model(word_elem_list, i):
                     word_elem_list[i].set('sent-break', '1')
 
             # NB no other tokenisation models at present
 
         # the last word will always be a sentence break
@@ -428,21 +438,43 @@
 
     def transform_v_to_u(self) -> None:
         self.update_spellings_regex(match='v([bcdfghjklmnpqrstvwxz].*)', replace='u\\1')
 
     def transform_u_to_v(self) -> None:
         self.update_spellings_regex(match='(.*[aeiouy])u([aeiouy].*)', replace='\\1v\\2')
 
-    def transform_ye_caret_to_the(self) -> None:
+    def transform_carets(self) -> None:
+        # several spellings where a digraph is represented with carets
         self.update_spellings('y^e^', 'the')
         self.update_spellings('y^e', 'the')
+        self.update_spellings('y^t^', 'that')
+        self.update_spellings('w^t^', 'with')
 
     def transform_lbar_to_l(self) -> None:
         self.update_spellings('ƚ', 'l')
 
+    def transform_nasal_bars(self) -> None:
+        # several spellings where a nasalised vowel is represented with a bar
+        # most often this represents letter n, but it can also be m
+        # a separate spelling update can be applied before this, if this is the case
+        self.update_spellings('ā', 'an')
+        self.update_spellings('ē', 'en')
+        self.update_spellings('ī', 'in')
+        self.update_spellings('ō', 'on')
+        self.update_spellings('ū', 'un')
+
+    def transform_common_spellings(self) -> None:
+        # helper function which bundles common spelling updates together
+        self.transform_remove_asterisks()
+        self.transform_v_to_u()
+        self.transform_u_to_v()
+        self.transform_carets()
+        self.transform_lbar_to_l()
+        self.transform_nasal_bars()
+
                 
     def update_spellings(self, match: str, replace: str) -> None:
         # for each word, check if it matches the match pattern
         # if so, make corrections and add the updated orthography to the word as an attribute
         # if we have already made a change, use the value in the ortho attribute
         for w in self.iter('w'):
             if 'ortho' in w.attrib:
@@ -514,18 +546,26 @@
 
 # break sentences where there is a period
 def _period_tokenisation_model(word_list, index: int) -> bool:
     if word_list[index].text == '.':
         return True
     return False
 
+# break sentences where there is a period, or a colon or oblique
+def _period_and_pause_tokenisation_model(word_list, index: int) -> bool:
+    if word_list[index].text in ['.', ':', '/']:
+        return True
+    return False
+
 # break sentences where there is a period, or a colon or oblique which is followed immediatley by a capital letter
 def _period_and_capital_tokenisation_model(word_list, index: int) -> bool:
     if word_list[index].text == '.':
         return True
+    if index == len(word_list) - 1:
+        return True
     if word_list[index].text in [':', '/'] and word_list[index + 1].text[0].isupper():
         return True
     return False
 
 
 ##############################################################################
 # Utilities
```

### Comparing `corpusparser-0.0.1/corpusparser/document.py` & `corpusparser-0.0.2/corpusparser/document.py`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/corpusparser/sentence.py` & `corpusparser-0.0.2/corpusparser/sentence.py`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/corpusparser/word.py` & `corpusparser-0.0.2/corpusparser/word.py`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/tests/.DS_Store` & `corpusparser-0.0.2/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/tests/test_corpusparser.py` & `corpusparser-0.0.2/tests/test_corpusparser.py`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/tests/data/input.xml` & `corpusparser-0.0.2/tests/data/input.xml`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/tests/data/output.xml` & `corpusparser-0.0.2/tests/data/output.xml`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/tests/data/sents.txt` & `corpusparser-0.0.2/tests/data/sents.txt`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/tests/data/stage1.xml` & `corpusparser-0.0.2/tests/data/stage1.xml`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/.gitignore` & `corpusparser-0.0.2/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -157,8 +157,12 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # local files
 Aymon*.txt
-Aymon*.xml
+Aymon*.xml
+Arthur*.txt
+Arthur*.xml
+Melusine*.txt
+Melusine*.xml
```

### Comparing `corpusparser-0.0.1/LICENSE` & `corpusparser-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corpusparser-0.0.1/pyproject.toml` & `corpusparser-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "corpusparser"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ian Pattison", email="ianpattison2@gmail.com" },
 ]
 description = "Python library for importing and using corpus data in linguistic research"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

