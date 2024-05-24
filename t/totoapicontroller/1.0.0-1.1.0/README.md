# Comparing `tmp/totoapicontroller-1.0.0.tar.gz` & `tmp/totoapicontroller-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totoapicontroller-1.0.0.tar", last modified: Mon Jan  1 10:58:16 2024, max compression
+gzip compressed data, was "totoapicontroller-1.1.0.tar", last modified: Fri May 24 18:21:23 2024, max compression
```

## Comparing `totoapicontroller-1.0.0.tar` & `totoapicontroller-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nicolasmatteazzi   (501) staff       (20)        0 2024-01-01 10:58:16.537741 totoapicontroller-1.0.0/
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      226 2024-01-01 10:58:16.537610 totoapicontroller-1.0.0/PKG-INFO
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      579 2024-01-01 10:55:20.000000 totoapicontroller-1.0.0/README.md
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)       38 2024-01-01 10:58:16.537777 totoapicontroller-1.0.0/setup.cfg
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      382 2024-01-01 10:57:21.000000 totoapicontroller-1.0.0/setup.py
-drwxr-xr-x   0 nicolasmatteazzi   (501) staff       (20)        0 2024-01-01 10:58:16.535599 totoapicontroller-1.0.0/totoapicontroller/
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)     4826 2024-01-01 10:20:44.000000 totoapicontroller-1.0.0/totoapicontroller/TotoDelegateDecorator.py
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      639 2023-12-31 17:05:43.000000 totoapicontroller-1.0.0/totoapicontroller/TotoLogger.py
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)     1863 2024-01-01 10:20:30.000000 totoapicontroller-1.0.0/totoapicontroller/TotoTokenVerifier.py
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)        0 2023-12-31 17:05:43.000000 totoapicontroller-1.0.0/totoapicontroller/__init__.py
-drwxr-xr-x   0 nicolasmatteazzi   (501) staff       (20)        0 2024-01-01 10:58:16.537280 totoapicontroller-1.0.0/totoapicontroller/model/
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      359 2024-01-01 10:20:51.000000 totoapicontroller-1.0.0/totoapicontroller/model/ExecutionContext.py
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)     1222 2024-01-01 10:21:00.000000 totoapicontroller-1.0.0/totoapicontroller/model/TotoConfig.py
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      116 2023-12-31 17:05:43.000000 totoapicontroller-1.0.0/totoapicontroller/model/UserContext.py
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      967 2024-01-01 10:21:06.000000 totoapicontroller-1.0.0/totoapicontroller/model/ValidationResult.py
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)        0 2023-12-31 17:05:43.000000 totoapicontroller-1.0.0/totoapicontroller/model/__init__.py
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      218 2023-12-31 18:31:21.000000 totoapicontroller-1.0.0/totoapicontroller/model/singleton.py
-drwxr-xr-x   0 nicolasmatteazzi   (501) staff       (20)        0 2024-01-01 10:58:16.536132 totoapicontroller-1.0.0/totoapicontroller.egg-info/
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      226 2024-01-01 10:58:16.000000 totoapicontroller-1.0.0/totoapicontroller.egg-info/PKG-INFO
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      604 2024-01-01 10:58:16.000000 totoapicontroller-1.0.0/totoapicontroller.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)        1 2024-01-01 10:58:16.000000 totoapicontroller-1.0.0/totoapicontroller.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)       51 2024-01-01 10:58:16.000000 totoapicontroller-1.0.0/totoapicontroller.egg-info/requires.txt
--rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)       18 2024-01-01 10:58:16.000000 totoapicontroller-1.0.0/totoapicontroller.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasmatteazzi   (501) staff       (20)        0 2024-05-24 18:21:23.727164 totoapicontroller-1.1.0/
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      226 2024-05-24 18:21:23.727048 totoapicontroller-1.1.0/PKG-INFO
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      579 2024-01-01 10:55:20.000000 totoapicontroller-1.1.0/README.md
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)       38 2024-05-24 18:21:23.727204 totoapicontroller-1.1.0/setup.cfg
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      400 2024-05-24 18:21:22.000000 totoapicontroller-1.1.0/setup.py
+drwxr-xr-x   0 nicolasmatteazzi   (501) staff       (20)        0 2024-05-24 18:21:23.724973 totoapicontroller-1.1.0/totoapicontroller/
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)     4813 2024-05-23 17:34:33.000000 totoapicontroller-1.1.0/totoapicontroller/TotoDelegateDecorator.py
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      639 2023-12-31 17:05:43.000000 totoapicontroller-1.1.0/totoapicontroller/TotoLogger.py
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)     1863 2024-01-01 10:20:30.000000 totoapicontroller-1.1.0/totoapicontroller/TotoTokenVerifier.py
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)        0 2023-12-31 17:05:43.000000 totoapicontroller-1.1.0/totoapicontroller/__init__.py
+drwxr-xr-x   0 nicolasmatteazzi   (501) staff       (20)        0 2024-05-24 18:21:23.726779 totoapicontroller-1.1.0/totoapicontroller/model/
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      359 2024-01-01 10:20:51.000000 totoapicontroller-1.1.0/totoapicontroller/model/ExecutionContext.py
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)     2471 2024-05-24 18:19:20.000000 totoapicontroller-1.1.0/totoapicontroller/model/TotoConfig.py
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      116 2023-12-31 17:05:43.000000 totoapicontroller-1.1.0/totoapicontroller/model/UserContext.py
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      967 2024-01-01 10:21:06.000000 totoapicontroller-1.1.0/totoapicontroller/model/ValidationResult.py
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)        0 2023-12-31 17:05:43.000000 totoapicontroller-1.1.0/totoapicontroller/model/__init__.py
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      218 2023-12-31 18:31:21.000000 totoapicontroller-1.1.0/totoapicontroller/model/singleton.py
+drwxr-xr-x   0 nicolasmatteazzi   (501) staff       (20)        0 2024-05-24 18:21:23.725602 totoapicontroller-1.1.0/totoapicontroller.egg-info/
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      226 2024-05-24 18:21:23.000000 totoapicontroller-1.1.0/totoapicontroller.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)      604 2024-05-24 18:21:23.000000 totoapicontroller-1.1.0/totoapicontroller.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)        1 2024-05-24 18:21:23.000000 totoapicontroller-1.1.0/totoapicontroller.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)       57 2024-05-24 18:21:23.000000 totoapicontroller-1.1.0/totoapicontroller.egg-info/requires.txt
+-rw-r--r--   0 nicolasmatteazzi   (501) staff       (20)       18 2024-05-24 18:21:23.000000 totoapicontroller-1.1.0/totoapicontroller.egg-info/top_level.txt
```

### Comparing `totoapicontroller-1.0.0/README.md` & `totoapicontroller-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `totoapicontroller-1.0.0/totoapicontroller/TotoDelegateDecorator.py` & `totoapicontroller-1.1.0/totoapicontroller/TotoDelegateDecorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             return dlg(request, user_context, execution_context)
 
         return decorator
     
     return delegate
 
 
-def extract_info(request: Request) -> (str, str):
+def extract_info(request: Request) :
     """Extracts needed info from the request
     
     Returns cid and auth header
     """
     
     # Extract cid
     cid = request.headers.get("x-correlation-id")
```

### Comparing `totoapicontroller-1.0.0/totoapicontroller/TotoLogger.py` & `totoapicontroller-1.1.0/totoapicontroller/TotoLogger.py`

 * *Files identical despite different names*

### Comparing `totoapicontroller-1.0.0/totoapicontroller/TotoTokenVerifier.py` & `totoapicontroller-1.1.0/totoapicontroller/TotoTokenVerifier.py`

 * *Files identical despite different names*

### Comparing `totoapicontroller-1.0.0/totoapicontroller/model/ValidationResult.py` & `totoapicontroller-1.1.0/totoapicontroller/model/ValidationResult.py`

 * *Files identical despite different names*

### Comparing `totoapicontroller-1.0.0/totoapicontroller.egg-info/SOURCES.txt` & `totoapicontroller-1.1.0/totoapicontroller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

