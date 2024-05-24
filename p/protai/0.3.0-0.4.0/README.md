# Comparing `tmp/protai-0.3.0.tar.gz` & `tmp/protai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protai-0.3.0.tar", last modified: Thu May 23 14:32:56 2024, max compression
+gzip compressed data, was "protai-0.4.0.tar", last modified: Thu May 23 15:52:17 2024, max compression
```

## Comparing `protai-0.3.0.tar` & `protai-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:32:56.113078 protai-0.3.0/
--rw-rw-rw-   0        0        0     1479 2024-05-23 14:32:56.113078 protai-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      828 2024-05-17 06:24:20.000000 protai-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 14:32:56.092896 protai-0.3.0/protai/
--rw-rw-rw-   0        0        0        5 2024-05-23 14:32:24.000000 protai-0.3.0/protai/VERSION
--rw-rw-rw-   0        0        0       69 2024-05-22 20:52:15.000000 protai-0.3.0/protai/__init__.py
--rw-rw-rw-   0        0        0     4469 2024-05-23 14:23:52.000000 protai-0.3.0/protai/auth.py
--rw-rw-rw-   0        0        0     2345 2024-05-23 14:19:00.000000 protai-0.3.0/protai/protai.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:32:56.111076 protai-0.3.0/protai.egg-info/
--rw-rw-rw-   0        0        0     1479 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 14:32:56.114076 protai-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     4178 2024-05-17 06:22:19.000000 protai-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:52:17.433414 protai-0.4.0/
+-rw-rw-rw-   0        0        0     1107 2024-05-23 14:43:04.000000 protai-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2358 2024-05-23 15:52:17.433414 protai-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1684 2024-05-23 15:41:29.000000 protai-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 15:52:17.407334 protai-0.4.0/protai/
+-rw-rw-rw-   0        0        0        5 2024-05-23 15:47:13.000000 protai-0.4.0/protai/VERSION
+-rw-rw-rw-   0        0        0       69 2024-05-22 20:52:15.000000 protai-0.4.0/protai/__init__.py
+-rw-rw-rw-   0        0        0     4469 2024-05-23 14:23:52.000000 protai-0.4.0/protai/auth.py
+-rw-rw-rw-   0        0        0     2345 2024-05-23 15:47:05.000000 protai-0.4.0/protai/protai.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:52:17.432416 protai-0.4.0/protai.egg-info/
+-rw-rw-rw-   0        0        0     2358 2024-05-23 15:52:17.000000 protai-0.4.0/protai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-23 15:52:17.000000 protai-0.4.0/protai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 15:52:17.000000 protai-0.4.0/protai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-23 15:52:17.000000 protai-0.4.0/protai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-23 15:52:17.000000 protai-0.4.0/protai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 15:52:17.000000 protai-0.4.0/protai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 15:52:17.434915 protai-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     4178 2024-05-17 06:22:19.000000 protai-0.4.0/setup.py
```

### Comparing `protai-0.3.0/protai/auth.py` & `protai-0.4.0/protai/auth.py`

 * *Files identical despite different names*

### Comparing `protai-0.3.0/protai/protai.py` & `protai-0.4.0/protai/protai.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,38 +23,38 @@
 
 def exitHandler(exit_code: int) -> None:
     sys.exit(exit_code)
 
 
 def main():
     if len(sys.argv) < 2:
-        print("Usage: termai <user input>")
+        print("Usage: protai <user input>")
         exitHandler(1)
 
     # user_input = urllib.parse.quote(sys.argv[1])  # Sanitize the user input
     user_input = ""
     for args in sys.argv:
         if args == sys.argv[0]:
             continue
         if args == "-h" or args == "--help":
-            print("Usage: termai <user input>")
+            print("Usage: protai <user input>")
             exitHandler(0)
         if args == "-v" or args == "--version":
             print(f"{ProtAI_VERSION}")
             exitHandler(0)
         if args == "-c" or args == "--change":
             print("Change the API key for the GROQ API")
             exitHandler(changeApiKey())
         user_input += str(args) + " "
     # print(f"[DEBUG] User input is: {user_input}")
 
     # Set the query parameters
     client = Groq(api_key=authGroq())
-    system_prompt = "You are an AI agent called TermAI. You will reply succinctly to any input you receive. \
-        Your replies will be in the Github Markdown format. ALWAYS start your replies with '[TermAI]: ' \
+    system_prompt = "You are an AI agent called ProtAI. You will reply succinctly to any input you receive. \
+        Your replies will be in the Github Markdown format. ALWAYS start your replies with '[ProtAI]: ' \
         If providing code snippets, always ensure code highlighting for the appropriate programming language \
         is applied."
 
     # Send the request to the GROQ API
     chat_completion = client.chat.completions.create(
         messages=[
             {"role": "system", "content": system_prompt},
```

### Comparing `protai-0.3.0/setup.py` & `protai-0.4.0/setup.py`

 * *Files identical despite different names*

