# Comparing `tmp/jwtgen-0.1.0.tar.gz` & `tmp/jwtgen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtgen-0.1.0.tar", max compression
+gzip compressed data, was "jwtgen-0.1.1.tar", max compression
```

## Comparing `jwtgen-0.1.0.tar` & `jwtgen-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2024-05-23 22:34:39.003454 jwtgen-0.1.0/LICENSE
--rw-r--r--   0        0        0       42 2024-05-23 22:34:39.003605 jwtgen-0.1.0/README.md
--rw-r--r--   0        0        0       22 2024-05-23 22:41:31.139233 jwtgen-0.1.0/jwtgen/__init__.py
--rw-r--r--   0        0        0     2218 2024-05-23 23:49:27.579781 jwtgen-0.1.0/jwtgen/cli.py
--rw-r--r--   0        0        0      167 2024-05-23 23:22:50.903925 jwtgen-0.1.0/jwtgen/jwt_utils.py
--rw-r--r--   0        0        0      227 2024-05-23 22:51:26.531450 jwtgen-0.1.0/jwtgen/version.py
--rw-r--r--   0        0        0      594 2024-05-23 23:18:31.179152 jwtgen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 jwtgen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-23 22:34:39.003454 jwtgen-0.1.1/LICENSE
+-rw-r--r--   0        0        0       42 2024-05-23 22:34:39.003605 jwtgen-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-23 22:41:31.139233 jwtgen-0.1.1/jwtgen/__init__.py
+-rw-r--r--   0        0        0     2854 2024-05-24 00:53:44.214958 jwtgen-0.1.1/jwtgen/cli.py
+-rw-r--r--   0        0        0      308 2024-05-24 00:14:21.690608 jwtgen-0.1.1/jwtgen/jwt_utils.py
+-rw-r--r--   0        0        0      219 2024-05-24 00:07:08.547608 jwtgen-0.1.1/jwtgen/version.py
+-rw-r--r--   0        0        0      594 2024-05-24 00:54:56.393804 jwtgen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 jwtgen-0.1.1/PKG-INFO
```

### Comparing `jwtgen-0.1.0/LICENSE` & `jwtgen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtgen-0.1.0/jwtgen/cli.py` & `jwtgen-0.1.1/jwtgen/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,90 @@
 import argparse
 import logging
 import os
 import json
 from jwtgen.version import get_version
-from jwtgen.jwt_utils import create_jwt
+from jwtgen.jwt_utils import create_jwt, decode_jwt
+import time
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s - %(levelname)s - %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 logging.getLogger("botocore").setLevel(logging.ERROR)
 
+now = int(time.time())
+
 def generate_template():
     template = {
         "scope": "profile email",
         "authorization_details": ["read", "write"],
         "client_id": "a123456",
         "iss": "https://sso.example.com",
         "jti": "aBcD1234EfGh5678IjKl",
-        "aud": "aud://sso.exampleapp.com",
+        "aud": "https://sso.exampleapp.com",
         "sub": "exampleuser",
         "auth_time": 1716307067,
         "groups": [
           "USER",
           "ADMIN"
         ],
         "cn": "u123456",
         "iat": 1716307067,
-        "exp": 1716350267
+        "exp": now + 3600
     }
     with open('jwtgen.json', 'w') as f:
         json.dump(template, f, indent=4)
     print("Template jwtgen.json file created. You can edit this file with your payload.")
 
 def main():
     parser = argparse.ArgumentParser(
         description="JWTGen: A CLI utility for generating JWT tokens."
     )
 
     allowed_algorithms = ["HS256", "HS384", "HS512", "RS256", "RS384", "RS512", "ES256", "ES384", "ES512"]
 
     parser.add_argument("--version", action="version", version=f"%(prog)s {get_version()}")
-    parser.add_argument("--secret", type=str, required=True, help="The secret key to sign the JWT")
+    parser.add_argument("--secret", type=str, help="The secret key to sign the JWT (required for encoding)")
     parser.add_argument("--algorithm", type=str, default="HS256", help="The algorithm to use for signing the JWT", choices=allowed_algorithms)
     parser.add_argument("--generate-template", action="store_true", help="Generate a template jwtgen.json file")
-
+    parser.add_argument("--decode", action="store_true", help="Decode the JWT token")
 
     args = parser.parse_args()
 
+    if args.decode:
+        if not args.secret:
+            logging.error("Secret key is not provided.")
+            return
+        token = input("Enter the JWT token: ")
+        payload = decode_jwt(args.secret.encode(), token)
+        print("Decoded payload:")
+        print(json.dumps(payload, indent=4))
+        return
+
+    if args.generate_template:
+        generate_template()
+        return
+
     if not os.path.exists("jwtgen.json"):
         logging.error("jwtgen.json file not found.")
         generate_template()
         return
 
     with open("jwtgen.json", "r") as f:
         try:
             payload = json.load(f)
         except json.JSONDecodeError:
             logging.error("jwtgen.json is not a valid JSON file.")
             return
 
+    if not args.secret:
+        logging.error("Secret key is not provided.")
+        return
+
     token = create_jwt(args.secret, args.algorithm, payload)
     print(f"{args.algorithm} encoded token: {token}")
 
 if __name__ == "__main__":
     main()
```

### Comparing `jwtgen-0.1.0/pyproject.toml` & `jwtgen-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwtgen"
-version = "0.1.0"
+version = "0.1.1"
 description = "A CLI that generates a JWT based on a local jwtgen.json file"
 authors = ["Aaron West <aphexlog@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aphexlog/jwtgen"
 packages = [{ include = "jwtgen", from = "." }]
 scripts = { "jwtgen" = "jwtgen.cli:main" }
```

### Comparing `jwtgen-0.1.0/PKG-INFO` & `jwtgen-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtgen
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI that generates a JWT based on a local jwtgen.json file
 Home-page: https://github.com/aphexlog/jwtgen
 License: MIT
 Author: Aaron West
 Author-email: aphexlog@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

