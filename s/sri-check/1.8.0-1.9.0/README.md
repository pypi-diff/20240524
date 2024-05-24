# Comparing `tmp/sri-check-1.8.0.tar.gz` & `tmp/sri-check-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sri-check-1.8.0.tar", last modified: Mon Oct 16 13:42:57 2023, max compression
+gzip compressed data, was "sri-check-1.9.0.tar", last modified: Tue Oct 17 11:35:10 2023, max compression
```

## Comparing `sri-check-1.8.0.tar` & `sri-check-1.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:42:57.465780 sri-check-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-16 13:42:45.000000 sri-check-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2023-10-16 13:42:57.465780 sri-check-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11168 2023-10-16 13:42:45.000000 sri-check-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-16 13:42:45.000000 sri-check-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 13:42:57.465780 sri-check-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:42:57.461780 sri-check-1.8.0/sri_check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2023-10-16 13:42:57.000000 sri-check-1.8.0/sri_check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-16 13:42:57.000000 sri-check-1.8.0/sri_check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 13:42:57.000000 sri-check-1.8.0/sri_check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-16 13:42:57.000000 sri-check-1.8.0/sri_check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-16 13:42:57.000000 sri-check-1.8.0/sri_check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-16 13:42:57.000000 sri-check-1.8.0/sri_check.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 13:42:57.465780 sri-check-1.8.0/sricheck/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-16 13:42:45.000000 sri-check-1.8.0/sricheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-16 13:42:45.000000 sri-check-1.8.0/sricheck/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8074 2023-10-16 13:42:45.000000 sri-check-1.8.0/sricheck/sricheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:35:10.186095 sri-check-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-17 11:34:51.000000 sri-check-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2023-10-17 11:35:10.186095 sri-check-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11168 2023-10-17 11:34:51.000000 sri-check-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-17 11:34:51.000000 sri-check-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 11:35:10.186095 sri-check-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:35:10.186095 sri-check-1.9.0/sri_check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2023-10-17 11:35:10.000000 sri-check-1.9.0/sri_check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-17 11:35:10.000000 sri-check-1.9.0/sri_check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 11:35:10.000000 sri-check-1.9.0/sri_check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-17 11:35:10.000000 sri-check-1.9.0/sri_check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-17 11:35:10.000000 sri-check-1.9.0/sri_check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-17 11:35:10.000000 sri-check-1.9.0/sri_check.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:35:10.186095 sri-check-1.9.0/sricheck/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-17 11:34:51.000000 sri-check-1.9.0/sricheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-17 11:34:51.000000 sri-check-1.9.0/sricheck/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8557 2023-10-17 11:34:51.000000 sri-check-1.9.0/sricheck/sricheck.py
```

### Comparing `sri-check-1.8.0/LICENSE` & `sri-check-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sri-check-1.8.0/PKG-INFO` & `sri-check-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sri-check
-Version: 1.8.0
+Version: 1.9.0
 Summary: Subresource Integrity Checker
 Author-email: Marc Wickenden <code@4armed.com>
 Project-URL: Homepage, https://github.com/4armed/sri-check
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sri-check Version: 1.8.0 Summary: Subresource
+Metadata-Version: 2.1 Name: sri-check Version: 1.9.0 Summary: Subresource
 Integrity Checker Author-email: Marc Wickenden
 4armed.com> Project-URL: Homepage, https://github.com/4armed/sri-check
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: beautifulsoup4>=4.0 Requires-Dist: lxml>=4.8 Requires-
 Dist: requests>=2.0 Requires-Dist: selenium>=4.10 # SRI Checker Ridiculously
 simple Python script for grabbing resource tags (script, link) from a remote
 URL and outputting any that don't have an `integrity` attribute for Subresource
```

### Comparing `sri-check-1.8.0/README.md` & `sri-check-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sri-check-1.8.0/pyproject.toml` & `sri-check-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sri-check-1.8.0/sri_check.egg-info/PKG-INFO` & `sri-check-1.9.0/sri_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sri-check
-Version: 1.8.0
+Version: 1.9.0
 Summary: Subresource Integrity Checker
 Author-email: Marc Wickenden <code@4armed.com>
 Project-URL: Homepage, https://github.com/4armed/sri-check
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sri-check Version: 1.8.0 Summary: Subresource
+Metadata-Version: 2.1 Name: sri-check Version: 1.9.0 Summary: Subresource
 Integrity Checker Author-email: Marc Wickenden
 4armed.com> Project-URL: Homepage, https://github.com/4armed/sri-check
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: beautifulsoup4>=4.0 Requires-Dist: lxml>=4.8 Requires-
 Dist: requests>=2.0 Requires-Dist: selenium>=4.10 # SRI Checker Ridiculously
 simple Python script for grabbing resource tags (script, link) from a remote
 URL and outputting any that don't have an `integrity` attribute for Subresource
```

### Comparing `sri-check-1.8.0/sricheck/sricheck.py` & `sri-check-1.9.0/sricheck/sricheck.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,17 +18,20 @@
     tag['crossorigin'] = 'anonymous'
 
     return tag
 
 class SRICheck:
     def __init__(self, url):
         self.browser = False
-        self.headers = {}
+        self.headers = {
+            "User-Agent": "4ARMED SRI Check (https://github.com/4armed/sri-check)",
+        }
         self.skip_checks = False
         self.stdin = False
+        self.verbose = False
 
         if url == "-":
             self.stdin = True
         elif url == "":
             raise ValueError("URL cannot be empty")
         else:
             parsed_url = urlparse(url)
@@ -50,19 +53,25 @@
         if self.stdin is False:
             self.allowlisted_hosts.append(re.escape(urlparse(self.url).netloc))
     
     def set_browser(self, browser):
         self.browser = browser
     
     def set_headers(self, headers):
-        self.headers = headers
+        self.headers = { 
+            **self.headers,
+            **headers
+        }
     
     def set_stdin(self, stdin):
         self.stdin = stdin
     
+    def set_verbose(self, verbose):
+        self.verbose = verbose
+    
     def add_allowlisted_host(self, pattern):
         self.allowlisted_hosts.append(pattern)
     
     def allowlisted_hosts(self):
         return self.allowlisted_hosts
     
     def set_skip_checks(self, skip_checks):
@@ -97,19 +106,19 @@
 
             browser = webdriver.Chrome(options=chrome_options)
 
             def interceptor(request):
                 request.headers.update(self.headers)
 
             browser.request_interceptor = interceptor
-
             browser.get(self.url)
             return browser.page_source
         else:
             # file deepcode ignore Ssrf: The purpose of the script is to parse remote URLs from the CLI
+
             return requests.get(self.url, headers=self.headers).content
 
 
     def get_remote_resource_tags(self, html):
         soup = BeautifulSoup(html, 'lxml')
 
         resource_tags = []
@@ -146,29 +155,33 @@
         return remote_resource_tags
 
     def run(self):
         if self.stdin:
             html = sys.stdin.read()
         else:
             html = self.get_html()
+        
+        if self.verbose is True:
+            print(html)
 
         remote_resource_tags = self.get_remote_resource_tags(html)
 
         return remote_resource_tags
 
 def cli():
     parser = argparse.ArgumentParser()
     parser.add_argument("-g", "--generate", help="Generate sha384 hashes for resources", action="store_true")
     parser.add_argument("-a", "--all", help="Output detected script/link tags regardless of SRI status", action="store_true")
     parser.add_argument("-b", "--browser", help="Use headless browser to retrieve page and run client side rendering", action="store_true")
     parser.add_argument("-H", "--header", help="HTTP header value to send with the request. Specify multiple times if needed", action="append")
     parser.add_argument("-i", "--ignore", help="host to ignore when checking for SRI. e.g. cdn.4armed.com. Specify multiple times if needed", action="append")
     parser.add_argument("-I", "--ignore-regex", help="regex host to ignore when checking for SRI. e.g. .*\.4armed\.com. Specify multiple times if needed", action="append")
-    parser.add_argument("-q", "--quiet", help="Suppress output if all tags have SRI", action="store_true")
+    parser.add_argument("-q", "--quiet", help="Suppress output if all tags have SRI (deprecated: now default, use --verbose)", action="store_true")
     parser.add_argument("-z", "--zero-exit", help="Return zero exit code even if tags are found without SRI (default is exit 99)", action="store_true")
+    parser.add_argument("-v", "--verbose", help="Enable verbose output", action="store_true")
     parser.add_argument("--version", action="version", version=metadata.version("sri-check"))
     parser.add_argument("url", help="Target URL to check for SRI (use - to read from stdin)")
     args = parser.parse_args()
 
     try:
         s = SRICheck(url=args.url)
     except ValueError as error:
@@ -181,14 +194,15 @@
             k, v = header.split(": ")
             headers[k] = v
 
     if len(headers) > 0:
         s.set_headers(headers)
 
     s.set_browser(args.browser)
+    s.set_verbose(args.verbose)
 
     if args.ignore:
         for host in args.ignore:
             s.add_allowlisted_host(re.escape(host))
 
     if args.ignore_regex:
         for pattern in args.ignore_regex:
@@ -203,14 +217,14 @@
                 print(generate_sha(remote_resource_tag))
             else:
                 print(remote_resource_tag['tag'])
         
         if args.zero_exit is False:
             return 99
     else:
-        if args.quiet is False:
+        if args.verbose is True:
             print("[*] No resource tags found without integrity attribute")
         
     return 0
 
 if __name__== "__main__":
     sys.exit(cli())
```

