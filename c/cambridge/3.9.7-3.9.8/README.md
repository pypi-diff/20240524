# Comparing `tmp/cambridge-3.9.7.tar.gz` & `tmp/cambridge-3.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cambridge-3.9.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cambridge-3.9.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cambridge-3.9.7.tar` & `cambridge-3.9.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       72 2024-03-03 06:01:31.364439 cambridge-3.9.7/.gitignore
--rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.000000 cambridge-3.9.7/LICENSE
--rw-r--r--   0        0        0     4122 2024-03-06 13:40:28.754758 cambridge-3.9.7/README.md
--rw-r--r--   0        0        0      266 2024-05-20 17:09:52.089277 cambridge-3.9.7/cambridge/__init__.py
--rw-r--r--   0        0        0     9591 2024-03-14 06:49:30.831288 cambridge-3.9.7/cambridge/args.py
--rw-r--r--   0        0        0     2306 2024-04-02 14:57:17.675678 cambridge-3.9.7/cambridge/cache.py
--rw-r--r--   0        0        0     1769 2024-03-05 14:25:39.637097 cambridge-3.9.7/cambridge/color.py
--rw-r--r--   0        0        0     3076 2024-05-20 15:35:19.125434 cambridge-3.9.7/cambridge/console.py
--rw-r--r--   0        0        0    18565 2024-03-14 06:49:30.832165 cambridge-3.9.7/cambridge/dicts/cambridge.py
--rw-r--r--   0        0        0     5591 2024-05-20 15:35:19.127425 cambridge-3.9.7/cambridge/dicts/dict.py
--rw-r--r--   0        0        0    47792 2024-05-20 17:09:52.092128 cambridge-3.9.7/cambridge/dicts/webster.py
--rw-r--r--   0        0        0      770 2024-03-11 05:51:25.317401 cambridge-3.9.7/cambridge/errors.py
--rw-r--r--   0        0        0      599 2024-03-05 14:25:39.642688 cambridge-3.9.7/cambridge/log.py
--rw-r--r--   0        0        0      682 2024-03-05 14:25:39.643531 cambridge-3.9.7/cambridge/main.py
--rw-r--r--   0        0        0     2561 2024-03-13 08:59:30.744980 cambridge-3.9.7/cambridge/utils.py
--rw-r--r--   0        0        0      731 2024-03-03 06:01:31.379053 cambridge-3.9.7/pyproject.toml
--rw-r--r--   0        0        0       45 2024-03-03 06:01:31.380018 cambridge-3.9.7/requirements.txt
--rw-r--r--   0        0        0   430578 2024-03-06 13:51:33.866712 cambridge-3.9.7/screenshots/cambridge.png
--rw-r--r--   0        0        0   338780 2023-08-21 11:28:38.010650 cambridge-3.9.7/screenshots/fzf.png
--rw-r--r--   0        0        0   228507 2023-11-10 15:57:56.401249 cambridge-3.9.7/screenshots/webster.png
--rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 cambridge-3.9.7/PKG-INFO
+-rw-r--r--   0        0        0       72 2024-03-03 06:01:31.364439 cambridge-3.9.8/.gitignore
+-rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.000000 cambridge-3.9.8/LICENSE
+-rw-r--r--   0        0        0     4122 2024-03-06 13:40:28.754758 cambridge-3.9.8/README.md
+-rw-r--r--   0        0        0      266 2024-05-24 04:32:32.406246 cambridge-3.9.8/cambridge/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-24 04:12:20.868957 cambridge-3.9.8/cambridge/args.py
+-rw-r--r--   0        0        0     2306 2024-04-02 14:57:17.675678 cambridge-3.9.8/cambridge/cache.py
+-rw-r--r--   0        0        0     1769 2024-05-23 14:16:50.775853 cambridge-3.9.8/cambridge/color.py
+-rw-r--r--   0        0        0     3159 2024-05-24 02:25:10.074112 cambridge-3.9.8/cambridge/console.py
+-rw-r--r--   0        0        0    18593 2024-05-24 02:25:10.076072 cambridge-3.9.8/cambridge/dicts/cambridge.py
+-rw-r--r--   0        0        0     5597 2024-05-24 02:25:10.077496 cambridge-3.9.8/cambridge/dicts/dict.py
+-rw-r--r--   0        0        0    44386 2024-05-24 04:32:32.407192 cambridge-3.9.8/cambridge/dicts/webster.py
+-rw-r--r--   0        0        0      770 2024-03-11 05:51:25.317401 cambridge-3.9.8/cambridge/errors.py
+-rw-r--r--   0        0        0      599 2024-03-05 14:25:39.642688 cambridge-3.9.8/cambridge/log.py
+-rw-r--r--   0        0        0      682 2024-03-05 14:25:39.643531 cambridge-3.9.8/cambridge/main.py
+-rw-r--r--   0        0        0     2561 2024-03-13 08:59:30.744980 cambridge-3.9.8/cambridge/utils.py
+-rw-r--r--   0        0        0      731 2024-03-03 06:01:31.379053 cambridge-3.9.8/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-03-03 06:01:31.380018 cambridge-3.9.8/requirements.txt
+-rw-r--r--   0        0        0   430578 2024-03-06 13:51:33.866712 cambridge-3.9.8/screenshots/cambridge.png
+-rw-r--r--   0        0        0   338780 2023-08-21 11:28:38.010650 cambridge-3.9.8/screenshots/fzf.png
+-rw-r--r--   0        0        0   228507 2023-11-10 15:57:56.401249 cambridge-3.9.8/screenshots/webster.png
+-rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 cambridge-3.9.8/PKG-INFO
```

### Comparing `cambridge-3.9.7/LICENSE` & `cambridge-3.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/README.md` & `cambridge-3.9.8/README.md`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/cambridge/args.py` & `cambridge-3.9.8/cambridge/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,43 +209,19 @@
 
 
 def list_words(args, con, cur):
     # The subparser i.e. the sub-command isn't in the namespace of args
 
     if args.delete:
         to_delete = args.delete
-
-        ids = []
-        words = []
-
-        for index, item in enumerate(to_delete):
-            # multiple words/phrases are seperated by ","
-            if "," in item or ("," not in item and index == len(to_delete) - 1):
-                ids.append(index)
-
-        # if there is only one word/phrase to delete
-        if len(ids) == 1:
-            word = " ".join(to_delete).strip().strip(",")
-            delete(word, con, cur)
-
-        # if there are multiple words/phrase to delete
-        else:
-            for i, id in enumerate(ids):
-                if i == 0:
-                    words.append(" ".join(to_delete[: (id + 1)]).strip(",").strip())
-                if i > 0:
-                    words.append(" ".join(to_delete[(ids[i-1] + 1): (id + 1)]).strip(",").strip())
-
-            # If the last word in `to_delete` variable does not end with ",", it should be collected.
-            # Else the last word ends with ",", it has been covered and handled above.
-            if ids[-1] != len(to_delete) - 1:
-                words.append(to_delete[-1])
-
-            for word in words:
-                delete(word, con, cur)
+        words = " ".join(to_delete)
+        for w in words.split(","):
+            i = w.strip()
+            if i:
+                delete(i, con, cur)
 
     elif args.random:
         try:
             data = get_random_words(cur)
         except sqlite3.OperationalError:
             logger.error("You may haven't searched any word yet")
         else:
```

### Comparing `cambridge-3.9.7/cambridge/cache.py` & `cambridge-3.9.8/cambridge/cache.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/cambridge/color.py` & `cambridge-3.9.8/cambridge/color.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/cambridge/console.py` & `cambridge-3.9.8/cambridge/console.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,34 +65,39 @@
 
         if s not in Symbol.values():
             after_parse += s
             i = i + 1
         elif s == Symbol["SLASH"] and string[i - 1] != Symbol["L_BRACKET"]:
             after_parse += s
             i = i + 1
-        else:
-            if s == Symbol["L_BRACKET"]:
+        elif s == Symbol["HASH"] and string[i + 1] != Symbol["L_BRACKET"]:
+            after_parse += s
+            i = i + 1
+        elif s == Symbol["HASH"] and string[i + 1] == Symbol["L_BRACKET"]:
+            i = i + 1
+        elif s == Symbol["L_BRACKET"] and string[i - 1] == Symbol["HASH"]:
                 k = i
                 for j, ss in enumerate(string[i + 1 : ]):
                     k += 1
                     if ss == Symbol["R_BRACKET"]:
                         text_in_bracket = string[i + 1 : i + 1 + j]
                         for word in text_in_bracket.split():
-                            # for normal [], not for color syntax
-                            if word.isalpha() and word.upper() not in COLOR_EFFECT.keys():
-                                after_parse += string[i : i + 1 + j + 1]
-                                i = k
-                                break
-                            else:
-                                after_parse += parse_in_bracket(string[i + 1 : i + 1 + j])
-                                i = k
-                                break
+                            after_parse += parse_in_bracket(string[i + 1 : i + 1 + j])
+                            i = k
+                            break
                         break
                 i = i + 1
 
+        elif s == Symbol["L_BRACKET"] and string[i - 1] != Symbol["HASH"]:
+            after_parse += s
+            i = i + 1
+        else:
+            after_parse += s
+            i = i + 1
+
     return after_parse + get_color_effect("RESET")
 
 
 def c_print(*objects, sep=' ', end='\n', file=None, flush=False, justify: Optional[JustifyMethod] = None):
     if not objects:
         objects = ("\n",)
```

### Comparing `cambridge-3.9.7/cambridge/dicts/cambridge.py` & `cambridge-3.9.8/cambridge/dicts/cambridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     return w_type
 
 
 def print_pron(block, area):
     w_pron = block.find("span", "pron dpron")
     if w_pron is not None:
         w_pron_text = replace_all(w_pron.text).replace("/", "|")
-        c_print(f"[bold]{area} [/bold]" + w_pron_text, end=" ")
+        c_print(f"#[bold]{area} #[/bold]" + w_pron_text, end=" ")
 
 
 def parse_head_pron(head):
     uk_dpron = head.find("span", "uk dpron-i")
     if uk_dpron is not None:
         print_pron(uk_dpron, "UK")
 
@@ -232,15 +232,15 @@
 def parse_head_tense(block):
     sub_blocks = block.find_all("span", "inf-group dinfg")
     if len(sub_blocks) != 0:
         for index, sub in enumerate(sub_blocks):
             tenses = sub.find_all("b", "inf dinf")
             if len(tenses) != 0:
                 for tense in tenses:
-                    c_print("[bold]" + tense.text + "[/bold]", end=" ")
+                    c_print("#[bold]" + tense.text + "#[/bold]", end=" ")
             if index == 0 and len(sub_blocks) > 1:
                 print("|", end=" ")
 
 
 def parse_head_domain(block):
     domain = replace_all(block.text)
     print(domain, end="  ")
@@ -272,15 +272,15 @@
     if head is not None:
         w_type = parse_head_type(head)
 
         if not word:
             word = parse_head_title(head)
         if w_type:
             w_type = w_type.replace(" or ", "/")
-            c_print(f"\n[bold blue]{word}[/bold blue] [bold yellow]{w_type}[/bold yellow]")
+            c_print(f"\n#[bold blue]{word}#[/bold blue] #[bold yellow]{w_type}#[/bold yellow]")
 
         parse_head_pron(head)
 
         irreg = head.find("span", "irreg-infls dinfls")
         if irreg is not None:
             parse_head_tense(irreg)
 
@@ -293,23 +293,23 @@
         spellvar = head.find_all("span", "spellvar dspellvar")
         if len(spellvar) != 0:
             parse_head_spellvar(spellvar)
 
         print()
 
     else:
-        c_print("[bold blue]" + word)
+        c_print("#[bold blue]" + word)
         if info:
             print(f"{info[0]} {info[1]}")
 
 
 # ----------Parse Dict Body----------
 def parse_def_title(block):
     d_title = replace_all(block.find("h3", "dsense_h").text)
-    c_print("[red]" + "\n" + d_title.upper())
+    c_print("#[red]" + "\n" + d_title.upper())
 
 def parse_ptitle(block):
     p_title = block.find("span", "phrase-title dphrase-title").text
     p_info = block.find("span", "phrase-info dphrase-info")
 
     if p_info is not None:
         phrase_info = replace_all(p_info.text)
@@ -392,35 +392,35 @@
 
         example_lan = e.find("span", "trans dtrans dtrans-se hdb break-cj")
         if example_lan is not None:
             example_lan_sent = " " + example_lan.text.replace("。", "")
         else:
             example_lan_sent = ""
 
-        c_print("[blue]" + "|" + "[/blue]", end="")
+        c_print("#[blue]" + "|" + "#[/blue]", end="")
 
         dlab = e.find("span", "lab dlab")
         print_example_tag(dlab)
 
         dgram = e.find("span", "gram dgram")
         print_example_tag(dgram)
 
         dlu = e.find("span", "lu dlu")
         print_example_tag(dlu)
 
-        c_print(f"[#757575]{example}{example_lan_sent}[/#757575]")
+        c_print(f"#[#757575]{example}{example_lan_sent}#[/#757575]")
 
 
 def print_synonym(block):
     s_title = block.strong.text.upper()
-    c_print("[bold #757575]" + "\n  " + s_title)
+    c_print("#[bold #757575]" + "\n  " + s_title)
 
     for s in block.find_all("div", ["item lc lc1 lpb-10 lpr-10", "item lc lc1 lc-xs6-12 lpb-10 lpr-10"]):
         s = s.text
-        c_print("[#757575]" + "  • " + s)
+        c_print("#[#757575]" + "  • " + s)
 
     print()
 
 
 def parse_synonym(block):
     s_block = block.find("div", re.compile("xref synonyms? hax dxref-w( lmt-25)?"))
     if s_block is not None:
@@ -430,52 +430,52 @@
 
 
 def parse_see_also(def_block):
     see_also_block = def_block.find("div", re.compile("xref see_also hax dxref-w( lmt-25)?"))
 
     if see_also_block is not None:
         see_also = see_also_block.strong.text.upper()
-        c_print("[bold #757575]" + "\n  " + see_also)
+        c_print("#[bold #757575]" + "\n  " + see_also)
 
         for item in see_also_block.find_all("span", ["x-h dx-h", "x-p dx-p"]):
-            c_print("[#757575]" + "  • " + item.text, end=" ")
+            c_print("#[#757575]" + "  • " + item.text, end=" ")
             next_sibling = item.find_next_sibling("span")
             if next_sibling is not None:
                 print(next_sibling.text)
             else:
                 print()
 
 
 def parse_compare(def_block):
     compare_block = def_block.find("div", re.compile("xref compare hax dxref-w( lmt-25)?"))
 
     if compare_block is not None:
         compare = compare_block.strong.text.upper()
-        c_print("[bold #757575]" + "\n  " + compare)
+        c_print("#[bold #757575]" + "\n  " + compare)
         for word in compare_block.find_all("div", ["item lc lc1 lpb-10 lpr-10", "item lc lc1 lc-xs6-12 lpb-10 lpr-10"]):
             item = word.a.text
-            c_print("[#757575]" + "  • " + item + "[/#757575]", end="")
+            c_print("#[#757575]" + "  • " + item + "#[/#757575]", end="")
 
             usage = word.find("span", "x-lab dx-lab")
             if usage:
                 usage = usage.text
                 print(usage, end="")
 
             print()
 
 
 def parse_usage_note(def_block):
     usage_block = def_block.find("div", "usagenote dusagenote daccord")
 
     if usage_block is not None:
         usagenote = usage_block.h5.text
-        c_print("[bold #757575]" + "\n  " + usagenote)
+        c_print("#[bold #757575]" + "\n  " + usagenote)
         for item in usage_block.find_all("li", "text"):
             item = item.text
-            c_print("[#757575]" + "    " + item)
+            c_print("#[#757575]" + "    " + item)
 
 
 def parse_def(def_block):
     if "phrase-body" in def_block.parent.attrs["class"]:
         parse_meaning(def_block, True)
         parse_example(def_block, True)
     else:
@@ -488,18 +488,18 @@
     parse_usage_note(def_block)
 
 def parse_idiom(block):
     idiom_block = block.find("div", re.compile("xref idioms? hax dxref-w lmt-25 lmb-25"))
 
     if idiom_block is not None:
         idiom_title = idiom_block.h3.text.upper()
-        c_print("[bold #757575]" + "\n" + idiom_title)
+        c_print("#[bold #757575]" + "\n" + idiom_title)
         for idiom in idiom_block.find_all("div", ["item lc lc1 lpb-10 lpr-10", "item lc lc1 lc-xs6-12 lpb-10 lpr-10"]):
             idiom = idiom.text
-            c_print("[#757575]" + "  • " + idiom)
+            c_print("#[#757575]" + "  • " + idiom)
 
 
 def parse_sole_idiom(block):
     idiom_sole_meaning = block.find("div", "def ddef_d db")
 
     if idiom_sole_meaning is not None:
         print("\033[34m" + idiom_sole_meaning.text + "\033[0m")
@@ -508,18 +508,18 @@
 
 
 def parse_phrasal_verb(block):
     pv_block = block.find("div", re.compile("xref phrasal_verbs? hax dxref-w lmt-25 lmb-25"))
 
     if pv_block is not None:
         pv_title = pv_block.h3.text.upper()
-        c_print("[bold #757575]" + "\n" + pv_title)
+        c_print("#[bold #757575]" + "\n" + pv_title)
         for pv in pv_block.find_all("div", ["item lc lc1 lc-xs6-12 lpb-10 lpr-10", "item lc lc1 lpb-10 lpr-10"]):
             pv = pv.text
-            c_print("[#757575]" + "  • " + pv)
+            c_print("#[#757575]" + "  • " + pv)
 
 
 def parse_dict_body(block):
     subblocks = block.find_all("div", ["pr dsense", "pr dsense dsense-noh"])
 
     if len(subblocks) != 0:
         for subblock in subblocks:
@@ -559,8 +559,8 @@
 def parse_dict_name(first_dict):
     if first_dict.small is not None:
         dict_info = replace_all(first_dict.small.text).strip("(").strip(")")
         dict_name = dict_info.split("©")[0]
         dict_name = dict_name.split("the")[-1]
     else:
         dict_name="Cambridge Dictionary"
-    c_print(f"[#757575]{dict_name}", justify="right")
+    c_print(f"#[#757575]{dict_name}", justify="right")
```

### Comparing `cambridge-3.9.7/cambridge/dicts/dict.py` & `cambridge-3.9.8/cambridge/dicts/dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,19 +69,19 @@
 
     res_url, res_word, res_text = data
 
     if DICT.CAMBRIDGE.name.lower() in res_url:
         logger.debug(f"{OP.PARSING.name} {res_url}")
         soup = make_a_soup(res_text)
         cambridge.parse_and_print(soup, res_url)
-        c_print(f'\n[#757575]{OP.FOUND.name} "{res_word}" from {dict} in cache. You can add "-f -w" to fetch the {DICT.MERRIAM_WEBSTER.name} dictionary', justify="left")
+        c_print(f'\n#[#757575]{OP.FOUND.name} "{res_word}" from {dict} in cache. You can add "-f -w" to fetch the {DICT.MERRIAM_WEBSTER.name} dictionary', justify="left")
     else:
         nodes = webster.parse_dict(res_text, True, res_url, False)
         webster.parse_and_print(nodes, res_url)
-        c_print(f'\n[#757575]{OP.FOUND.name} "{res_word}" from {dict} in cache. You can add "-f" to fetch the {DICT.CAMBRIDGE.name} dictionary', justify="left")
+        c_print(f'\n#[#757575]{OP.FOUND.name} "{res_word}" from {dict} in cache. You can add "-f" to fetch the {DICT.CAMBRIDGE.name} dictionary', justify="left")
     return True
 
 
 def save(con, cur, input_word, response_word, response_url, response_text):
     """Save a word info into local DB for cache."""
 
     try:
@@ -105,21 +105,21 @@
         logger.debug(f'{OP.CACHED.name} the search result of "{input_word}"')
 
 #TODO add an option for inputing a new word
 def print_spellcheck(con, cur, input_word, suggestions, dict, is_ch=False):
     """Parse and print spellcheck info."""
 
     for count, sug in enumerate(suggestions):
-        c_print("[bold]%2d" % (count+1), end="")
+        c_print("#[bold]%2d" % (count+1), end="")
         if dict == DICT.MERRIAM_WEBSTER.name:
-            c_print("[#4A7D95] %s" % sug)
+            c_print("#[#4A7D95] %s" % sug)
         else:
             print("\033[34m" + " " + sug + "\033[0m")
 
-    c_print(f"Press [NUMBER] to look up the suggestion inferred from the unfound [red]{input_word}[/red], [ENTER] to toggle dictionary, or [ANY OTHER KEY] to exit: ", end="")
+    c_print(f"Press [NUMBER] to look up the suggestion inferred from the unfound #[red]{input_word}#[/red], [ENTER] to toggle dictionary, or [ANY OTHER KEY] to exit: ", end="")
     key = input("")
     if key.isnumeric() and (1 <= int(key) <= len(suggestions)):
         if dict == DICT.MERRIAM_WEBSTER.name:
             webster.search_webster(con, cur, suggestions[int(key) - 1])
         if dict == DICT.CAMBRIDGE.name:
            cambridge.search_cambridge(con, cur, suggestions[int(key) - 1], False, is_ch)
     elif key == "":
```

### Comparing `cambridge-3.9.7/cambridge/dicts/webster.py` & `cambridge-3.9.8/cambridge/dicts/webster.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 sub_text = ""
 res_word = ""
 word_entries = [] # A page may have multiple word entries, e.g. "give away", "giveaway"
 word_forms = []   # A word may have multiple word forms, e.g. "ran", "running", "run", "flies"
 word_types = []   # A word's word types, e.g. "preposition", "adjective"
 
 
-# TODO examples and definiations word wrap
-# TODO fzf integration
-
 def search_webster(con, cur, input_word, is_fresh=False, no_suggestions=False):
     """
     Entry point for searching a word in Webster.
     It first checks the cache, if the word has been cached,
     uses it and prints it; if not, go fetch the web.
     If the word is found, prints it to the terminal and caches it concurrently.
     if not found, prints word suggestions and exit.
@@ -121,36 +118,38 @@
         res_url, res_text = result[1]
         parse_and_print_wod(res_url, res_text)
 
 
 def parse_redirect(nodes, res_url):
     input_word = decode_url(res_url).split("/")[-1]
     print("No exact result found.")
-    c_print(f"The following entries include the term [#b22222 bold]{input_word}[/#b22222 bold].")
+    c_print(f"The following entries include the term #[#b22222 bold]{input_word}#[/#b22222 bold].")
 
     for node in nodes:
         try:
             attr = node.attrib["id"]
         except KeyError:
             attr = node.attrib["class"]
 
         if "row entry-header" in attr:
             print()
             row_entry_header(node, True)
+            continue
 
         if "-entry" in attr:
             print()
             for n in node.iterchildren():
                 if n.tag == "div" and n.attrib["class"] == "vg":
                     for child in n.iterchildren():
                         if child.tag == "p":
                             x = list(child.itertext())
                             print("".join(x).strip())
+            continue
 
-    c_print(f'\n[#757575]You can add "camb -w" before one above entry to get its full definition from the {DICT.MERRIAM_WEBSTER.name} dictionary')
+    c_print(f'\n#[#757575]You can add "camb -w" before one above entry to get its full definition from the {DICT.MERRIAM_WEBSTER.name} dictionary')
 
 
 def parse_dict(res_text, found, res_url, is_fresh):
     """Parse the dict section of the page for the word."""
 
     logger.debug(f"{OP.PARSING.name} {res_url}")
 
@@ -225,25 +224,29 @@
             has_word = (elm.tag == "span") and (elm.attrib["class"] == "b-link hw-text fw-bold")
             has_nearby = (elm.tag == "a") and (elm.attrib["class"] == "b-link")
             has_em = (elm.tag == "em")
         except KeyError:
             continue
         else:
             if has_title:
-                c_print(f"[bold {w_col.nearby_title}]{elm.text}", end="")
+                c_print(f"#[bold {w_col.nearby_title}]{elm.text}", end="")
+                continue
 
             if has_em:
                 word = "".join(list(elm.itertext()))
-                c_print(f"[bold {w_col.nearby_em}]{word}", end="\n")
+                c_print(f"#[bold {w_col.nearby_em}]{word}", end="\n")
+                continue
 
             if has_word:
-                c_print(f"[{w_col.nearby_word}]{elm.text}", end="\n")
+                c_print(f"#[{w_col.nearby_word}]{elm.text}", end="\n")
+                continue
 
             if has_nearby:
-                c_print(f"[{w_col.nearby_item}]{elm.text}", end="\n")
+                c_print(f"#[{w_col.nearby_item}]{elm.text}", end="\n")
+                continue
 
 
 ###########################################
 # parse and print synonyms
 ###########################################
 
 def synonyms(node):
@@ -254,29 +257,29 @@
             has_title = (elm.tag == "h2") # "Synonyms"
             has_label = (elm.tag == "p") and (elm.attrib["class"] == "function-label") # "Noun"
             has_syn = (elm.tag == "ul") # synonym list
         except KeyError:
             continue
         else:
             if has_title:
-                c_print(f"[bold {w_col.syn_title}]{elm.text}", end=" ")
+                c_print(f"#[bold {w_col.syn_title}]{elm.text}", end=" ")
 
             if has_label:
-                c_print(f"\n[{w_col.syn_label}]{elm.text}")
+                c_print(f"\n#[{w_col.syn_label}]{elm.text}")
 
             if has_syn:
                 children = elm.getchildren()
                 total_num = len(children)
 
                 for index, child in enumerate(children):
                     syn = "".join(list(child.itertext())).strip()
                     if index != (total_num - 1):
-                        c_print(f"[{w_col.syn_item}]{syn},", end=" ")
+                        c_print(f"#[{w_col.syn_item}]{syn},", end=" ")
                     else:
-                        c_print(f"[{w_col.syn_item}]{syn}", end=" ")
+                        c_print(f"#[{w_col.syn_item}]{syn}", end=" ")
 
 
 ###########################################
 # parse and print examples
 ###########################################
 
 # NOTE:
@@ -289,23 +292,23 @@
         try:
             is_title = ("ex-header function-label" in elm.attrib["class"]) # Recent Examples on the Web
             has_aq = (elm.attrib["class"] == "t has-aq")
         except KeyError:
             continue
         else:
             if is_title:
-                c_print(f"\n[{w_col.eg_title} bold]{elm.text}", end="")
+                c_print(f"\n#[{w_col.eg_title} bold]{elm.text}", end="")
             if has_aq:
                 texts = list(elm.itertext())
 
                 for index, t in enumerate(texts):
                     if time in [0, 1, 8, 9, 16, 17, 24, 25]:
                         if index == 0:
-                            c_print(f"\n[{w_col.accessory}]|", end="")
-                            c_print(f"[{w_col.eg_sentence}]{t}", end="")
+                            c_print(f"\n#[{w_col.accessory}]|", end="")
+                            c_print(f"#[{w_col.eg_sentence}]{t}", end="")
                         else:
                             hit = False
                             global word_entries, word_forms
                             words = set(word_entries)
                             forms = set(word_forms)
                             text = t.strip().lower()
                             for w in words:
@@ -319,20 +322,17 @@
                                         break
                             for f in forms:
                                 if f == text:
                                     hit = True
                                     break
 
                             if hit:
-                                c_print(f"[{w_col.eg_sentence} bold]{t}", end="")
+                                c_print(f"#[{w_col.eg_sentence} bold]{t}", end="")
                             else:
-                                # FIXME This is a temp solution to embedded "[[]]" e.g "Only Chloe sense its [clears throat] presence"
-                                # Within [], there is also [#xxxxxx bold] to colorize "clears", which is the searched word needing highlighting.
-                                t = t.replace("[", "").replace("]", "")
-                                c_print(f"[{w_col.eg_sentence}]{t}", end="")
+                                c_print(f"#[{w_col.eg_sentence}]{t}", end="")
                     else:
                         continue
                 time = time + 1
 
 
 ###########################################
 # parse and print phrases
@@ -342,27 +342,27 @@
     print()
 
     children = node.getchildren()[1]
     for child in children:
         try:
             if child.attrib["class"] == "drp":
                 if child.getnext().tag == "span":
-                    c_print(f"[{w_col.ph_item} bold]{child.text}", end = "")
+                    c_print(f"#[{w_col.ph_item} bold]{child.text}", end = "")
                 else:
-                    c_print(f"[{w_col.ph_item} bold]{child.text}", end = "\n")
+                    c_print(f"#[{w_col.ph_item} bold]{child.text}", end = "\n")
 
             if child.attrib["class"] == "vg":
                 vg(child)
 
         except KeyError:
             for i in child.getchildren():
                 if i.attrib["class"] == "vl":
                     print_or_badge(i.text)
                 else:
-                    c_print(f"[{w_col.ph_item} bold]{i.text}", end = "\n")
+                    c_print(f"#[{w_col.ph_item} bold]{i.text}", end = "\n")
 
 
 ##########################################################
 # parse and print related phrases (Phrases Containing ...)
 ##########################################################
 
 def related_phrases(node):
@@ -374,31 +374,31 @@
     texts = list(title.itertext())
     global word_entries
     words = set(word_entries)
 
     for t in texts:
         if t.strip():
             if t.lower() in words:
-                c_print(f"[{w_col.rph_em} bold]{t}", end="\n")
+                c_print(f"#[{w_col.rph_em} bold]{t}", end="\n")
             else:
-                c_print(f"[{w_col.rph_title} bold]{t}", end="")
+                c_print(f"#[{w_col.rph_title} bold]{t}", end="")
 
     pr_sec = children[2]
     phrases = [] # li tags, each tag has one phrase
     for i in pr_sec.iterdescendants():
         if i.tag == "li":
             phrases.append(i)
 
     for phrase in phrases:
         ts = list(phrase.itertext())
         ts = "". join(ts).strip("\n").strip()
         if phrase != phrases[-1]:
-            c_print(f"[{w_col.rph_item}]{ts},", end=" ")
+            c_print(f"#[{w_col.rph_item}]{ts},", end=" ")
         else:
-            c_print(f"[{w_col.rph_item}]{ts}", end="")
+            c_print(f"#[{w_col.rph_item}]{ts}", end="")
 
 
 ###########################################
 # parse and print dictionary-entry-[number]
 ###########################################
 
 # --- parse class "vg" --- #
@@ -410,22 +410,23 @@
         if attr is not None:
             if "lowercase" in attr:
                 l_words.append(i.text)
             if "uppercase" in attr:
                 u_words.append(i.text)
     return l_words, u_words
 
-def dtText(node, ancestor_attr, count, root_attr=""):
+def dtText(node, ancestor_attr):
     texts = list(node.itertext())
-    if count != 1:
-        format_basedon_ancestor(ancestor_attr, prefix="\n", root_attr=root_attr)
 
     l_words = get_word_cases(node)[0]
     u_words = get_word_cases(node)[1]
 
+    if node.getprevious() is not None and node.getprevious().get("class") == "sub-content-thread":
+        format_basedon_ancestor(ancestor_attr, prefix="\n")
+
     for index, text in enumerate(texts):
         if text == " " and index == 0:
             continue
         if text == ": ":
             print_meaning_content(text, end="")
         elif text == " see also ":
             print_meaning_keyword(text.strip())
@@ -442,87 +443,88 @@
 
     print("", end = " ")
 
 
 def print_mw(text, has_tail, tag):
     if tag == "hl":
         if has_tail is True:
-            c_print(f"[{w_col.meaning_sentence} bold]{text}", end = "")
+            c_print(f"#[{w_col.meaning_sentence} bold]{text}", end = "")
         else:
-            c_print(f"[{w_col.meaning_sentence} bold]{text}", end = " ")
+            c_print(f"#[{w_col.meaning_sentence} bold]{text}", end = " ")
     if tag == "normal":
         if has_tail is True:
-            c_print(f"[{w_col.meaning_sentence}]{text}", end = "")
+            c_print(f"#[{w_col.meaning_sentence}]{text}", end = "")
         else:
-            c_print(f"[{w_col.meaning_sentence}]{text}", end = " ")
+            c_print(f"#[{w_col.meaning_sentence}]{text}", end = " ")
 
 
-def ex_sent(node, ancestor_attr, root_attr="", num_label_count=1):
+def ex_sent(node, ancestor_attr, num_label_count=1):
     if ancestor_attr:
-        format_basedon_ancestor(ancestor_attr, prefix="\n", root_attr=root_attr)
+        format_basedon_ancestor(ancestor_attr, prefix="\n")
     else:
         print("")
 
     if num_label_count == 2:
         print(" ", end="")
 
-    c_print(f"[{w_col.accessory}]|", end="")
+    c_print(f"#[{w_col.accessory}]|", end="")
 
     hl_words = []
     ems = []
     for i in node.iterdescendants():
         attr = i.get("class")
         if attr is not None:
             if i.tag == "em" and "mw" in attr:
                 ems.append(i.text)
+                continue
             if i.tag == "span" and "mw" in attr:
                 hl_words.append(i.text)
+                continue
 
     texts = list(node.itertext())
     count = len(texts)
 
-    # TODO: Here needs a better logic, compliant with both normal words and words as prefixs and suffixs like 'in'.
     for index, t in enumerate(texts):
         text = t.strip("\n").strip()
         if text:
             if t in hl_words:
-                hl_has_tail = ((index != (count - 1)) and (texts[index + 1].strip("\n").strip()) and (not texts[index + 1].strip("\n").strip()[0].isalpha()))
+                hl_has_tail = ((index != (count - 1)) and (texts[index + 1].strip("\n").strip()) and (not texts[index + 1].strip("\n").strip()[0].isalnum()))
                 print_mw(text, hl_has_tail, "hl")
             elif t in ems:
                 if index != 0 and texts[index - 1].endswith(" "):
                     print("", end = " ")
-                c_print(f"[{w_col.meaning_sentence} bold]{text}", end = "")
+                c_print(f"#[{w_col.meaning_sentence} bold]{text}", end = "")
                 if index != (count - 1) and texts[index + 1].startswith(" "):
                     print("", end = " ")
             else:
                 normal_has_tail = (index != (count - 1) and (texts[index + 1] in ems))
                 print_mw(text, normal_has_tail, "normal")
 
 
-def sub_content_thread(node, ancestor_attr, root_attr="", num_label_count=1):
+def sub_content_thread(node, ancestor_attr, num_label_count=1):
     children = node.getchildren()
     for child in children:
         attr = child.attrib["class"]
 
         if ("ex-sent" in attr) and ("aq has-aq" not in attr):
-            ex_sent(child, ancestor_attr, root_attr, num_label_count)
+            ex_sent(child, ancestor_attr, num_label_count)
+            continue
 
         if "vis" in attr:
             elms = child.getchildren()
             for e in elms:
                 elm = e.getchildren()[0]
                 elm_attr = elm.attrib["class"]
                 if ("ex-sent" in elm_attr) and ("aq has-aq" not in elm_attr):
-                    ex_sent(elm, ancestor_attr, root_attr, num_label_count)
+                    ex_sent(elm, ancestor_attr, num_label_count)
+            continue
 
 
-def extra(node, ancestor_attr, count, root_attr=""):
+def extra(node, ancestor_attr):
     texts = list(node.itertext())
-    if count != 1:
-        format_basedon_ancestor(ancestor_attr, prefix="\n", root_attr=root_attr)
 
     l_words = get_word_cases(node)[0]
     u_words = get_word_cases(node)[1]
 
     for text in texts:
         text_new = text.strip("\n").strip()
         if text_new:
@@ -538,106 +540,30 @@
                 print_meaning_content(text_new, end=" ")
             else:
                 print_meaning_content(text_new, end="")
 
     print("", end = " ")
 
 
-def vi(node, ancestor_attr, root_attr, num_label_count=1):
-    children = node.getchildren()
-    for child in children:
-        child_attr = child.get("class")
-        if child_attr == "sub-content-thread":
-            sub_content_thread(child, ancestor_attr, root_attr, num_label_count)
-
+def unText_simple(node, ancestor_attr, num_label_count=1, has_badge=True):
+    text = "".join(list(node.itertext())).strip()
 
-def uns(node, ancestor_attr, root_attr, num_label_count=1):
-    node_pre = node.getprevious()
-    if node_pre is not None and node_pre.get("class") == "sub-content-thread":
+    if not has_badge:
         print()
+        if num_label_count == 2:
+            print(" ", end="")
+        format_basedon_ancestor(ancestor_attr, prefix="")
 
-    # elms = node.getchildren()[0].getchildren()
-    for child in node.iterchildren():
-        child_attr = child.get("class")
-
-        if child_attr == "un":
-            elms = child.getchildren()
-            for elm in elms:
-                elm_attr = elm.get("class")
-                if elm_attr == "unText":
-                    if num_label_count == 2:
-                        print(" ", end="")
-
-                    text = "".join(list(elm.itertext())).strip()
-                    if "mdash" in elm.getprevious().attrib["class"]:
-                        if node_pre is not None and node_pre.get("class") == "sub-content-thread":
-                            format_basedon_ancestor(ancestor_attr, prefix="", root_attr=root_attr)
-                        print_meaning_arrow("->" + text)
-                    else:
-                        format_basedon_ancestor(ancestor_attr, prefix="", root_attr=root_attr)
-                        print_meaning_badge(text)
-
-                if elm_attr == "sub-content-thread":
-                    sub_content_thread(elm, ancestor_attr, root_attr, num_label_count)
-
-                if elm_attr == "vi":
-                    vi(elm, ancestor_attr, root_attr, num_label_count)
-
-        if child_attr == "unText":
-            unText_simple(child, ancestor_attr, ancestor_attr, num_label_count)
-
-        if child_attr == "vi":
-            format_basedon_ancestor(ancestor_attr, prefix="", root_attr=root_attr)
-            vi(child, ancestor_attr, root_attr, num_label_count)
-
-
-def unText_simple(node, ancestor_attr, root_attr, num_label_count=1):
     node_pre = node.getprevious()
-    if node_pre is not None and (node_pre.get("class") == "un" or node_pre.get("class") == "uns"):
-        print()
-
-    if num_label_count == 2:
-        print(" ", end="")
-
-    text = list(node.itertext())
-    format_basedon_ancestor(ancestor_attr, prefix="", root_attr=root_attr)
-    for t in text:
-        print_meaning_content(t, end="")
-
-
-def dt(node, ancestor_attr, self_attr, root_attr="", num_label_count=1):
-    children = node.getchildren()
-    dtText_count = 1
-
-    for child in children:
-        child_attr = child.get("class")
-        if child_attr is not None:
-            if child_attr == "sd": # label before meaning content
-                if self_attr == "sdsense":
-                    format_basedon_ancestor(ancestor_attr, prefix="")
-                    if num_label_count == 2:
-                        print(" ", end="")
-                    print_meaning_badge(child.text)
-                else:
-                    print_meaning_badge(child.text)
-            if child_attr == "dtText":
-                dtText(child, ancestor_attr, dtText_count, root_attr) # only meaning text
-                dtText_count += 1
-            if child_attr == "uns":
-                uns(child, ancestor_attr, root_attr, num_label_count)
-            if child_attr == "sub-content-thread":
-                sub_content_thread(child, ancestor_attr, root_attr, num_label_count) # example under the meaning
-            if child_attr == "ca" or child_attr == "dx-jump":
-                extra(child, ancestor_attr, dtText_count, root_attr)
-            if child_attr == "unText":
-                unText_simple(child, ancestor_attr, root_attr, num_label_count)
-            if child_attr == "vi":
-                vi(child, ancestor_attr, root_attr, num_label_count)
+    node_pre_attr = node_pre.get("class")
 
-    print()
+    if "mdash" in node_pre_attr:
+        print_meaning_arrow("->" + text)
+    else:
+        print_meaning_badge(text)
 
 
 ### sense(node, "sense has-sn", "sb-0 sb-entry, "sb has-num has-let ms-lg-4 ms-3 w-100", 1)
 def sense(node, attr, parent_attr, ancestor_attr, num_label_count=1):
     children = node.getchildren()
 
     # meaning without any sign
@@ -646,40 +572,40 @@
 
     # meaning with "1" + "a"
     elif attr == "sense has-sn has-num":
         sn = children[0].getchildren()[0].text
 
         node_prev = node.getprevious()
         if "has-subnum" in ancestor_attr and node_prev is None and "sb-0" in parent_attr:
-            c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
+            c_print(f"#[bold {w_col.meaning_letter}]{sn}", end = " ")
         elif "has-subnum" in ancestor_attr and (node_prev is not None or parent_attr != "pseq no-subnum"):
             if num_label_count == 2:
                 print(" ", end="")
-            c_print(f"  [bold {w_col.meaning_letter}]{sn}", end = " ")
+            c_print(f"  #[bold {w_col.meaning_letter}]{sn}", end = " ")
         else:
-            c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
+            c_print(f"#[bold {w_col.meaning_letter}]{sn}", end = " ")
 
         sense_content = children[1] # class "sense-content w-100"
 
     # meaing with only "b" or "1" + "a" + "(1)", or "1" + "a"
     elif attr == "sense has-sn" or attr == "sen has-sn":
         sn = children[0].getchildren()[0].text
 
         if "has-subnum" in ancestor_attr and "sb-0" in parent_attr:
-            c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
+            c_print(f"#[bold {w_col.meaning_letter}]{sn}", end = " ")
         else:
             if num_label_count == 2:
                     print(" ", end="")
 
             if "letter-only" in ancestor_attr:
                 if "sb-0" not in parent_attr:
                     print("  ", end="")
-                c_print(f"[bold {w_col.meaning_letter}]{sn}", end = " ")
+                c_print(f"#[bold {w_col.meaning_letter}]{sn}", end = " ")
             else:
-                c_print(f"  [bold {w_col.meaning_letter}]{sn}", end = " ")
+                c_print(f"  #[bold {w_col.meaning_letter}]{sn}", end = " ")
 
         sense_content = children[1] # class "sense-content w-100"
 
     # meaning with only (2)
     elif attr == "sense has-num-only has-subnum-only":
         if num_label_count == 2:
             print(" ", end="")
@@ -695,145 +621,159 @@
     # meaning with only number
     elif attr == "sense has-sn has-num-only":
         sense_content = children[1] # class "sense-content w-100"
 
     else:
         sense_content = children[1]
 
-    for c in children:
-        if c.attrib["class"] == "if":
-            print_class_if(c.text.strip())
-        if "badge mw-badge-gray-100" in c.attrib["class"]:
-            print_meaning_badge(c.text.strip(), end="\n")
-
     # "sense-content w-100"
-    elms = sense_content.getchildren()
-    for elm in elms:
+    tags(sense_content, attr, num_label_count)
+
+
+def sb_entry(node, parent_attr, num_label_count=1):
+    child = node.getchildren()[0]
+    attr = node.attrib["class"]         # "sb-0 sb-entry"
+    child_attr = child.attrib["class"]  # "sense has-sn" or "pseq no-subnum"
+    if "pseq" in child_attr:
+        elms = child.getchildren()[0].getchildren()
+        for e in elms:
+            e_attr = e.attrib["class"]  # "sense has-sn"
+            sense(e, e_attr, attr, parent_attr, num_label_count)     # e.g. sense(child, "sense has-sn", "sb-0 sb-entry", "....", 1)
+    elif "sense" in child_attr and child.tag != "span":
+        sense(child, child_attr, attr, parent_attr, num_label_count) # e.g. sense(child, "sense has-sn", "sb-0 sb-entry, "sb has-num has-let ms-lg-4 ms-3 w-100", 1)
+
+
+def tags(node, ancestor_attr, num_label_count):
+    has_badge = True
+
+    for elm in node.iterdescendants():
         elm_attr = elm.get("class")
         if elm_attr is not None:
             if "badge" in elm_attr:
                 text = "".join(list(elm.itertext())).strip()
                 print_meaning_badge(text)
-
-            if elm_attr == "dt " or elm_attr == "dt hasSdSense" or elm_attr == "sdsense":
-                dt(elm, attr, elm_attr, ancestor_attr, num_label_count)
+                continue
 
             if elm_attr == "et":
                 et(elm)
+                continue
 
             if elm_attr == "il ":
                 print_meaning_badge(elm.text.strip(), end=" ")
+                continue
 
             if elm_attr == "if":
                 print_class_if(elm.text)
+                continue
 
             if elm_attr == "sgram":
                 print_class_sgram(elm)
+                continue
 
-            if elm_attr == "unText":
-                unText_simple(elm, attr, ancestor_attr, num_label_count)
+            if elm_attr == "vl":
+                print_meaning_badge(elm.text.strip())
+                continue
 
-            if elm_attr == "vi":
-                vi(elm, attr, ancestor_attr, num_label_count)
+            if elm_attr == "va":
+                print_class_va(elm.text.strip())
+                continue
 
-        else:
-            for i in elm.iterchildren():
-                if i.get("class") == "vl":
-                    print_meaning_badge(i.text.strip())
-                elif i.get("class") == "va":
-                    print_class_va(i.text.strip())
-                elif "prons-entries-list" in i.get("class"):
-                    continue
-                    # print_pron(i)
-                else:
-                    print_meaning_content(i.text, end=" ")
+            if elm_attr == "sd":
+                parent = elm.getparent()
+                parent_attr = parent.get("class")
+                parent_prev = parent.getprevious()
+                if parent_prev is not None and "hasSdSense" in parent_prev.get("class"):
+                    print()
+                if parent_attr is not None and parent_attr == "sdsense":
+                    format_basedon_ancestor(ancestor_attr, prefix="")
 
+                if num_label_count == 2:
+                    print(" ", end="")
 
-def sb_entry(node, parent_attr, num_label_count=1):
-    child = node.getchildren()[0]
-    attr = node.attrib["class"]         # "sb-0 sb-entry"
-    child_attr = child.attrib["class"]  # "sense has-sn" or "pseq no-subnum"
-    if "pseq" in child_attr:
-        elms = child.getchildren()[0].getchildren()
-        for e in elms:
-            e_attr = e.attrib["class"]  # "sense has-sn"
-            sense(e, e_attr, attr, parent_attr, num_label_count)     # e.g. sense(child, "sense has-sn", "sb-0 sb-entry", "....", 1)
-    elif "sense" in child_attr and child.tag != "span":
-        sense(child, child_attr, attr, parent_attr, num_label_count) # e.g. sense(child, "sense has-sn", "sb-0 sb-entry, "sb has-num has-let ms-lg-4 ms-3 w-100", 1)
+                print_meaning_badge(elm.text)
+
+            if elm_attr == "dtText":
+                dtText(elm, ancestor_attr) # only meaning text
+                continue
+
+            if elm_attr == "sub-content-thread":
+                sub_content_thread(elm, ancestor_attr, num_label_count) # example under the meaning
+                has_badge = False
+                continue
+
+            if elm_attr == "ca" or elm_attr == "dx-jump":
+                extra(elm, ancestor_attr)
+                continue
+
+            if elm_attr == "unText":
+                unText_simple(elm, ancestor_attr, num_label_count, has_badge)
+                continue
+
+    print()
 
 
 def vg_sseq_entry_item(node):
     """Print one meaning of one entry(noun entry, adjective entry, or verb entry and so forth). e.g. 1: the monetary worth of something."""
 
     num_label_count = 0
     children = node.getchildren()
     for child in children:
         attr = child.attrib["class"]
         # print number label if any
         if attr == "vg-sseq-entry-item-label":
-            c_print(f"[bold {w_col.meaning_num}]{child.text}", end=" ")
+            c_print(f"#[bold {w_col.meaning_num}]{child.text}", end=" ")
             num_label_count = len(child.text)
 
         # print meaning content
         if "ms-lg-4 ms-3 w-100" in attr:
-            for c in child.iterchildren():
-                cc = c.getchildren()
-                if cc[0].get("class") == "sen has-num-only":
-                    for i in cc[0].iterdescendants():
-                        i_attr = i.get("class")
-                        if i_attr is not None and i.tag == "span":
-                            if ("badge mw-badge" in i_attr) or ("il" in i_attr):
-                                print_meaning_badge(i.text.strip())
-                            if "if" in i_attr:
-                                print_class_if(i.text)
-                            if i_attr == "et":
-                                et(i)
-                            if i_attr == "sgram":
-                                print_class_sgram(i)
-                            if i.get("class") == "vl":
-                                print_meaning_badge(i.text.strip())
-                            if i.get("class") == "va":
-                                print_class_va(i.text.strip())
-                    print()
+            for c in child.iterchildren(): # c:  class="sb-0 sb-entry"
+                cc = c.getchildren()[0]    # cc: class="sen has-num-only"
+                cc_attr = cc.get("class")
+                if cc_attr is not None and cc_attr == "sen has-num-only":
+                    tags(cc, cc_attr, num_label_count)
 
                 # print class "sb-0 sb-entry", "sb-1 sb-entry" ...
                 sb_entry(c, attr, num_label_count)
 
 def et(node):
     for t in node.itertext():
         print(t.strip("\n"), end= "")
 
     if node.getnext() is None:
         print()
     else:
         print("", end=" ")
 
 def vg(node):
-    """Print one entry(e.g. 1 of 3)'s all meanings. e.g. 1 :the monetary worth of somethng 2 :a fair return... 3 :..."""
+    """Print one entry(e.g. 1 of 3)'s all meanings. e.g. 1 :the monetary worth of something 2 :a fair return... 3 :..."""
 
     children = node.getchildren()
     for child in children:
         # print one meaning of one entry
         if "vg-sseq-entry-item" in child.attrib["class"]:
             vg_sseq_entry_item(child)
 
         # print transitive or intransitive
         if child.attrib["class"] == "vd firstVd" or child.attrib["class"] == "vd":
             e = child.getchildren()[0]
-            c_print(f"[bold]{e.text}")
+            c_print(f"#[bold]{e.text}")
 
         # print tags like "informal" and the tags at the same livel with transitives
         if "sls" in child.attrib["class"]:
-             e = child.getchildren()[0]
-             c_print(f"[bold]{e.text}")
+            e = child.getchildren()[0]
+            e_attr = e.get("class")
+            if e_attr is not None and "badge" in e_attr:
+                print_meaning_badge(e.text)
+            else:
+                c_print(f"#[bold]{e.text}")
 
 
 # --- parse class "row entry-header" --- #
 def print_word(text):
-    c_print(f"[{w_col.eh_h1_word} bold]{text}", end=" ")
+    c_print(f"#[{w_col.eh_h1_word} bold]{text}", end=" ")
 
 
 def entry_header_content(node):
     """Print entry header content. e.g. value 1 of 3 noun"""
 
     for elm in node.iterchildren():
         if elm.tag == "h1" or elm.tag == "p":
@@ -844,28 +784,29 @@
 
         if elm.tag == "span":
             num = " ".join(list(elm.itertext()))
             print(num, end=" ")
 
         if elm.tag == "h2":
             type = " ".join(list(elm.itertext()))
-            c_print(f"[bold {w_col.eh_word_type}]{type}", end="\n")
+            c_print(f"#[bold {w_col.eh_word_type}]{type}", end="")
             global word_types
             word_types.append(type.strip().lower())
+    print()
 
 
 def entry_attr(node):
     """Print the pronounciation. e.g. val·​ue |ˈval-(ˌ)yü|"""
 
     for elm in node.iterchildren():
         if "col word-syllables-prons-header-content" in elm.attrib["class"]:
             for i in elm.iterchildren():
                 if i.tag == "span" and i.attrib["class"] == "word-syllables-entry":
                     syllables = i.text
-                    c_print(f"{syllables}", end=" ")
+                    print(f"{syllables}", end=" ")
 
                 if i.tag == "span" and "prons-entries-list-inline" in i.attrib["class"]:
                     print_pron(i, True)
 
 
 def row_entry_header(node, is_redirect=False):
     """Print class row entry-header, the parent and caller of entry_header_content() and entry_attr()."""
@@ -877,123 +818,137 @@
                     entry_header_content(i)
                 if "row entry-attr" in i.attrib["class"]:
                     entry_attr(i)
 
                 if is_redirect:
                     if "hword" == i.attrib["class"]:
                         hword = "".join(list(i.itertext()))
-                        c_print(f"[bold {w_col.eh_h1_word}]{hword}", end=" ")
+                        c_print(f"#[bold {w_col.eh_h1_word}]{hword}", end=" ")
                     if "fl" == i.attrib["class"]:
                         type = "".join(list(i.itertext()))
-                        c_print(f"[bold {w_col.eh_word_type}]{type}", end="")
+                        c_print(f"#[bold {w_col.eh_word_type}]{type}", end="")
 
 # --- parse class "entry-uros" --- #
 def entry_uros(node):
     """Print other word forms. e.g. valueless, valuelessness"""
 
     for elm in node.iterdescendants():
         attr = elm.get("class")
         if attr is not None:
             if elm.tag == "span" and "fw-bold ure" in attr:
-                c_print(f"[bold {w_col.wf}]{elm.text}", end = " ")
+                c_print(f"#[bold {w_col.wf}]{elm.text}", end = " ")
+                continue
+
             if elm.tag == "span" and "fw-bold fl" in attr:
                 next_sibling = elm.getnext()
-                if next_sibling is not None and next_sibling.get("class") == "utxt":
-                    c_print(f"[bold {w_col.wf_type}]{elm.text}", end = "")
-                else:
-                    c_print(f"[bold {w_col.wf_type}]{elm.text}", end = "\n")
+                c_print(f"#[yellow]{elm.text}", end = "")
+                continue
+
             if "ins" in attr:
                 print("", end="")
                 print_class_ins(elm)
+                continue
+
+            if "sl badge" in attr:
+                text = "".join(list(elm.itertext())).strip()
+                print_meaning_badge(text)
+                continue
+
             if "utxt" in attr:
                 for i in elm.iterchildren():
                     sub_attr = i.get("class")
                     if sub_attr is not None and sub_attr == "sub-content-thread":
                         sub_content_thread(i, "", "")
                 print()
+                continue
+
             if "prons-entries-list" in attr:
                 print_pron(elm)
+                continue
+
             if "vrs" in attr:
                 # can't get css element ::before.content like "variants" in the word "duel"
                 child = elm.getchildren()[0]
                 for c in child.iterchildren():
                     attr_c = c.get("class")
                     if attr_c == "il " or attr_c == "vl":
                         print_or_badge(c.text)
+                        continue
                     if attr_c == "va":
                         if c.text is None:
                             for i in child:
                                 print_class_va(i.text)
                         else:
                             print_class_va(c.text)
 
-                        if c.getnext() is None:
-                            print()
+                        continue
                     if "prons-entries-list" in attr_c:
                         continue
+                continue
 
 
 # --- parse class "row headword-row header-ins" --- #
 def row_headword_row_header_ins(node):
     """Print verb types. e.g. valued; valuing"""
 
     children = node.getchildren()[0].getchildren()[0]
     if "ins" in children.attrib["class"]:
         print_class_ins(children)
         print()
 
 
-# --- parse class "row headword-row header-vrs" --- #
 def print_vrs(node):
-    for child in node.iterdescendants():
-        attr = child.get("class")
-        if attr is not None:
-            if "badge mw-badge-gray-100 text-start text-wrap d-inline" in attr:
-                c_print(f"[bold]{child.text.strip()}", end="")
-            elif attr == "il " or attr == "vl":
-                print_or_badge(child.text)
-            elif attr == "va":
-                if child.text is None:
-                    for i in child:
-                        print_class_va(i.text)
-                else:
-                    print_class_va(child.text)
-            elif "prons-entries-list" in attr:
-                print_pron(child)
-            else:
-                continue
-                # print(f"{child.text}", end="")
+    for elm in node.iterchildren():
+        elm_attr = elm.get("class")
+        if elm_attr is not None and "badge mw-badge-gray-100 text-start text-wrap d-inline" in elm_attr:
+            c_print(f"#[bold]{elm.text.strip()}", end="")
+        else:
+            for child in elm.iterdescendants():
+                attr = child.get("class")
+                if attr is not None:
+                    if attr == "il " or attr == "vl":
+                        print_or_badge(child.text)
+                    elif attr == "va":
+                        if child.text is None:
+                            for i in child:
+                                print_class_va(i.text)
+                        else:
+                            print_class_va(child.text)
+                    elif "prons-entries-list" in attr:
+                        print_pron(child)
+                    else:
+                        continue
 
 
+# --- parse class "row headword-row header-vrs" --- #
 def row_headword_row_header_vrs(node):
     """Print word variants. e.g. premise variants or less commonly premiss"""
 
     children = node.getchildren()[0].getchildren()[0] # class "entry-attr vrs"
     print_vrs(children)
-    if not node.getnext().get("class") == "row headword-row header-ins":
-        print()
+    print()
 
 
 # --- parse class "dxnls" --- #
 def dxnls(node):
     """Print dxnls section, such as 'see also', 'compare' etc."""
 
     texts = list(node.itertext())
     for text in texts:
         text = text.strip()
         if not text:
             continue
         if text == "see also":
-            c_print(f"\n[bold {w_col.dxnls_content}]{text.upper()}", end = " ")
+            c_print(f"\n#[bold {w_col.dxnls_content}]{text.upper()}", end = " ")
         elif text == "compare":
-            c_print(f"\n[bold {w_col.dxnls_content}]{text.upper()}", end = " ")
+            c_print(f"\n#[bold {w_col.dxnls_content}]{text.upper()}", end = " ")
         elif text == ",":
-            c_print(f"[{w_col.dxnls_content}]{text}", end = " ")
+            c_print(f"#[{w_col.dxnls_content}]{text}", end = " ")
         else:
-            c_print(f"[{w_col.dxnls_content}]{text}", end = "")
+            c_print(f"#[{w_col.dxnls_content}]{text}", end = "")
 
     print()
 
 
 # --- parse class "dictionary-entry-[number]" --- #
 def dictionary_entry(node):
     """Print one entry of the word and its attributes like plural types, pronounciations, tenses, etc."""
@@ -1012,74 +967,74 @@
                 if elm.attrib["class"] == "row headword-row header-vrs":
                     row_headword_row_header_vrs(elm)
 
                 if elm.attrib["class"] == "vg":
                     vg(elm)
 
                 if "entry-uros" in elm.attrib["class"]:
-                    entry_uros(elm)
+                    for i in elm.iterchildren():
+                        entry_uros(i)
+                        print()
 
                 if elm.attrib["class"] == "dxnls":
                     dxnls(elm)
 
                 if elm.attrib["class"] == "mt-3":
                     badge = elm.getchildren()[0] # class "lbs badge mw-badge-gray-100 text-start text-wrap d-inline"
                     print_header_badge(badge.text, end="\n")
 
                 if elm.attrib["class"] == "cxl-ref":
                     text = list(elm.itertext())
-                    print_meaning_content(":", end="")
+                    print_meaning_content(": ", end="")
                     for t in text:
                         t = t.strip()
                         if t:
                             print_meaning_content(t, end=" ")
-                    print()
 
         except:
             continue
 
 
 ##############################
 # --- print abstractions --- #
 ##############################
 
 def print_meaning_badge(text, end=" "):
-    c_print(f"[{w_col.meaning_badge}]{text}", end=end)
+    c_print(f"#[{w_col.meaning_badge}]{text}", end=end)
 
 
 def print_header_badge(text, end=" "):
-    c_print(f"[{w_col.meaning_badge}]{text}", end=end)
+    c_print(f"#[{w_col.meaning_badge}]{text}", end=end)
 
 
 def print_meaning_arrow(text, end=" "):
-    c_print(f"[{w_col.meaning_arrow}]{text}", end=end)
+    c_print(f"#[{w_col.meaning_arrow}]{text}", end=end)
 
 
 def print_meaning_keyword(text, end=" "):
-    c_print(f"[{w_col.meaning_keyword}]{text}", end=end)
+    c_print(f"#[{w_col.meaning_keyword}]{text}", end=end)
 
 
 def print_meaning_content(text, end=""):
     if text == ": ":
-        c_print(f"[{w_col.meaning_content} bold]{text}", end=end)
+        c_print(f"#[{w_col.meaning_content} bold]{text}", end=end)
     else:
-        c_print(f"[{w_col.meaning_content}]{text}", end=end)
+        c_print(f"#[{w_col.meaning_content}]{text}", end=end)
 
 
-def format_basedon_ancestor(ancestor_attr, prefix="", suffix="", root_attr=""):
+def format_basedon_ancestor(ancestor_attr, prefix="", suffix=""):
     print(prefix, end="")
     if ancestor_attr == "sense has-sn has-num-only":
-        print("   ", end=suffix)
+        print("  ", end=suffix)
     if ancestor_attr == "sense has-sn has-num":
         print("    ", end=suffix)
     if ancestor_attr == "sense has-sn":
-        if "no-sn letter-only" in root_attr:
-            print("  ", end=suffix)
-        else:
-            print("    ", end=suffix)
+        #if "no-sn letter-only" in root_attr:
+        #    print("  ", end=suffix)
+        print("    ", end=suffix)
     if ancestor_attr == "sense  no-subnum":
         print("", end=suffix)
     if ancestor_attr == "sense has-num-only has-subnum-only":
         print("    ", end=suffix)
 
 
 def print_pron(node, header=False):
@@ -1110,59 +1065,58 @@
             if index == 0:
                 if before_semicolon or before_or:
                     print(f"|{pron}|", end="")
                 else:
                     print(f"|{pron}|", end="  ")
             elif index == count - 1:
                 if sibling is not None:
-                    c_print(f"[{w_col.eh_word_syllables}]{pron}", end=" ")
+                    c_print(f"#[{w_col.eh_word_syllables}]{pron}", end=" ")
                 else:
                     if header == True:
-                        c_print(f"[{w_col.eh_word_syllables}]{pron}", end="\n")
+                        c_print(f"#[{w_col.eh_word_syllables}]{pron}", end="\n")
                     else:
-                        c_print(f"[{w_col.eh_word_syllables}]{pron}", end="")
+                        c_print(f"#[{w_col.eh_word_syllables}]{pron}", end="")
             elif pron == "," or pron == ";":
                 continue
             else:
                 text = pron + ", "
-                c_print(f"[{w_col.eh_word_syllables}]{text}", end="")
+                c_print(f"#[{w_col.eh_word_syllables}]{text}", end="")
 
 
 def print_or_badge(text):
-    c_print(f"[{w_col.or_badge}]{text}", end = "")
+    c_print(f"#[{w_col.or_badge}]{text}", end = "")
 
 
 def print_class_if(text, before_semicolon=False, before_il=False):
     if before_semicolon or before_il:
-        c_print(f"[bold]{text}", end="")
+        c_print(f"#[bold]{text}", end="")
     else:
-        c_print(f"[bold]{text}", end=" ")
+        c_print(f"#[bold]{text}", end=" ")
 
 
 def print_class_va(text):
-    c_print(f"[bold]{text}", end=" ")
+    c_print(f"#[bold]{text}", end=" ")
 
 
 def print_class_sgram(node):
     for t in node.itertext():
         text = t.strip("\n").strip()
         if text and text.isalpha():
-            c_print(f"[bold]{t}", end=" ")
+            c_print(f"#[bold]{t}", end=" ")
 
 
 def print_class_ins(node):
     """print node whose class name includes ins, such as 'ins', 'vg-ins'."""
     for child in node:
         attr = child.get("class")
         if attr is not None:
             if attr == "il  il-badge badge mw-badge-gray-100":
                 print_header_badge(child.text.strip(), end=" ")
             elif attr == "prt-a":
                 print_pron(child)
-
             elif attr == "il ":
                 print_or_badge(child.text)
             elif attr == "sep-semicolon":
                 print(f"{child.text}", end="")
             elif attr == "if":
                 next_sibling = child.getnext()
                 if next_sibling is None:
@@ -1174,20 +1128,20 @@
                     elif sub_attr == "il ":
                         print_class_if(child.text, before_il=True)
                     else:
                         print_class_if(child.text, before_semicolon=False)
                 global word_forms
                 word_forms.append(child.text.strip().lower())
             else:
-                print(f"{child.text}", end="")
+                c_print(f"#[bold]{child.text}", end="")
 
 
 def print_dict_name():
     dict_name = "The Merriam-Webster Dictionary"
-    c_print(f"[{w_col.dict_name}]{dict_name}", justify="right")
+    c_print(f"#[{w_col.dict_name}]{dict_name}", justify="right")
 
 
 ###########################################################
 # --- entry point for printing all entries of a word --- #
 ###########################################################
 
 def parse_and_print(nodes, res_url, new_line=False):
@@ -1229,82 +1183,86 @@
 ######################################################
 
 def print_wod_header(node):
     for elm in node.iterdescendants():
         attr = elm.get("class")
         if attr == "w-a-title":
             for c in elm.iterchildren():
-                c_print(f"[{w_col.wod_title} bold]{c.text}", end="")
+                c_print(f"#[{w_col.wod_title} bold]{c.text}", end="")
             print()
 
         if attr == "word-header-txt":
-            c_print(f"[bold]{elm.text}")
+            c_print(f"#[bold]{elm.text}")
 
         if attr == "main-attr":
-            c_print(f"[{w_col.wod_type}]{elm.text}", end="")
+            c_print(f"#[{w_col.wod_type}]{elm.text}", end="")
             print(" | ", end="")
 
         if attr == "word-syllables":
-            c_print(f"[{w_col.wod_syllables}]{elm.text}")
+            c_print(f"#[{w_col.wod_syllables}]{elm.text}")
 
 
 def print_wod_p(node):
     text = node.text
     if text:
-        print(f"{text}", end="")
+        print(text, end="")
+
     for child in node.iterchildren():
         if child is not None and child.tag == "em":
-            c_print(f"[bold]{child.text}", end="")
-            print(f"{child.tail}", end="")
+            t = "".join(list(child.itertext()))
+            c_print(f"#[bold]{t}", end="")
+            print(child.tail, end="")
+            continue
         if child is not None and child.tag == "a":
             child_text = child.text
             child_tail = child.tail
             if child_text == "See the entry >":
                 continue
             else:
                 if child_text is not None:
-                    print(f"{child_text}", end="")
+                    print(child_text, end="")
                 for c in child.iterchildren():
                     if c is not None and c.tag == "em":
-                        c_print(f"[bold]{c.text}", end="")
+                        c_print(f"#[bold]{c.text}", end="")
 
             if child_tail is not None:
-                print(f"{child_tail}", end="")
+                print(child_tail, end="")
+            continue
     print()
 
 
 def print_wod_def(node):
     for elm in node.iterchildren():
         tag = elm.tag
 
         if tag == "h2":
             text = elm.text.strip("\n").strip()
             if text:
-                c_print(f"\n[{w_col.wod_subtitle} bold]{text}")
+                c_print(f"\n#[{w_col.wod_subtitle} bold]{text}")
             children = list(elm.iterchildren())
             if children:
                 child = children[0]
                 tail = child.tail.strip("\n").strip()
-                c_print(f"[{w_col.wod_subtitle} bold]{child.text}", end=" ")
-                c_print(f"[{w_col.wod_subtitle} bold]{tail}", end="\n")
+                c_print(f"#[{w_col.wod_subtitle} bold]{child.text}", end=" ")
+                c_print(f"#[{w_col.wod_subtitle} bold]{tail}", end="\n")
 
         if tag == "p":
             print_wod_p(elm)
 
         if tag == "div" and elm.attrib["class"] == "wotd-examples":
             child = elm.getchildren()[0].getchildren()[0]
             print_wod_p(child)
 
 
 def print_wod_dyk(node):
     for elm in node.iterchildren():
         tag = elm.tag
 
         if tag == "h2":
-            c_print(f"\n[{w_col.wod_subtitle} bold]{elm.text}")
+            c_print(f"\n#[{w_col.wod_subtitle} bold]{elm.text}")
 
         if tag == "p":
             print_wod_p(elm)
 
 
 def parse_and_print_wod(res_url, res_text):
     logger.debug(f"{OP.PARSING.name} {res_url}")
@@ -1317,18 +1275,20 @@
     //*[@class="did-you-know-wrapper"]
     """
 
     nodes = tree.xpath(s)
 
     logger.debug(f"{OP.PRINTING.name} the parsed result of {res_url}")
 
+    print()
     for node in nodes:
         attr = node.attrib["class"]
 
         if "header" in attr:
             print_wod_header(node)
 
         if "definition" in attr:
             print_wod_def(node)
 
         if "did-you-know" in attr:
             print_wod_dyk(node)
+    print()
```

### Comparing `cambridge-3.9.7/cambridge/errors.py` & `cambridge-3.9.8/cambridge/errors.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/cambridge/log.py` & `cambridge-3.9.8/cambridge/log.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/cambridge/main.py` & `cambridge-3.9.8/cambridge/main.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/cambridge/utils.py` & `cambridge-3.9.8/cambridge/utils.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/pyproject.toml` & `cambridge-3.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/screenshots/cambridge.png` & `cambridge-3.9.8/screenshots/cambridge.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/screenshots/fzf.png` & `cambridge-3.9.8/screenshots/fzf.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/screenshots/webster.png` & `cambridge-3.9.8/screenshots/webster.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.7/PKG-INFO` & `cambridge-3.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cambridge
-Version: 3.9.7
+Version: 3.9.8
 Summary: cambridge is a terminal version of Cambridge Dictionary.
 Home-page: https://github.com/KateWang2016/cambridge
 Keywords: dictionary, cambridge, webster, English, web scraping, python
 Author: Kate Wang
 Author-email: kate.wang2018@gmail.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

