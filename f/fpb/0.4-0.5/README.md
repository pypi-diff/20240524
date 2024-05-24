# Comparing `tmp/fpb-0.4.tar.gz` & `tmp/fpb-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpb-0.4.tar", last modified: Thu May 23 04:05:15 2024, max compression
+gzip compressed data, was "fpb-0.5.tar", last modified: Thu May 23 17:25:28 2024, max compression
```

## Comparing `fpb-0.4.tar` & `fpb-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 04:05:15.972958 fpb-0.4/
--rw-rw-rw-   0        0        0      169 2024-05-23 04:05:15.972958 fpb-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 04:05:15.965954 fpb-0.4/fingerprint_browser/
--rw-rw-rw-   0        0        0       41 2024-05-04 22:20:38.000000 fpb-0.4/fingerprint_browser/__init__.py
--rw-rw-rw-   0        0        0    17625 2024-05-23 04:05:02.000000 fpb-0.4/fingerprint_browser/hubstudio.py
--rw-rw-rw-   0        0        0      299 2024-05-23 03:47:41.000000 fpb-0.4/fingerprint_browser/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 04:05:15.971958 fpb-0.4/fpb.egg-info/
--rw-rw-rw-   0        0        0      169 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-23 04:05:15.000000 fpb-0.4/fpb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 04:05:15.972958 fpb-0.4/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-23 04:05:13.000000 fpb-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:25:28.569553 fpb-0.5/
+-rw-rw-rw-   0        0        0      169 2024-05-23 17:25:28.569553 fpb-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 17:25:28.563552 fpb-0.5/fingerprint_browser/
+-rw-rw-rw-   0        0        0       41 2024-05-04 22:20:38.000000 fpb-0.5/fingerprint_browser/__init__.py
+-rw-rw-rw-   0        0        0    17464 2024-05-23 17:02:02.000000 fpb-0.5/fingerprint_browser/hubstudio.py
+-rw-rw-rw-   0        0        0      299 2024-05-23 03:47:41.000000 fpb-0.5/fingerprint_browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:25:28.569553 fpb-0.5/fpb.egg-info/
+-rw-rw-rw-   0        0        0      169 2024-05-23 17:25:28.000000 fpb-0.5/fpb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-23 17:25:28.000000 fpb-0.5/fpb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:25:28.000000 fpb-0.5/fpb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 17:25:28.000000 fpb-0.5/fpb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 17:25:28.000000 fpb-0.5/fpb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:25:28.570552 fpb-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-23 17:25:27.000000 fpb-0.5/setup.py
```

### Comparing `fpb-0.4/fingerprint_browser/hubstudio.py` & `fpb-0.5/fingerprint_browser/hubstudio.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,14 @@
             os.path.join(client_path, "hubstudio_connector.exe"),
             *cmds,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             creationflags=subprocess.CREATE_NO_WINDOW,
         )
 
-        def on_exit():
-            p.terminate()
-            utils.terminate_process_by_name("hubstudio_connector.exe")
-
-        atexit.register(on_exit)
-
         while True:
             output_line = await p.stdout.readline()
             output_line = output_line.decode().strip()
             if echo:
                 print(output_line)
             if re.match(r'Program started: +{"\d+":"hubstudio_connector.exe"', output_line):
                 break
```

