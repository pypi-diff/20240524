# Comparing `tmp/adjuster-3.236.tar.gz` & `tmp/adjuster-3.237.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adjuster-3.236.tar", last modified: Thu May 16 18:10:26 2024, max compression
+gzip compressed data, was "adjuster-3.237.tar", last modified: Fri May 24 10:34:52 2024, max compression
```

## Comparing `adjuster-3.236.tar` & `adjuster-3.237.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 18:10:26.664259 adjuster-3.236/
--rw-r--r--   0 silbrown   (501) staff       (20)    11357 2021-08-21 08:25:30.000000 adjuster-3.236/LICENSE
--rw-r--r--   0 silbrown   (501) staff       (20)    66595 2024-05-16 18:10:26.663820 adjuster-3.236/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 18:10:26.659190 adjuster-3.236/adjuster/
--rwxr-xr-x   0 silbrown   (501) staff       (20)   490709 2024-05-16 18:10:26.000000 adjuster-3.236/adjuster/__init__.py
--rw-r--r--   0 silbrown   (501) staff       (20)       32 2024-05-16 18:10:26.000000 adjuster-3.236/adjuster/__main__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 18:10:26.663029 adjuster-3.236/adjuster.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)    66595 2024-05-16 18:10:26.000000 adjuster-3.236/adjuster.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      252 2024-05-16 18:10:26.000000 adjuster-3.236/adjuster.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-16 18:10:26.000000 adjuster-3.236/adjuster.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       53 2024-05-16 18:10:26.000000 adjuster-3.236/adjuster.egg-info/entry_points.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-16 18:10:26.000000 adjuster-3.236/adjuster.egg-info/requires.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        9 2024-05-16 18:10:26.000000 adjuster-3.236/adjuster.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-16 18:10:26.664388 adjuster-3.236/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)    66735 2024-05-16 18:10:26.000000 adjuster-3.236/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-24 10:34:52.458736 adjuster-3.237/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-24 10:34:47.000000 adjuster-3.237/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    66595 2024-05-24 10:34:52.458736 adjuster-3.237/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-24 10:34:52.458736 adjuster-3.237/adjuster/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)   490917 2024-05-24 10:34:52.000000 adjuster-3.237/adjuster/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       32 2024-05-24 10:34:52.000000 adjuster-3.237/adjuster/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-24 10:34:52.458736 adjuster-3.237/adjuster.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    66595 2024-05-24 10:34:52.000000 adjuster-3.237/adjuster.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      252 2024-05-24 10:34:52.000000 adjuster-3.237/adjuster.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-24 10:34:52.000000 adjuster-3.237/adjuster.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       53 2024-05-24 10:34:52.000000 adjuster-3.237/adjuster.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-24 10:34:52.000000 adjuster-3.237/adjuster.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-24 10:34:52.000000 adjuster-3.237/adjuster.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-24 10:34:52.458736 adjuster-3.237/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    66735 2024-05-24 10:34:52.000000 adjuster-3.237/setup.py
```

### Comparing `adjuster-3.236/LICENSE` & `adjuster-3.237/LICENSE`

 * *Files identical despite different names*

### Comparing `adjuster-3.236/PKG-INFO` & `adjuster-3.237/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: adjuster
-Version: 3.236
+Version: 3.237
 Summary: the Web Adjuster domain-rewriting proxy
 Home-page: http://ssb22.user.srcf.net/adjuster/
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: all
+Platform: any
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,15 +32,15 @@
 
 * Remove problematic markup from pages, etc.
 
 _Domain rewriting_ means you do not need to be able to change the device’s proxy settings—you simply go to a different address. However, _only the domain part is different_, so most in-site scripting should work as-is, without needing delicate alterations to its URI handling. For example, if you have a server called `adjuster.example.org` and you want to see `www.example.com`, simply go to `www.example.com.adjuster.example.org`. Your server ideally needs a wildcard domain, but you can manage without one in some cases, and Web Adjuster can also be a “real” HTTP proxy for local use on a desktop etc.
 
 Because it is based on a single-threaded event-driven Tornado server, Web Adjuster can efficiently handle connections even on a low-power machine like the original Raspberry Pi. (Add-on programs run in other threads, but this is seldom a slow-down in practice.) Tornado also makes Web Adjuster easier to set up: it is a separate, self-contained server that doesn’t need to be worked into the configuration of another one—it can listen on an alternate port (and can be password protected)—but if you prefer you can configure it to share port 80 with another server.
 
-Options for Web Adjuster v3.235
+Options for Web Adjuster v3.237
 ============
 
 General options
 ---------------
 
 `--config` 
 : Name of the configuration file to read, if any. The process's working directory will be set to that of the configuration file so that relative pathnames can be used inside it. Any option that would otherwise have to be set on the command line may be placed in this file as an option="value" or option='value' line (without any double-hyphen prefix). Multi-line values are possible if you quote them in """...""", and you can use standard \ escapes. You can also set config= in the configuration file itself to import another configuration file (for example if you have per-machine settings and global settings). If you want there to be a default configuration file without having to set it on the command line every time, an alternative option is to set the ADJUSTER_CFG environment variable.
```

### Comparing `adjuster-3.236/adjuster/__init__.py` & `adjuster-3.237/adjuster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # (can be run in either Python 2 or Python 3;
 # has been tested with Tornado versions 2 through 6)
 
-"Web Adjuster v3.236 (c) 2012-23 Silas S. Brown"
+"Web Adjuster v3.237 (c) 2012-24 Silas S. Brown"
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # 
 #     http://www.apache.org/licenses/LICENSE-2.0
 # 
@@ -550,17 +550,18 @@
 
 try: # can we page the help text?
     # (Tornado 2 just calls the module-level print_help, but Tornado 3 includes some direct calls to the object's method, so we have to override the latter.  Have to use __dict__ because they override __setattr__.)
     import pydoc ; pydoc.pager # ensure present
     def new_top(*args):
         dat = StringIO()
         dat.write(twoline_program_name+"\n")
-        tornado.options.options.old_top(dat)
+        old_top(dat)
         pydoc.pager(dat.getvalue())
-    tornado.options.options.__dict__['old_top'] = tornado.options.options.print_help
+        raise SystemExit
+    old_top = tornado.options.options.print_help
     tornado.options.options.__dict__['print_help'] = new_top
 except: pass # oh well, can't page the help text
 
 #@file: domain-rewrite.py
 # --------------------------------------------------
 # Domain-rewriting service routines
 # --------------------------------------------------
@@ -3715,15 +3716,19 @@
             if webdriver_AL[self.WA_PjsIndex]:
                 self.request.headers["Accept-Language"] = webdriver_AL[self.WA_PjsIndex]
             webdriver_inProgress[self.WA_PjsIndex].add(self.request.uri)
         elif not self.isSslUpstream:
             if self.handleSSHTunnel(): return
             if self.handleSpecificIPs(): return
             # TODO: Slow down heavy users by self.request.remote_ip ?
-            if extensions.handle("http://"+self.request.host+self.request.uri,self):
+            try: extensionHandled = extensions.handle("http://"+self.request.host+self.request.uri,self)
+            except:
+                self.request.suppress_logger_host_convert = True # counted as 'sort of handled' so we get the correct log entry after the exception
+                raise
+            if extensionHandled:
                 self.request.suppress_logger_host_convert = True
                 return self.myfinish()
             if cssReload_cookieSuffix and cssReload_cookieSuffix in self.request.uri:
                 ruri,rest = self.request.uri.split(cssReload_cookieSuffix,1)
                 self.setCookie_with_dots(rest)
                 return self.redirect(ruri) # so can set another
         self.cookieViaURL = None
```

### Comparing `adjuster-3.236/adjuster.egg-info/PKG-INFO` & `adjuster-3.237/adjuster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: adjuster
-Version: 3.236
+Version: 3.237
 Summary: the Web Adjuster domain-rewriting proxy
 Home-page: http://ssb22.user.srcf.net/adjuster/
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: all
+Platform: any
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,15 +32,15 @@
 
 * Remove problematic markup from pages, etc.
 
 _Domain rewriting_ means you do not need to be able to change the device’s proxy settings—you simply go to a different address. However, _only the domain part is different_, so most in-site scripting should work as-is, without needing delicate alterations to its URI handling. For example, if you have a server called `adjuster.example.org` and you want to see `www.example.com`, simply go to `www.example.com.adjuster.example.org`. Your server ideally needs a wildcard domain, but you can manage without one in some cases, and Web Adjuster can also be a “real” HTTP proxy for local use on a desktop etc.
 
 Because it is based on a single-threaded event-driven Tornado server, Web Adjuster can efficiently handle connections even on a low-power machine like the original Raspberry Pi. (Add-on programs run in other threads, but this is seldom a slow-down in practice.) Tornado also makes Web Adjuster easier to set up: it is a separate, self-contained server that doesn’t need to be worked into the configuration of another one—it can listen on an alternate port (and can be password protected)—but if you prefer you can configure it to share port 80 with another server.
 
-Options for Web Adjuster v3.235
+Options for Web Adjuster v3.237
 ============
 
 General options
 ---------------
 
 `--config` 
 : Name of the configuration file to read, if any. The process's working directory will be set to that of the configuration file so that relative pathnames can be used inside it. Any option that would otherwise have to be set on the command line may be placed in this file as an option="value" or option='value' line (without any double-hyphen prefix). Multi-line values are possible if you quote them in """...""", and you can use standard \ escapes. You can also set config= in the configuration file itself to import another configuration file (for example if you have per-machine settings and global settings). If you want there to be a default configuration file without having to set it on the command line every time, an alternative option is to set the ADJUSTER_CFG environment variable.
```

### Comparing `adjuster-3.236/setup.py` & `adjuster-3.237/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages;setup(name='adjuster',version='3.236',entry_points={'console_scripts':['adjuster=adjuster.__init__:main']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/adjuster/',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='the Web Adjuster domain-rewriting proxy',long_description=r'''Web Adjuster
+from setuptools import setup, find_packages;setup(name='adjuster',version='3.237',entry_points={'console_scripts':['adjuster=adjuster.__init__:main']},license='Apache 2',platforms='any',url='http://ssb22.user.srcf.net/adjuster/',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='the Web Adjuster domain-rewriting proxy',long_description=r'''Web Adjuster
 ============
 
 Web Adjuster is a Tornado-based, domain-rewriting proxy for applying custom processing to Web pages. It is particularly meant for users of smartphones etc as these might not support browser extensions. Web Adjuster can:
 
 * Add a custom stylesheet to change size, layout and colours
 
 * Add custom Javascript to all pages, allowing many desktop browser extensions to work as-is on a smartphone or tablet
@@ -15,15 +15,15 @@
 
 * Remove problematic markup from pages, etc.
 
 _Domain rewriting_ means you do not need to be able to change the device’s proxy settings—you simply go to a different address. However, _only the domain part is different_, so most in-site scripting should work as-is, without needing delicate alterations to its URI handling. For example, if you have a server called `adjuster.example.org` and you want to see `www.example.com`, simply go to `www.example.com.adjuster.example.org`. Your server ideally needs a wildcard domain, but you can manage without one in some cases, and Web Adjuster can also be a “real” HTTP proxy for local use on a desktop etc.
 
 Because it is based on a single-threaded event-driven Tornado server, Web Adjuster can efficiently handle connections even on a low-power machine like the original Raspberry Pi. (Add-on programs run in other threads, but this is seldom a slow-down in practice.) Tornado also makes Web Adjuster easier to set up: it is a separate, self-contained server that doesn’t need to be worked into the configuration of another one—it can listen on an alternate port (and can be password protected)—but if you prefer you can configure it to share port 80 with another server.
 
-Options for Web Adjuster v3.235
+Options for Web Adjuster v3.237
 ============
 
 General options
 ---------------
 
 `--config` 
 : Name of the configuration file to read, if any. The process's working directory will be set to that of the configuration file so that relative pathnames can be used inside it. Any option that would otherwise have to be set on the command line may be placed in this file as an option="value" or option='value' line (without any double-hyphen prefix). Multi-line values are possible if you quote them in """...""", and you can use standard \ escapes. You can also set config= in the configuration file itself to import another configuration file (for example if you have per-machine settings and global settings). If you want there to be a default configuration file without having to set it on the command line every time, an alternative option is to set the ADJUSTER_CFG environment variable.
```

