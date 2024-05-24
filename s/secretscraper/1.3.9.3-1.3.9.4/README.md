# Comparing `tmp/secretscraper-1.3.9.3.tar.gz` & `tmp/secretscraper-1.3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.9.3.tar", max compression
+gzip compressed data, was "secretscraper-1.3.9.4.tar", max compression
```

## Comparing `secretscraper-1.3.9.3.tar` & `secretscraper-1.3.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.3/LICENSE
--rw-r--r--   0        0        0     8142 2024-04-30 09:50:23.212758 secretscraper-1.3.9.3/README.md
--rw-r--r--   0        0        0     1910 2024-04-30 09:50:23.208488 secretscraper-1.3.9.3/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-30 09:50:23.216292 secretscraper-1.3.9.3/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7755 2024-04-30 09:48:52.854355 secretscraper-1.3.9.3/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.3/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2696 2024-04-30 09:47:48.177990 secretscraper-1.3.9.3/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.3/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    17214 2024-04-30 08:49:48.323754 secretscraper-1.3.9.3/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.9.3/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.3/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14320 2024-04-30 09:28:51.393423 secretscraper-1.3.9.3/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.3/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6774 2024-04-30 09:28:19.272007 secretscraper-1.3.9.3/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.3/src/secretscraper/log.py
--rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.3/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.3/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.3/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2862 2024-04-30 06:43:03.216699 secretscraper-1.3.9.3/src/secretscraper/util.py
--rw-r--r--   0        0        0     9626 1970-01-01 00:00:00.000000 secretscraper-1.3.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.4/LICENSE
+-rw-r--r--   0        0        0     9074 2024-04-30 10:24:02.401501 secretscraper-1.3.9.4/README.md
+-rw-r--r--   0        0        0     1910 2024-05-24 03:08:16.583332 secretscraper-1.3.9.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-05-24 03:07:23.229353 secretscraper-1.3.9.4/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7755 2024-04-30 09:48:52.854355 secretscraper-1.3.9.4/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.4/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2716 2024-05-24 03:03:31.799544 secretscraper-1.3.9.4/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.4/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    17214 2024-04-30 08:49:48.323754 secretscraper-1.3.9.4/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.9.4/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.4/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14636 2024-05-24 03:03:31.805841 secretscraper-1.3.9.4/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.4/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6774 2024-04-30 09:28:19.272007 secretscraper-1.3.9.4/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.4/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.4/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.4/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.4/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2862 2024-04-30 06:43:03.216699 secretscraper-1.3.9.4/src/secretscraper/util.py
+-rw-r--r--   0        0        0    10558 1970-01-01 00:00:00.000000 secretscraper-1.3.9.4/PKG-INFO
```

### Comparing `secretscraper-1.3.9.3/LICENSE` & `secretscraper-1.3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/README.md` & `secretscraper-1.3.9.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -28,14 +28,21 @@
 
 ### Install
 
 ```bash
 pip install secretscraper
 ```
 
+### Update
+
+```bash
+pip install --upgrade secretscraper
+```
+**Note that**, since _Secretscraper_ generates a default configuration under the work directory if `settings.yml` is absent, so remember to update the `settings.yml` to the latest version(just copy from [Customize Configuration](https://github.com/PadishahIII/SecretScraper?tab=readme-ov-file#customize-configuration)).
+
 ### Basic Usage
 
 Start with single target:
 
 ```bash
 secretscraper -u https://scrapeme.live/shop/
 ```
@@ -89,21 +96,26 @@
                                commas, e.g. 200,300-400
   -x, --proxy TEXT             Set proxy, e.g. http://127.0.0.1:8080,
                                socks5://127.0.0.1:7890
   -H, --hide-regex             Hide regex search result
   -F, --follow-redirects       Follow redirects
   -u, --url TEXT               Target url
   --detail                     Show detailed result
+  --validate                   Validate the status of found urls
   -l, --local PATH             Local file or directory, scan local
                                file/directory recursively
   --help                       Show this message and exit.
-
 ```
 
 ### Advanced Usage
+#### Validate the Status of Links
+Use `--validate` option to check the status of found links, this helps reduce invalid links in the result.
+```bash
+secretscraper -u https://scrapeme.live/shop/ --validate --max-page=10
+```
 
 #### Thorough Crawl
 
 The max depth is set to 1, which means only the start urls will be crawled. To change that, you can specify
 via `--max-depth <number>`. Or in a simpler way, use `-m 2` to run the crawler in thorough mode which is equivalent
 to `--max-depth 2`. By default the normal mode `-m 1` is adopted with max depth set to 1.
 ```bash
@@ -127,76 +139,80 @@
 ```
 
 #### Customize Configuration
 The built-in config is shown as below. You can assign custom configuration via `-i settings.yml`.
 ```yaml
 verbose: false
 debug: false
-loglevel: warning
+loglevel: critical
 logpath: log
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
-follow_redirects: false
+follow_redirects: true
 workers_num: 1000
 headers:
   Accept: "*/*"
   Cookie: ""
   User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.87 Safari/537.36 SE 2.X MetaSr 1.0
 
 urlFind:
-  - '["''‘“`]\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
-  - =\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
-  - '["''‘“`]\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
-  - '"([-a-zA-Z0-9()@:%_\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\+.~#?&//={}]+?)"'
-  - href\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})|action\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
+  - "[\"'‘“`]\\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250}?)\\s{0,6}[\"'‘“`]"
+  - "=\\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})"
+  - "[\"'‘“`]\\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250}?)\\s{0,6}[\"'‘“`]"
+  - "\"([-a-zA-Z0-9()@:%_\\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\\+.~#?&//={}]+?)\""
+  - "href\\s{0,6}=\\s{0,6}[\"'‘“`]{0,1}\\s{0,6}([-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})|action\\s{0,6}=\\s{0,6}[\"'‘“`]{0,1}\\s{0,6}([-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})"
 jsFind:
   - (https{0,1}:[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
   - '["''‘“`]\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)'
   - =\s{0,6}[",',’,”]{0,1}\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+
 dangerousPath:
   - logout
   - update
   - remove
   - insert
   - delete
 
 rules:
   - name: Swagger
     regex: \b[\w/]+?((swagger-ui.html)|(\"swagger\":)|(Swagger UI)|(swaggerUi)|(swaggerVersion))\b
     loaded: true
   - name: ID Card
-    regex: \b((\d{8}(0\d|10|11|12)([0-2]\d|30|31)\d{3}\$)|(\d{6}(18|19|20)\d{2}(0[1-9]|10|11|12)([0-2]\d|30|31)\d{3}(\d|X|x)))\b
+    regex: \b((\d{8}(0\d|10|11|12)([0-2]\d|30|31)\d{3})|(\d{6}(18|19|20)\d{2}(0[1-9]|10|11|12)([0-2]\d|30|31)\d{3}(\d|X|x)))\b
     loaded: true
   - name: Phone
-    regex: \b((?:(?:\+|00)86)?1(?:(?:3[\d])|(?:4[5-79])|(?:5[0-35-9])|(?:6[5-7])|(?:7[0-8])|(?:8[\d])|(?:9[189]))\d{8})\b
+    regex: "['\"](1(3([0-35-9]\\d|4[1-8])|4[14-9]\\d|5([\\d]\\d|7[1-79])|66\\d|7[2-35-8]\\d|8\\d{2}|9[89]\\d)\\d{7})['\"]"
     loaded: true
   - name: JS Map
     regex: \b([\w/]+?\.js\.map)
     loaded: true
   - name: URL as a Value
     regex: (\b\w+?=(https?)(://|%3a%2f%2f))
-    loaded: true
+    loaded: false
   - name: Email
-    regex: \b(([a-z0-9][_|\.])*[a-z0-9]+@([a-z0-9][-|_|\.])*[a-z0-9]+\.([a-z]{2,}))\b
+    regex: "['\"]([\\w]+(?:\\.[\\w]+)*@(?:[\\w](?:[\\w-]*[\\w])?\\.)+[\\w](?:[\\w-]*[\\w])?)['\"]"
     loaded: true
   - name: Internal IP
     regex: '[^0-9]((127\.0\.0\.1)|(10\.\d{1,3}\.\d{1,3}\.\d{1,3})|(172\.((1[6-9])|(2\d)|(3[01]))\.\d{1,3}\.\d{1,3})|(192\.168\.\d{1,3}\.\d{1,3}))'
     loaded: true
   - name: Cloud Key
     regex: \b((accesskeyid)|(accesskeysecret)|\b(LTAI[a-z0-9]{12,20}))\b
     loaded: true
   - name: Shiro
     regex: (=deleteMe|rememberMe=)
     loaded: true
   - name: Suspicious API Key
     regex: "[\"'][0-9a-zA-Z]{32}['\"]"
     loaded: true
+  - name: Jwt
+    regex: "['\"](ey[A-Za-z0-9_-]{10,}\\.[A-Za-z0-9._-]{10,}|ey[A-Za-z0-9_\\/+-]{10,}\\.[A-Za-z0-9._\\/+-]{10,})['\"]"
+    loaded: true
 
 ```
 
 ---
 
 # TODO
 - [ ] Support headless browser
@@ -211,16 +227,16 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
-## 2024.4.29 Version 1.3.9
-- Add `--validate` option
+## 2024.4.30 Version 1.3.9
+- Add `--validate` option: Validate urls after the crawler finish, which helps reduce useless links
 - Optimize url collector
 - Optimize built-in regex
 ## 2024.4.29 Version 1.3.8
 - Optimize log output
 - Optimize the performance of `--debug` option
 ## 2024.4.29 Version 1.3.7
 - Test on multiple python versions
```

### Comparing `secretscraper-1.3.9.3/pyproject.toml` & `secretscraper-1.3.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.9.3"
+version = "1.3.9.4"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.9.3/src/secretscraper/cmdline.py` & `secretscraper-1.3.9.4/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/config/__init__.py` & `secretscraper-1.3.9.4/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/config/settings.yml` & `secretscraper-1.3.9.4/src/secretscraper/config/settings.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 verbose: false
 debug: false
 loglevel: critical
 logpath: log
+handler_type: regex
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
 follow_redirects: true
 workers_num: 1000
```

### Comparing `secretscraper-1.3.9.3/src/secretscraper/coroutinue.py` & `secretscraper-1.3.9.4/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/crawler.py` & `secretscraper-1.3.9.4/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/entity.py` & `secretscraper-1.3.9.4/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/exception.py` & `secretscraper-1.3.9.4/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/facade.py` & `secretscraper-1.3.9.4/src/secretscraper/facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,15 +256,21 @@
         # Verbose
         verbose: typing.Optional[bool] = self.custom_settings.get("verbose", None)
         if verbose is not None:
             self.settings["verbose"] = verbose
 
         # Read rules from config file
         rules: typing.Dict[str, str] = read_rules_from_setting(self.settings)
-        handler = get_regex_handler(rules)
+        handler_type = self.settings.get("handler_type", "regex")
+        if handler_type == "hyperscan":
+            handler = get_regex_handler(rules)
+            print_config(f"Using regex handler: Hyperscan")
+        else:
+            handler = get_regex_handler(rules, type_="regex", use_groups=True)
+            print_config(f"Using regex handler: Re")
 
         # Read url/js regex
         rules: typing.List[str] = self.settings.get("urlFind")
         rules.extend(self.settings.get("jsFind"))
         rules_dict = {f"urlFinder_{i}": rule for i, rule in enumerate(rules)}
         parser = RegexURLParser(get_regex_handler(rules_dict, type_="regex", use_groups=True))
```

### Comparing `secretscraper-1.3.9.3/src/secretscraper/filter.py` & `secretscraper-1.3.9.4/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/handler.py` & `secretscraper-1.3.9.4/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/log.py` & `secretscraper-1.3.9.4/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/output_formatter.py` & `secretscraper-1.3.9.4/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/scanner.py` & `secretscraper-1.3.9.4/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/urlparser.py` & `secretscraper-1.3.9.4/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/src/secretscraper/util.py` & `secretscraper-1.3.9.4/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.3/PKG-INFO` & `secretscraper-1.3.9.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.9.3
+Version: 1.3.9.4
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -56,14 +56,21 @@
 
 ### Install
 
 ```bash
 pip install secretscraper
 ```
 
+### Update
+
+```bash
+pip install --upgrade secretscraper
+```
+**Note that**, since _Secretscraper_ generates a default configuration under the work directory if `settings.yml` is absent, so remember to update the `settings.yml` to the latest version(just copy from [Customize Configuration](https://github.com/PadishahIII/SecretScraper?tab=readme-ov-file#customize-configuration)).
+
 ### Basic Usage
 
 Start with single target:
 
 ```bash
 secretscraper -u https://scrapeme.live/shop/
 ```
@@ -117,21 +124,26 @@
                                commas, e.g. 200,300-400
   -x, --proxy TEXT             Set proxy, e.g. http://127.0.0.1:8080,
                                socks5://127.0.0.1:7890
   -H, --hide-regex             Hide regex search result
   -F, --follow-redirects       Follow redirects
   -u, --url TEXT               Target url
   --detail                     Show detailed result
+  --validate                   Validate the status of found urls
   -l, --local PATH             Local file or directory, scan local
                                file/directory recursively
   --help                       Show this message and exit.
-
 ```
 
 ### Advanced Usage
+#### Validate the Status of Links
+Use `--validate` option to check the status of found links, this helps reduce invalid links in the result.
+```bash
+secretscraper -u https://scrapeme.live/shop/ --validate --max-page=10
+```
 
 #### Thorough Crawl
 
 The max depth is set to 1, which means only the start urls will be crawled. To change that, you can specify
 via `--max-depth <number>`. Or in a simpler way, use `-m 2` to run the crawler in thorough mode which is equivalent
 to `--max-depth 2`. By default the normal mode `-m 1` is adopted with max depth set to 1.
 ```bash
@@ -155,76 +167,80 @@
 ```
 
 #### Customize Configuration
 The built-in config is shown as below. You can assign custom configuration via `-i settings.yml`.
 ```yaml
 verbose: false
 debug: false
-loglevel: warning
+loglevel: critical
 logpath: log
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
-follow_redirects: false
+follow_redirects: true
 workers_num: 1000
 headers:
   Accept: "*/*"
   Cookie: ""
   User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.87 Safari/537.36 SE 2.X MetaSr 1.0
 
 urlFind:
-  - '["''‘“`]\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
-  - =\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
-  - '["''‘“`]\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
-  - '"([-a-zA-Z0-9()@:%_\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\+.~#?&//={}]+?)"'
-  - href\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})|action\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
+  - "[\"'‘“`]\\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250}?)\\s{0,6}[\"'‘“`]"
+  - "=\\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})"
+  - "[\"'‘“`]\\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250}?)\\s{0,6}[\"'‘“`]"
+  - "\"([-a-zA-Z0-9()@:%_\\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\\+.~#?&//={}]+?)\""
+  - "href\\s{0,6}=\\s{0,6}[\"'‘“`]{0,1}\\s{0,6}([-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})|action\\s{0,6}=\\s{0,6}[\"'‘“`]{0,1}\\s{0,6}([-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})"
 jsFind:
   - (https{0,1}:[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
   - '["''‘“`]\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)'
   - =\s{0,6}[",',’,”]{0,1}\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+
 dangerousPath:
   - logout
   - update
   - remove
   - insert
   - delete
 
 rules:
   - name: Swagger
     regex: \b[\w/]+?((swagger-ui.html)|(\"swagger\":)|(Swagger UI)|(swaggerUi)|(swaggerVersion))\b
     loaded: true
   - name: ID Card
-    regex: \b((\d{8}(0\d|10|11|12)([0-2]\d|30|31)\d{3}\$)|(\d{6}(18|19|20)\d{2}(0[1-9]|10|11|12)([0-2]\d|30|31)\d{3}(\d|X|x)))\b
+    regex: \b((\d{8}(0\d|10|11|12)([0-2]\d|30|31)\d{3})|(\d{6}(18|19|20)\d{2}(0[1-9]|10|11|12)([0-2]\d|30|31)\d{3}(\d|X|x)))\b
     loaded: true
   - name: Phone
-    regex: \b((?:(?:\+|00)86)?1(?:(?:3[\d])|(?:4[5-79])|(?:5[0-35-9])|(?:6[5-7])|(?:7[0-8])|(?:8[\d])|(?:9[189]))\d{8})\b
+    regex: "['\"](1(3([0-35-9]\\d|4[1-8])|4[14-9]\\d|5([\\d]\\d|7[1-79])|66\\d|7[2-35-8]\\d|8\\d{2}|9[89]\\d)\\d{7})['\"]"
     loaded: true
   - name: JS Map
     regex: \b([\w/]+?\.js\.map)
     loaded: true
   - name: URL as a Value
     regex: (\b\w+?=(https?)(://|%3a%2f%2f))
-    loaded: true
+    loaded: false
   - name: Email
-    regex: \b(([a-z0-9][_|\.])*[a-z0-9]+@([a-z0-9][-|_|\.])*[a-z0-9]+\.([a-z]{2,}))\b
+    regex: "['\"]([\\w]+(?:\\.[\\w]+)*@(?:[\\w](?:[\\w-]*[\\w])?\\.)+[\\w](?:[\\w-]*[\\w])?)['\"]"
     loaded: true
   - name: Internal IP
     regex: '[^0-9]((127\.0\.0\.1)|(10\.\d{1,3}\.\d{1,3}\.\d{1,3})|(172\.((1[6-9])|(2\d)|(3[01]))\.\d{1,3}\.\d{1,3})|(192\.168\.\d{1,3}\.\d{1,3}))'
     loaded: true
   - name: Cloud Key
     regex: \b((accesskeyid)|(accesskeysecret)|\b(LTAI[a-z0-9]{12,20}))\b
     loaded: true
   - name: Shiro
     regex: (=deleteMe|rememberMe=)
     loaded: true
   - name: Suspicious API Key
     regex: "[\"'][0-9a-zA-Z]{32}['\"]"
     loaded: true
+  - name: Jwt
+    regex: "['\"](ey[A-Za-z0-9_-]{10,}\\.[A-Za-z0-9._-]{10,}|ey[A-Za-z0-9_\\/+-]{10,}\\.[A-Za-z0-9._\\/+-]{10,})['\"]"
+    loaded: true
 
 ```
 
 ---
 
 # TODO
 - [ ] Support headless browser
@@ -239,16 +255,16 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
-## 2024.4.29 Version 1.3.9
-- Add `--validate` option
+## 2024.4.30 Version 1.3.9
+- Add `--validate` option: Validate urls after the crawler finish, which helps reduce useless links
 - Optimize url collector
 - Optimize built-in regex
 ## 2024.4.29 Version 1.3.8
 - Optimize log output
 - Optimize the performance of `--debug` option
 ## 2024.4.29 Version 1.3.7
 - Test on multiple python versions
```

