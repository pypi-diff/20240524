# Comparing `tmp/localizable-0.1.2.tar.gz` & `tmp/localizable-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/localizable-0.1.2.tar", last modified: Wed Oct 23 23:43:22 2013, max compression
+gzip compressed data, was "localizable-0.1.3.tar", last modified: Fri May 24 05:39:25 2024, max compression
```

## Comparing `localizable-0.1.2.tar` & `localizable-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,14 @@
-drwxr-xr-x   0 chrisbal   (501) staff       (20)        0 2013-10-23 23:43:22.000000 localizable-0.1.2/
--rw-r--r--   0 chrisbal   (501) staff       (20)    18035 2013-10-23 22:25:23.000000 localizable-0.1.2/LICENSE
--rw-r--r--   0 chrisbal   (501) staff       (20)     3337 2013-10-23 22:45:54.000000 localizable-0.1.2/localizable.py
--rw-r--r--   0 chrisbal   (501) staff       (20)     1159 2013-10-23 23:43:22.000000 localizable-0.1.2/PKG-INFO
--rw-r--r--   0 chrisbal   (501) staff       (20)      628 2013-10-23 23:26:00.000000 localizable-0.1.2/README.md
--rw-r--r--   0 chrisbal   (501) staff       (20)      497 2013-10-23 23:42:04.000000 localizable-0.1.2/setup.py
+drwxr-xr-x   0 chrisbal   (501) staff       (20)        0 2024-05-24 05:39:25.727491 localizable-0.1.3/
+-rw-r--r--   0 chrisbal   (501) staff       (20)    18035 2024-05-24 05:32:46.000000 localizable-0.1.3/LICENSE
+-rw-r--r--   0 chrisbal   (501) staff       (20)       25 2024-05-24 05:32:46.000000 localizable-0.1.3/MANIFEST.in
+-rw-r--r--   0 chrisbal   (501) staff       (20)      982 2024-05-24 05:39:25.727034 localizable-0.1.3/PKG-INFO
+-rw-r--r--   0 chrisbal   (501) staff       (20)      628 2024-05-24 05:32:46.000000 localizable-0.1.3/README.md
+drwxr-xr-x   0 chrisbal   (501) staff       (20)        0 2024-05-24 05:39:25.726542 localizable-0.1.3/localizable.egg-info/
+-rw-r--r--   0 chrisbal   (501) staff       (20)      982 2024-05-24 05:39:25.000000 localizable-0.1.3/localizable.egg-info/PKG-INFO
+-rw-r--r--   0 chrisbal   (501) staff       (20)      227 2024-05-24 05:39:25.000000 localizable-0.1.3/localizable.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisbal   (501) staff       (20)        1 2024-05-24 05:39:25.000000 localizable-0.1.3/localizable.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisbal   (501) staff       (20)        8 2024-05-24 05:39:25.000000 localizable-0.1.3/localizable.egg-info/requires.txt
+-rw-r--r--   0 chrisbal   (501) staff       (20)       12 2024-05-24 05:39:25.000000 localizable-0.1.3/localizable.egg-info/top_level.txt
+-rw-r--r--   0 chrisbal   (501) staff       (20)     3346 2024-05-24 05:32:46.000000 localizable-0.1.3/localizable.py
+-rw-r--r--   0 chrisbal   (501) staff       (20)       38 2024-05-24 05:39:25.727593 localizable-0.1.3/setup.cfg
+-rw-r--r--   0 chrisbal   (501) staff       (20)      548 2024-05-24 05:38:54.000000 localizable-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `localizable-0.1.2/LICENSE` & `localizable-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `localizable-0.1.2/localizable.py` & `localizable-0.1.3/localizable.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,31 +36,31 @@
         else:
             return content
     if filename is None:
         return None
     return _get_content_from_file(filename, format_encoding)
 
 def _get_content_from_file(filename, encoding):
-    f = open(filename, 'r')
+    f = open(filename, 'rb')
     try:
         content = f.read()
         if chardet.detect(content)['encoding'].startswith(format_encoding):
             #f = f.decode(format_encoding)
             encoding = format_encoding
         else:
             #f = f.decode(default_encoding)
             encoding = 'utf-8'
         f.close()
         f = codecs.open(filename, 'r', encoding=encoding)
         return f.read()
-    except IOError, e:
-        print "Error opening file %s with encoding %s: %s" %\
-                (filename, format_encoding, e.message)
-    except Exception, e:
-        print "Unhandled exception: %s" % e.message
+    except IOError as e:
+        print("Error opening file %s with encoding %s: %s" %\
+                (filename, format_encoding, e.message))
+    except Exception as e:
+        print("Unhandled exception: %s" % e.message)
     finally:
         f.close()
 
 def parse_strings(content="", filename=None):
     """Parse an apple .strings file and create a stringset with
     all entries in the file.
 
@@ -90,14 +90,14 @@
         comment = i.group('comment') or ''
         if not key:
             key = i.group('property')
         value = i.group('value')
         while end < start:
             m = c.match(f, end, start) or ws.match(f, end, start)
             if not m or m.start() != end:
-                print "Invalid syntax: %s" %\
-                        f[end:start]
+                print("Invalid syntax: %s" %\
+                        f[end:start])
             end = m.end()
         end = end_
         key = _unescape_key(key)
         stringset.append({'key': key, 'value': _unescape(value), 'comment': comment})
-    return stringset
+    return stringset
```

### Comparing `localizable-0.1.2/PKG-INFO` & `localizable-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: localizable
-Version: 0.1.2
+Version: 0.1.3
 Summary: Localizable.strings parser for Apple-specific localization files
 Home-page: https://github.com/chrisballinger/python-localizable
 Author: Chris Ballinger
 Author-email: chris@chatsecure.org
 License: GPLv2
-Description: python-localizable
-        ==================
-        
-        Localizable.strings parser for Python
-        
-        # Usage
-        
-        Install using pip.
-        
-            $ pip install localizable
-            
-        You can either parse a full string directly or pass a file path:
-        
-        	import localizable
-        	
-        	strings = localizable.parse_strings(filename='Localizable.strings')
-        	strings = localizable.parse_strings(content="content of .strings file") # this works too
-        	
-        The output format is an array of dictionaries, in order, with the following key/value pairs:
-        
-            /* Comment */
-            "Key" = "Value";
-        
-         * `key`: "Key"
-         * `value`: "Value"
-         * `comment`: "Comment"
-         
-        # License
-        
-        GPLv2. Adapted from Transifex.
-Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: chardet
+
+python-localizable
+==================
+
+Localizable.strings parser for Python
+
+# Usage
+
+Install using pip.
+
+    $ pip install localizable
+    
+You can either parse a full string directly or pass a file path:
+
+	import localizable
+	
+	strings = localizable.parse_strings(filename='Localizable.strings')
+	strings = localizable.parse_strings(content="content of .strings file") # this works too
+	
+The output format is an array of dictionaries, in order, with the following key/value pairs:
+
+    /* Comment */
+    "Key" = "Value";
+
+ * `key`: "Key"
+ * `value`: "Value"
+ * `comment`: "Comment"
+ 
+# License
+
+GPLv2. Adapted from Transifex.
```

### Comparing `localizable-0.1.2/README.md` & `localizable-0.1.3/README.md`

 * *Files identical despite different names*

