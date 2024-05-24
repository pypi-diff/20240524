# Comparing `tmp/docrawl-1.3.2.tar.gz` & `tmp/docrawl-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-1.3.2.tar", last modified: Thu May 16 23:12:41 2024, max compression
+gzip compressed data, was "docrawl-1.3.3.tar", last modified: Fri May 24 13:04:32 2024, max compression
```

## Comparing `docrawl-1.3.2.tar` & `docrawl-1.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 23:12:41.436941 docrawl-1.3.2/
--rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.3.2/LICENSE
--rw-rw-rw-   0        0        0      527 2024-05-16 23:12:41.434938 docrawl-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 23:12:41.409381 docrawl-1.3.2/docrawl/
--rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.3.2/docrawl/__init__.py
--rw-rw-rw-   0        0        0    13161 2024-05-16 23:10:20.000000 docrawl-1.3.2/docrawl/docrawl_client.py
--rw-rw-rw-   0        0        0    43228 2024-05-10 08:26:51.000000 docrawl-1.3.2/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.3.2/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.3.2/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.3.2/docrawl/elements.py
--rw-rw-rw-   0        0        0      100 2024-05-16 23:10:20.000000 docrawl-1.3.2/docrawl/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-16 23:12:41.434429 docrawl-1.3.2/docrawl.egg-info/
--rw-rw-rw-   0        0        0      527 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 23:12:41.436941 docrawl-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      834 2024-05-16 23:10:45.000000 docrawl-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:04:32.628455 docrawl-1.3.3/
+-rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      527 2024-05-24 13:04:32.627454 docrawl-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 13:04:32.604557 docrawl-1.3.3/docrawl/
+-rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.3.3/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    13277 2024-05-24 12:50:03.000000 docrawl-1.3.3/docrawl/docrawl_client.py
+-rw-rw-rw-   0        0        0    43628 2024-05-24 12:50:03.000000 docrawl-1.3.3/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.3.3/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.3.3/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.3.3/docrawl/elements.py
+-rw-rw-rw-   0        0        0      100 2024-05-16 23:10:20.000000 docrawl-1.3.3/docrawl/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:04:32.627454 docrawl-1.3.3/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-24 13:04:32.000000 docrawl-1.3.3/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-24 13:04:32.000000 docrawl-1.3.3/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 13:04:32.000000 docrawl-1.3.3/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-05-24 13:04:32.000000 docrawl-1.3.3/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 13:04:32.000000 docrawl-1.3.3/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 13:04:32.628455 docrawl-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      834 2024-05-24 12:50:21.000000 docrawl-1.3.3/setup.py
```

### Comparing `docrawl-1.3.2/LICENSE` & `docrawl-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.2/PKG-INFO` & `docrawl-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.3.2
+Version: 1.3.3
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.3.2/docrawl/docrawl_client.py` & `docrawl-1.3.3/docrawl/docrawl_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         timeout_start = time.time()
         while not is_page_loaded and time.time() < timeout_start + timeout:
             try:
                 is_page_loaded = self.get_browser_meta_data()['request']['loaded']
             except:
                 is_page_loaded = False
             time.sleep(0.5)
-            # docrawl_logger.info('Page is still loading, waiting 0.5 sec ...')
+            docrawl_logger.info('Page is still loading, waiting 0.5 sec ...')
 
         if is_page_loaded:
             docrawl_logger.success('Page loaded')
         else:
             docrawl_logger.error('Page was not loaded')
             raise PageDidNotLoadError()
 
@@ -112,15 +112,15 @@
         timeout_start = time.time()
         while not is_function_done and time.time() < timeout_start + timeout:
             try:
                 is_function_done = self.get_browser_meta_data()['function']['done']
             except:
                 is_function_done = False
             time.sleep(0.5)
-            # docrawl_logger.info('Function is still running, waiting 0.5 sec ...')
+            docrawl_logger.info('Function is still running, waiting 0.5 sec ...')
 
         if is_function_done:
             if function_error_message is None:
                 docrawl_logger.success('Spider function finished successfully')
             else:
                 docrawl_logger.error(f'Spider function failed: {function_error_message}')
                 raise SpiderFunctionError(spider_function['error'])
@@ -327,9 +327,12 @@
     def click_name(self, text, timeout=20):
         inp = {
             'text': text
         }
 
         self._execute_function('click_name', inp, timeout)
 
+    def refresh_page_source(self, timeout=30):
+        self._execute_function('refresh_page_source', None, timeout)
+
     def __exit__(self):
         self.close_browser()
```

### Comparing `docrawl-1.3.2/docrawl/docrawl_core.py` & `docrawl-1.3.3/docrawl/docrawl_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,21 @@
             if self.headless:
                 self.options.add_argument("--headless")
 
                 # For headless mode different width of window is needed
                 window_size_x = 1450
 
             try:
-                self.browser = webdriver.Firefox(options=self.options, service=Service(GeckoDriverManager().install()), seleniumwire_options=sw_options)
+                try:
+                    service = Service(GeckoDriverManager().install())
+                except Exception as e:
+                    service = None
+                    docrawl_logger.warning("GeckoDriverManager update was not successful - launching latest Firefox version instead"+str(e))
+                
+                self.browser = webdriver.Firefox(options=self.options, service=service, seleniumwire_options=sw_options)
             except Exception as e:
                 docrawl_logger.error(f'Error while creating Firefox instance {e}')
                 self.browser = webdriver.Firefox(options=self.options)
 
         elif self.driver_type == 'Chrome':
             self.options = ChromeOptions()
 
@@ -953,14 +959,16 @@
 
         # Remove empty rows
         df.dropna(axis=0, how='all', inplace=True)
         df.to_excel(short_filename + '.xlsx')
 
         self.docrawl_client.kv_redis.set(key='extracted_table', value=df)
 
+    def _refresh_page_source(self, inp):
+        self.page = Selector(text=self.browser.page_source)
 
     def initialize_screenshot_thread_if_not_existing(self, screenshot_filename = "website_loading_screenshot.png"):
         
         if self.screenshot_thread is None:
             self.screenshot_thread = ScreenshotThread(docrawl_spider = self, screenshot_filename = screenshot_filename)
             self.screenshot_thread.start()
             self.screenshot_time=0
```

### Comparing `docrawl-1.3.2/docrawl/docrawl_launcher.py` & `docrawl-1.3.3/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.2/docrawl/docrawl_logger.py` & `docrawl-1.3.3/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.2/docrawl/elements.py` & `docrawl-1.3.3/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.2/docrawl.egg-info/PKG-INFO` & `docrawl-1.3.3/docrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.3.2
+Version: 1.3.3
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.3.2/setup.py` & `docrawl-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='1.3.2',
+    version='1.3.3',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```

