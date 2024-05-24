# Comparing `tmp/web-ui-helper-0.1.2.tar.gz` & `tmp/web-ui-helper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-0.1.2.tar", last modified: Fri May 17 08:33:20 2024, max compression
+gzip compressed data, was "web-ui-helper-1.0.0.tar", last modified: Fri May 24 07:42:14 2024, max compression
```

## Comparing `web-ui-helper-0.1.2.tar` & `web-ui-helper-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.529798 web-ui-helper-0.1.2/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      715 2024-05-17 08:33:20.527804 web-ui-helper-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 08:33:20.530794 web-ui-helper-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-17 08:32:37.000000 web-ui-helper-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.478933 web-ui-helper-0.1.2/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.1.2/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.500874 web-ui-helper-0.1.2/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.1.2/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.506858 web-ui-helper-0.1.2/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-07 17:56:47.000000 web-ui-helper-0.1.2/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.508854 web-ui-helper-0.1.2/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.512841 web-ui-helper-0.1.2/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    31244 2024-05-17 08:32:46.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.516833 web-ui-helper-0.1.2/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 07:19:52.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.519851 web-ui-helper-0.1.2/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     1615 2024-05-07 17:57:06.000000 web-ui-helper-0.1.2/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.522842 web-ui-helper-0.1.2/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.1.2/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:33:20.525836 web-ui-helper-0.1.2/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      715 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 08:33:20.000000 web-ui-helper-0.1.2/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.326744 web-ui-helper-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      715 2024-05-24 07:42:14.325748 web-ui-helper-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:42:14.327756 web-ui-helper-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-05-24 07:40:54.000000 web-ui-helper-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.220785 web-ui-helper-1.0.0/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.0/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.283865 web-ui-helper-1.0.0/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.0/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.292836 web-ui-helper-1.0.0/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.0/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.294831 web-ui-helper-1.0.0/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.299817 web-ui-helper-1.0.0/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    31720 2024-05-22 07:02:55.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.303808 web-ui-helper-1.0.0/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.307797 web-ui-helper-1.0.0/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.0/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.310788 web-ui-helper-1.0.0/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.0/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:42:14.323753 web-ui-helper-1.0.0/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      715 2024-05-24 07:42:13.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-05-24 07:42:14.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:42:13.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-24 07:42:13.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 07:42:13.000000 web-ui-helper-1.0.0/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-0.1.2/LICENSE` & `web-ui-helper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/PKG-INFO` & `web-ui-helper-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.1.2
+Version: 1.0.0
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.1.2/setup.py` & `web-ui-helper-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='0.1.2',
+    version='1.0.0',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-0.1.2/web_ui_helper/common/date_extend.py` & `web-ui-helper-1.0.0/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper/common/dir.py` & `web-ui-helper-1.0.0/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper/common/log.py` & `web-ui-helper-1.0.0/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper/common/metaclass.py` & `web-ui-helper-1.0.0/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper/common/platforms.py` & `web-ui-helper-1.0.0/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper/common/webdriver.py` & `web-ui-helper-1.0.0/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-1.0.0/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-1.0.0/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-1.0.0/web_ui_helper/selenium/frame/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -662,20 +662,34 @@
     kwargs.clear()
     return WebDriverWait(driver, timeout).until(
         ec.presence_of_all_elements_located((Locator.get(locator), regx))
     )
 
 
 @loop_find_element
+def get_element(driver: webdriver, locator: str, regx: str, timeout: int = 3, **kwargs) -> WebElement:
+    kwargs.clear()
+    return WebDriverWait(driver, timeout).until(
+        ec.presence_of_element_located((Locator.get(locator), regx))
+    )
+
+
+@loop_find_element
 def get_sub_element(element: WebElement, locator: str, regx: str, **kwargs) -> WebElement:
     kwargs.clear()
     return element.find_element(Locator.get(locator), regx)
 
 
 @loop_find_element
+def get_sub_elements(element: WebElement, locator: str, regx: str, **kwargs) -> [WebElement]:
+    kwargs.clear()
+    return element.find_elements(Locator.get(locator), regx)
+
+
+@loop_find_element
 def js_click(driver: webdriver, element: WebElement, **kwargs):
     kwargs.clear()
     # 使用 JavaScript 点击操作
     driver.execute_script("arguments[0].click();", element)
 
 
 @loop_find_element
```

### Comparing `web-ui-helper-0.1.2/web_ui_helper/terminal/device.py` & `web-ui-helper-1.0.0/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.1.2/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-1.0.0/web_ui_helper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.1.2
+Version: 1.0.0
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.1.2/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-1.0.0/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

