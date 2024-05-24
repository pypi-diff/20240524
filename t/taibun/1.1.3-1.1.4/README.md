# Comparing `tmp/taibun-1.1.3.tar.gz` & `tmp/taibun-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taibun-1.1.3.tar", last modified: Mon May 20 10:37:46 2024, max compression
+gzip compressed data, was "taibun-1.1.4.tar", last modified: Fri May 24 06:35:52 2024, max compression
```

## Comparing `taibun-1.1.3.tar` & `taibun-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.756819 taibun-1.1.3/
--rw-rw-rw-   0        0        0     1099 2024-04-30 01:55:12.000000 taibun-1.1.3/LICENSE
--rw-rw-rw-   0        0        0    16307 2024-05-20 10:37:46.756819 taibun-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    15514 2024-05-20 10:33:29.000000 taibun-1.1.3/README.md
--rw-rw-rw-   0        0        0      103 2024-05-11 09:38:22.000000 taibun-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      875 2024-05-20 10:37:46.765403 taibun-1.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.550818 taibun-1.1.3/taibun/
--rw-rw-rw-   0        0        0       85 2024-05-07 21:05:54.000000 taibun-1.1.3/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.630342 taibun-1.1.3/taibun/data/
--rw-rw-rw-   0        0        0     2188 2024-05-20 10:19:40.000000 taibun-1.1.3/taibun/data/simplified.json
--rw-rw-rw-   0        0        0    70011 2024-05-20 10:02:42.000000 taibun-1.1.3/taibun/data/traditional.json
--rw-rw-rw-   0        0        0      835 2024-05-20 08:22:03.000000 taibun-1.1.3/taibun/data/vars.json
--rw-rw-rw-   0        0        0  1893399 2024-05-20 08:22:41.000000 taibun-1.1.3/taibun/data/words.json
--rw-rw-rw-   0        0        0    25068 2024-05-20 10:16:45.000000 taibun-1.1.3/taibun/taibun.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.748705 taibun-1.1.3/taibun.egg-info/
--rw-rw-rw-   0        0        0    16307 2024-05-20 10:37:46.000000 taibun-1.1.3/taibun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-05-20 10:37:46.000000 taibun-1.1.3/taibun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 10:37:46.000000 taibun-1.1.3/taibun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 10:37:46.000000 taibun-1.1.3/taibun.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 10:37:46.744631 taibun-1.1.3/tests/
--rw-rw-rw-   0        0        0     2350 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_additional.py
--rw-rw-rw-   0        0        0    17804 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_convert_non_cjk.py
--rw-rw-rw-   0        0        0     9343 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_delimiter.py
--rw-rw-rw-   0        0        0     6995 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_format.py
--rw-rw-rw-   0        0        0    18978 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_ipa_conversion.py
--rw-rw-rw-   0        0        0     6841 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_pingyim_conversion.py
--rw-rw-rw-   0        0        0     7306 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_poj_conversion.py
--rw-rw-rw-   0        0        0    12530 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_punctuation.py
--rw-rw-rw-   0        0        0    34066 2024-05-20 09:38:45.000000 taibun-1.1.3/tests/test_sandhi.py
--rw-rw-rw-   0        0        0     7214 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_tailo_conversion.py
--rw-rw-rw-   0        0        0     7304 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_tlpa_conversion.py
--rw-rw-rw-   0        0        0     1573 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_tokenisation.py
--rw-rw-rw-   0        0        0     7197 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_tongiong_conversion.py
--rw-rw-rw-   0        0        0    11681 2024-05-10 21:33:06.000000 taibun-1.1.3/tests/test_zhuyin_conversion.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:35:52.077467 taibun-1.1.4/
+-rw-rw-rw-   0        0        0     1099 2024-04-30 01:55:12.000000 taibun-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0    16546 2024-05-24 06:35:52.076236 taibun-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15753 2024-05-24 06:27:44.000000 taibun-1.1.4/README.md
+-rw-rw-rw-   0        0        0      103 2024-05-11 09:38:22.000000 taibun-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      875 2024-05-24 06:35:52.082208 taibun-1.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 06:35:51.932963 taibun-1.1.4/taibun/
+-rw-rw-rw-   0        0        0       85 2024-05-07 21:05:54.000000 taibun-1.1.4/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:35:51.988478 taibun-1.1.4/taibun/data/
+-rw-rw-rw-   0        0        0     2188 2024-05-20 10:19:40.000000 taibun-1.1.4/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0    70011 2024-05-20 10:02:42.000000 taibun-1.1.4/taibun/data/traditional.json
+-rw-rw-rw-   0        0        0      835 2024-05-20 08:22:03.000000 taibun-1.1.4/taibun/data/vars.json
+-rw-rw-rw-   0        0        0  1893399 2024-05-20 08:22:41.000000 taibun-1.1.4/taibun/data/words.json
+-rw-rw-rw-   0        0        0    25516 2024-05-22 09:22:31.000000 taibun-1.1.4/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:35:52.072377 taibun-1.1.4/taibun.egg-info/
+-rw-rw-rw-   0        0        0    16546 2024-05-24 06:35:51.000000 taibun-1.1.4/taibun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-05-24 06:35:51.000000 taibun-1.1.4/taibun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 06:35:51.000000 taibun-1.1.4/taibun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 06:35:51.000000 taibun-1.1.4/taibun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 06:35:52.063372 taibun-1.1.4/tests/
+-rw-rw-rw-   0        0        0     2350 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_additional.py
+-rw-rw-rw-   0        0        0    17804 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_convert_non_cjk.py
+-rw-rw-rw-   0        0        0     9343 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_delimiter.py
+-rw-rw-rw-   0        0        0     6995 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_format.py
+-rw-rw-rw-   0        0        0    18978 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_ipa_conversion.py
+-rw-rw-rw-   0        0        0     6841 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_pingyim_conversion.py
+-rw-rw-rw-   0        0        0     7306 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_poj_conversion.py
+-rw-rw-rw-   0        0        0    12530 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_punctuation.py
+-rw-rw-rw-   0        0        0    34066 2024-05-20 09:38:45.000000 taibun-1.1.4/tests/test_sandhi.py
+-rw-rw-rw-   0        0        0     7214 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_tailo_conversion.py
+-rw-rw-rw-   0        0        0     7304 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_tlpa_conversion.py
+-rw-rw-rw-   0        0        0     1573 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_tokenisation.py
+-rw-rw-rw-   0        0        0     7197 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_tongiong_conversion.py
+-rw-rw-rw-   0        0        0    11681 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_zhuyin_conversion.py
```

### Comparing `taibun-1.1.3/LICENSE` & `taibun-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/PKG-INFO` & `taibun-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taibun
-Version: 1.1.3
+Version: 1.1.4
 Summary: Taiwanese Hokkien Transliterator and Tokeniser
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: andrei.harbachov@gmail.com
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic
@@ -14,27 +14,32 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[台語](readme/README-oan.md) | [國語](readme/README-cmn.md)
+
+
+
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
-    <img src="[readme/logo.png](https://github.com/andreihar/taibun/raw/main/readme/logo.png)" alt="Logo" width="90" height="80">
+    <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
   </a>
   
 # Taibun
 
 
 
 <!-- PROJECT SHIELDS -->
 [![Contributions][contributions-badge]][contributions]
+[![Live Demo][demo-badge]][demo]
 [![Tests][tests-badge]][tests]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
 [![Downloads][downloads-badge]][pypi]
 
 **Taiwanese Hokkien Transliterator and Tokeniser**
@@ -425,14 +430,16 @@
 The data is licensed under [CC BY-SA 4.0][data-cc]
 
 
 
 <!-- MARKDOWN LINKS -->
 [contributions]: https://github.com/andreihar/taibun/issues
 [contributions-badge]: https://img.shields.io/badge/Contributions-Welcomed-be132d?style=for-the-badge&logo=github
+[demo]: https://taibun.andreihar.com/
+[demo-badge]: https://img.shields.io/badge/Live_Demo-222222?style=for-the-badge&logo=homeadvisor&logoColor=white
 [tests]: https://github.com/andreihar/taibun/actions
 [tests-badge]: https://img.shields.io/github/actions/workflow/status/andreihar/taibun/ci.yaml?style=for-the-badge&logo=github-actions&logoColor=ffffff
 [release-badge]: https://img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-badge
 [release]: https://github.com/andreihar/taibun/releases
 [licence-badge]: https://img.shields.io/github/license/andreihar/taibun?color=000000&style=for-the-badge
 [licence]: LICENSE
 [linkedin-badge]: https://img.shields.io/badge/LinkedIn-0077b5?style=for-the-badge&logo=linkedin&logoColor=ffffff
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: taibun Version: 1.1.3 Summary: Taiwanese Hokkien
+Metadata-Version: 2.1 Name: taibun Version: 1.1.4 Summary: Taiwanese Hokkien
 Transliterator and Tokeniser Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email: andrei.harbachov@gmail.com License: MIT
 Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE
-_[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Tests]
-[tests-badge]][tests] [![Release][release-badge]][release] [![Licence][licence-
-    badge]][licence] [![LinkedIn][linkedin-badge]][linkedin] [![Downloads]
-[downloads-badge]][pypi] **Taiwanese Hokkien Transliterator and Tokeniser** It
-has methods that allow to customise transliteration and retrieve any necessary
-              information about Taiwanese Hokkien pronunciation.
+text/markdown License-File: LICENSE [å°èª](readme/README-oan.md) | [åèª]
+(readme/README-cmn.md)
+ _[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Live
+ Demo][demo-badge]][demo] [![Tests][tests-badge]][tests] [![Release][release-
+ badge]][release] [![Licence][licence-badge]][licence] [![LinkedIn][linkedin-
+  badge]][linkedin] [![Downloads][downloads-badge]][pypi] **Taiwanese Hokkien
+     Transliterator and Tokeniser** It has methods that allow to customise
+transliteration and retrieve any necessary information about Taiwanese Hokkien
+                                pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 --- Table of Contents
    1. _V_e_r_s_i_o_n_s
    2. _I_n_s_t_a_l_l
    3. _U_s_a_g_e
           o _C_o_n_v_e_r_t_e_r
@@ -166,15 +168,17 @@
 [samuel-linkedin]) - Taiwanese and Mandarin translation ## Licence Because
 Taibun is MIT-licensed, any developer can essentially do whatever they want
 with it as long as they include the original copyright and licence notice in
 any copies of the source code. Note, that the data used by the package is
 licensed under a different copyright. The data is licensed under [CC BY-SA 4.0]
 [data-cc] [contributions]: https://github.com/andreihar/taibun/issues
 [contributions-badge]: https://img.shields.io/badge/Contributions-Welcomed-
-be132d?style=for-the-badge&logo=github [tests]: https://github.com/andreihar/
+be132d?style=for-the-badge&logo=github [demo]: https://taibun.andreihar.com/
+[demo-badge]: https://img.shields.io/badge/Live_Demo-222222?style=for-the-
+badge&logo=homeadvisor&logoColor=white [tests]: https://github.com/andreihar/
 taibun/actions [tests-badge]: https://img.shields.io/github/actions/workflow/
 status/andreihar/taibun/ci.yaml?style=for-the-badge&logo=github-
 actions&logoColor=ffffff [release-badge]: https://img.shields.io/github/v/
 release/andreihar/taibun?color=38618c&style=for-the-badge [release]: https://
 github.com/andreihar/taibun/releases [licence-badge]: https://img.shields.io/
 github/license/andreihar/taibun?color=000000&style=for-the-badge [licence]:
 LICENSE [linkedin-badge]: https://img.shields.io/badge/LinkedIn-
```

### Comparing `taibun-1.1.3/README.md` & `taibun-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+[台語](readme/README-oan.md) | [國語](readme/README-cmn.md)
+
+
+
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
-    <img src="[readme/logo.png](https://github.com/andreihar/taibun/raw/main/readme/logo.png)" alt="Logo" width="90" height="80">
+    <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
   </a>
   
 # Taibun
 
 
 
 <!-- PROJECT SHIELDS -->
 [![Contributions][contributions-badge]][contributions]
+[![Live Demo][demo-badge]][demo]
 [![Tests][tests-badge]][tests]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
 [![Downloads][downloads-badge]][pypi]
 
 **Taiwanese Hokkien Transliterator and Tokeniser**
@@ -405,14 +410,16 @@
 The data is licensed under [CC BY-SA 4.0][data-cc]
 
 
 
 <!-- MARKDOWN LINKS -->
 [contributions]: https://github.com/andreihar/taibun/issues
 [contributions-badge]: https://img.shields.io/badge/Contributions-Welcomed-be132d?style=for-the-badge&logo=github
+[demo]: https://taibun.andreihar.com/
+[demo-badge]: https://img.shields.io/badge/Live_Demo-222222?style=for-the-badge&logo=homeadvisor&logoColor=white
 [tests]: https://github.com/andreihar/taibun/actions
 [tests-badge]: https://img.shields.io/github/actions/workflow/status/andreihar/taibun/ci.yaml?style=for-the-badge&logo=github-actions&logoColor=ffffff
 [release-badge]: https://img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-badge
 [release]: https://github.com/andreihar/taibun/releases
 [licence-badge]: https://img.shields.io/github/license/andreihar/taibun?color=000000&style=for-the-badge
 [licence]: LICENSE
 [linkedin-badge]: https://img.shields.io/badge/LinkedIn-0077b5?style=for-the-badge&logo=linkedin&logoColor=ffffff
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-
-_[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Tests]
-[tests-badge]][tests] [![Release][release-badge]][release] [![Licence][licence-
-    badge]][licence] [![LinkedIn][linkedin-badge]][linkedin] [![Downloads]
-[downloads-badge]][pypi] **Taiwanese Hokkien Transliterator and Tokeniser** It
-has methods that allow to customise transliteration and retrieve any necessary
-              information about Taiwanese Hokkien pronunciation.
+[å°èª](readme/README-oan.md) | [åèª](readme/README-cmn.md)
+ _[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Live
+ Demo][demo-badge]][demo] [![Tests][tests-badge]][tests] [![Release][release-
+ badge]][release] [![Licence][licence-badge]][licence] [![LinkedIn][linkedin-
+  badge]][linkedin] [![Downloads][downloads-badge]][pypi] **Taiwanese Hokkien
+     Transliterator and Tokeniser** It has methods that allow to customise
+transliteration and retrieve any necessary information about Taiwanese Hokkien
+                                pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 --- Table of Contents
    1. _V_e_r_s_i_o_n_s
    2. _I_n_s_t_a_l_l
    3. _U_s_a_g_e
           o _C_o_n_v_e_r_t_e_r
@@ -156,15 +157,17 @@
 [samuel-linkedin]) - Taiwanese and Mandarin translation ## Licence Because
 Taibun is MIT-licensed, any developer can essentially do whatever they want
 with it as long as they include the original copyright and licence notice in
 any copies of the source code. Note, that the data used by the package is
 licensed under a different copyright. The data is licensed under [CC BY-SA 4.0]
 [data-cc] [contributions]: https://github.com/andreihar/taibun/issues
 [contributions-badge]: https://img.shields.io/badge/Contributions-Welcomed-
-be132d?style=for-the-badge&logo=github [tests]: https://github.com/andreihar/
+be132d?style=for-the-badge&logo=github [demo]: https://taibun.andreihar.com/
+[demo-badge]: https://img.shields.io/badge/Live_Demo-222222?style=for-the-
+badge&logo=homeadvisor&logoColor=white [tests]: https://github.com/andreihar/
 taibun/actions [tests-badge]: https://img.shields.io/github/actions/workflow/
 status/andreihar/taibun/ci.yaml?style=for-the-badge&logo=github-
 actions&logoColor=ffffff [release-badge]: https://img.shields.io/github/v/
 release/andreihar/taibun?color=38618c&style=for-the-badge [release]: https://
 github.com/andreihar/taibun/releases [licence-badge]: https://img.shields.io/
 github/license/andreihar/taibun?color=000000&style=for-the-badge [licence]:
 LICENSE [linkedin-badge]: https://img.shields.io/badge/LinkedIn-
```

### Comparing `taibun-1.1.3/setup.cfg` & `taibun-1.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6169 6275 6e0d 0a76 6572 7369   = taibun..versi
-00000020: 6f6e 203d 2031 2e31 2e33 0d0a 6175 7468  on = 1.1.3..auth
+00000020: 6f6e 203d 2031 2e31 2e34 0d0a 6175 7468  on = 1.1.4..auth
 00000030: 6f72 203d 2041 6e64 7265 6920 4861 7262  or = Andrei Harb
 00000040: 6163 686f 760d 0a61 7574 686f 725f 656d  achov..author_em
 00000050: 6169 6c20 3d20 616e 6472 6569 2e68 6172  ail = andrei.har
 00000060: 6261 6368 6f76 4067 6d61 696c 2e63 6f6d  bachov@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 5461 6977 616e 6573 6520 486f 6b6b 6965  Taiwanese Hokkie
 00000090: 6e20 5472 616e 736c 6974 6572 6174 6f72  n Transliterator
```

### Comparing `taibun-1.1.3/taibun/data/simplified.json` & `taibun-1.1.4/taibun/data/simplified.json`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/taibun/data/traditional.json` & `taibun-1.1.4/taibun/data/traditional.json`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/taibun/data/vars.json` & `taibun-1.1.4/taibun/data/vars.json`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/taibun/data/words.json` & `taibun-1.1.4/taibun/data/words.json`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/taibun/taibun.py` & `taibun-1.1.4/taibun/taibun.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         },
         'ipa': {
             'convert': {'tsing':'tɕiɪŋ','jiang':'dʑiaŋ','tshing':'tɕʰiɪŋ','tsik':'tɕiɪk','tshik':'tɕʰiɪk','jian':'dʑiɛn','jiat':'dʑiɛt','tshi':'tɕʰi','iann':'iã','ainn':'ãi','iang':'iaŋ','nng':'nŋ','mia':'miã','mui':'muĩ','mue':'muẽ','mua':'muã','ma':'mã','me':'mẽ','mi':'mĩ','moo':'mɔ̃','nia':'niã','nua':'nuã','na':'nã','ne':'nẽ','ni':'nĩ','noo':'nɔ̃','ngia':'ŋiã','ngiu':'ŋiũ','nga':'ŋã','nge':'ŋẽ','ngi':'ŋĩ','ngoo':'ŋɔ̃','ing':'iɪŋ','tsh':'tsʰ','tsi':'tɕi','ian':'iɛn','iat':'iɛt','onn':'ɔ̃','ong':'ɔŋ','ik':'iɪk','ji':'dʑi','kh':'kʰ','ng':'ŋ','oo':'ɔ','nn':'̃','hm':'hm̩','ph':'pʰ','th':'tʰ','ok':'ɔk','om':'ɔm','j':'dz','o':'ə'},
             'convert2': {'p4':'p̚4','p8':'p̚8','k4':'k̚4','k8':'k̚8','t4':'t̚4','t8':'t̚8','h4':'ʔ4','h8':'ʔ8','si':'ɕi','h0':'0'},
             'tones': ['','⁴⁴','⁵³','¹¹','²¹','²⁵','','²²','⁵']
         }
     }
-    __suffixes = ['啊','矣','喂','欸','唅','嘿','諾','乎','唷','喔','嘖']
+    __suffixes = ['啊','矣','喂','欸','唅','嘿','諾','乎','唷','啦','喔','嘖']
     __no_sandhi = ['這','彼','遮','遐']
     __location = ['頂','跤','外','內']
 
     def __init__(self, system='Tailo', dialect='south', format='mark', delimiter=DEFAULT_DELIMITER, sandhi=DEFAULT_SANDHI, punctuation='format', convert_non_cjk=False):
         self.system = system.lower()
         self.format = format
         self.delimiter = delimiter if delimiter != self.DEFAULT_DELIMITER else self.__set_default_delimiter()
@@ -127,15 +127,29 @@
         if 'placement' in config: self.placement = config['placement'] + [s.capitalize() for s in config['placement']]
         if 'convert' in config: self.convert = {**config['convert'], **{k.capitalize(): v.capitalize() for k, v in config['convert'].items()}}
         if 'convert2' in config: self.convert2 = {**config['convert2'], **{k.capitalize(): v.capitalize() for k, v in config['convert2'].items()}}
 
         # Dialect
         self.sandhi_conversion = {'1':'7','7':'3','3':'2','2':'1','5':'7','p4':'p8','t4':'t8','k4':'k8','h4':'2','p8':'p4','t8':'t4','k8':'k4','h8':'3'}
         self.a_sandhi = {'1':'7','2':'1','3':'1','5':'7','p4':'p8','t4':'t8','k4':'k8','h4':'1','p8':'p4','t8':'t4','k8':'k4','h8':'7'}
-        self.word_dict = {k: (v.split('/')[1] if dialect == 'north' else v.split('/')[0]) if '/' in v else v for k, v in word_dict.items()}
+        class WordDict:
+            def __init__(self, word_dict, dialect):
+                self.word_dict = word_dict
+                self.dialect = dialect
+
+            def __getitem__(self, key):
+                value = self.word_dict.get(key)
+                if value and '/' in value:
+                    return value.split('/')[1] if self.dialect == 'north' else value.split('/')[0]
+                return value
+
+            def __contains__(self, key):
+                return key in self.word_dict
+        
+        self.word_dict = WordDict(word_dict, dialect)
         if dialect == 'north':
             self.sandhi_conversion.update({'5':'3'})
             if self.system == 'ipa':
                 self.convert.update({'o':'o'})
                 self.tones = ['','⁵⁵','⁵¹','²¹','³²','²⁴','','³³','⁴']
```

### Comparing `taibun-1.1.3/taibun.egg-info/PKG-INFO` & `taibun-1.1.4/taibun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taibun
-Version: 1.1.3
+Version: 1.1.4
 Summary: Taiwanese Hokkien Transliterator and Tokeniser
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: andrei.harbachov@gmail.com
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic
@@ -14,27 +14,32 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[台語](readme/README-oan.md) | [國語](readme/README-cmn.md)
+
+
+
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
-    <img src="[readme/logo.png](https://github.com/andreihar/taibun/raw/main/readme/logo.png)" alt="Logo" width="90" height="80">
+    <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
   </a>
   
 # Taibun
 
 
 
 <!-- PROJECT SHIELDS -->
 [![Contributions][contributions-badge]][contributions]
+[![Live Demo][demo-badge]][demo]
 [![Tests][tests-badge]][tests]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
 [![Downloads][downloads-badge]][pypi]
 
 **Taiwanese Hokkien Transliterator and Tokeniser**
@@ -425,14 +430,16 @@
 The data is licensed under [CC BY-SA 4.0][data-cc]
 
 
 
 <!-- MARKDOWN LINKS -->
 [contributions]: https://github.com/andreihar/taibun/issues
 [contributions-badge]: https://img.shields.io/badge/Contributions-Welcomed-be132d?style=for-the-badge&logo=github
+[demo]: https://taibun.andreihar.com/
+[demo-badge]: https://img.shields.io/badge/Live_Demo-222222?style=for-the-badge&logo=homeadvisor&logoColor=white
 [tests]: https://github.com/andreihar/taibun/actions
 [tests-badge]: https://img.shields.io/github/actions/workflow/status/andreihar/taibun/ci.yaml?style=for-the-badge&logo=github-actions&logoColor=ffffff
 [release-badge]: https://img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-badge
 [release]: https://github.com/andreihar/taibun/releases
 [licence-badge]: https://img.shields.io/github/license/andreihar/taibun?color=000000&style=for-the-badge
 [licence]: LICENSE
 [linkedin-badge]: https://img.shields.io/badge/LinkedIn-0077b5?style=for-the-badge&logo=linkedin&logoColor=ffffff
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: taibun Version: 1.1.3 Summary: Taiwanese Hokkien
+Metadata-Version: 2.1 Name: taibun Version: 1.1.4 Summary: Taiwanese Hokkien
 Transliterator and Tokeniser Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email: andrei.harbachov@gmail.com License: MIT
 Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE
-_[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Tests]
-[tests-badge]][tests] [![Release][release-badge]][release] [![Licence][licence-
-    badge]][licence] [![LinkedIn][linkedin-badge]][linkedin] [![Downloads]
-[downloads-badge]][pypi] **Taiwanese Hokkien Transliterator and Tokeniser** It
-has methods that allow to customise transliteration and retrieve any necessary
-              information about Taiwanese Hokkien pronunciation.
+text/markdown License-File: LICENSE [å°èª](readme/README-oan.md) | [åèª]
+(readme/README-cmn.md)
+ _[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Live
+ Demo][demo-badge]][demo] [![Tests][tests-badge]][tests] [![Release][release-
+ badge]][release] [![Licence][licence-badge]][licence] [![LinkedIn][linkedin-
+  badge]][linkedin] [![Downloads][downloads-badge]][pypi] **Taiwanese Hokkien
+     Transliterator and Tokeniser** It has methods that allow to customise
+transliteration and retrieve any necessary information about Taiwanese Hokkien
+                                pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 --- Table of Contents
    1. _V_e_r_s_i_o_n_s
    2. _I_n_s_t_a_l_l
    3. _U_s_a_g_e
           o _C_o_n_v_e_r_t_e_r
@@ -166,15 +168,17 @@
 [samuel-linkedin]) - Taiwanese and Mandarin translation ## Licence Because
 Taibun is MIT-licensed, any developer can essentially do whatever they want
 with it as long as they include the original copyright and licence notice in
 any copies of the source code. Note, that the data used by the package is
 licensed under a different copyright. The data is licensed under [CC BY-SA 4.0]
 [data-cc] [contributions]: https://github.com/andreihar/taibun/issues
 [contributions-badge]: https://img.shields.io/badge/Contributions-Welcomed-
-be132d?style=for-the-badge&logo=github [tests]: https://github.com/andreihar/
+be132d?style=for-the-badge&logo=github [demo]: https://taibun.andreihar.com/
+[demo-badge]: https://img.shields.io/badge/Live_Demo-222222?style=for-the-
+badge&logo=homeadvisor&logoColor=white [tests]: https://github.com/andreihar/
 taibun/actions [tests-badge]: https://img.shields.io/github/actions/workflow/
 status/andreihar/taibun/ci.yaml?style=for-the-badge&logo=github-
 actions&logoColor=ffffff [release-badge]: https://img.shields.io/github/v/
 release/andreihar/taibun?color=38618c&style=for-the-badge [release]: https://
 github.com/andreihar/taibun/releases [licence-badge]: https://img.shields.io/
 github/license/andreihar/taibun?color=000000&style=for-the-badge [licence]:
 LICENSE [linkedin-badge]: https://img.shields.io/badge/LinkedIn-
```

### Comparing `taibun-1.1.3/taibun.egg-info/SOURCES.txt` & `taibun-1.1.4/taibun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_additional.py` & `taibun-1.1.4/tests/test_additional.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_convert_non_cjk.py` & `taibun-1.1.4/tests/test_convert_non_cjk.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_delimiter.py` & `taibun-1.1.4/tests/test_delimiter.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_format.py` & `taibun-1.1.4/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_ipa_conversion.py` & `taibun-1.1.4/tests/test_ipa_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_pingyim_conversion.py` & `taibun-1.1.4/tests/test_pingyim_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_poj_conversion.py` & `taibun-1.1.4/tests/test_poj_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_punctuation.py` & `taibun-1.1.4/tests/test_punctuation.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_sandhi.py` & `taibun-1.1.4/tests/test_sandhi.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_tailo_conversion.py` & `taibun-1.1.4/tests/test_tailo_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_tlpa_conversion.py` & `taibun-1.1.4/tests/test_tlpa_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_tokenisation.py` & `taibun-1.1.4/tests/test_tokenisation.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_tongiong_conversion.py` & `taibun-1.1.4/tests/test_tongiong_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.3/tests/test_zhuyin_conversion.py` & `taibun-1.1.4/tests/test_zhuyin_conversion.py`

 * *Files identical despite different names*

