# Comparing `tmp/conson-3.1.9.tar.gz` & `tmp/conson-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conson-3.1.9.tar", last modified: Wed Feb 14 10:14:43 2024, max compression
+gzip compressed data, was "conson-3.2.1.tar", last modified: Fri May 24 08:21:07 2024, max compression
```

## Comparing `conson-3.1.9.tar` & `conson-3.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 10:14:43.392608 conson-3.1.9/
--rw-rw-rw-   0        0        0     1119 2023-12-29 08:11:22.000000 conson-3.1.9/LICENSE.md
--rw-rw-rw-   0        0        0     3346 2024-02-14 10:14:43.391578 conson-3.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3081 2024-02-14 10:14:37.000000 conson-3.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-02-14 10:14:43.382886 conson-3.1.9/conson/
--rw-rw-rw-   0        0        0       52 2023-12-29 08:10:23.000000 conson-3.1.9/conson/__init__.py
--rw-rw-rw-   0        0        0     7080 2024-02-14 10:03:05.000000 conson-3.1.9/conson/conson.py
-drwxrwxrwx   0        0        0        0 2024-02-14 10:14:43.390416 conson-3.1.9/conson.egg-info/
--rw-rw-rw-   0        0        0     3346 2024-02-14 10:14:43.000000 conson-3.1.9/conson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-02-14 10:14:43.000000 conson-3.1.9/conson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 10:14:43.000000 conson-3.1.9/conson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-02-14 10:14:43.000000 conson-3.1.9/conson.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-14 10:14:43.000000 conson-3.1.9/conson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-14 10:14:43.392608 conson-3.1.9/setup.cfg
--rw-rw-rw-   0        0        0      512 2024-02-14 10:14:37.000000 conson-3.1.9/setup.py
+drwxr-xr-x   0 pawelgabrys  (1000) pawelgabrys  (1000)        0 2024-05-24 08:21:07.689030 conson-3.2.1/
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)     1098 2024-05-14 05:57:24.000000 conson-3.2.1/LICENSE.md
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)     3609 2024-05-24 08:21:07.689030 conson-3.2.1/PKG-INFO
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)     3354 2024-05-24 08:20:29.000000 conson-3.2.1/README.md
+drwxr-xr-x   0 pawelgabrys  (1000) pawelgabrys  (1000)        0 2024-05-24 08:21:07.689030 conson-3.2.1/conson/
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)       49 2024-05-14 05:57:24.000000 conson-3.2.1/conson/__init__.py
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)     7956 2024-05-24 08:20:29.000000 conson-3.2.1/conson/conson.py
+drwxr-xr-x   0 pawelgabrys  (1000) pawelgabrys  (1000)        0 2024-05-24 08:21:07.689030 conson-3.2.1/conson.egg-info/
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)     3609 2024-05-24 08:21:07.000000 conson-3.2.1/conson.egg-info/PKG-INFO
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)      214 2024-05-24 08:21:07.000000 conson-3.2.1/conson.egg-info/SOURCES.txt
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)        1 2024-05-24 08:21:07.000000 conson-3.2.1/conson.egg-info/dependency_links.txt
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)       21 2024-05-24 08:21:07.000000 conson-3.2.1/conson.egg-info/requires.txt
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)        7 2024-05-24 08:21:07.000000 conson-3.2.1/conson.egg-info/top_level.txt
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)       38 2024-05-24 08:21:07.693030 conson-3.2.1/setup.cfg
+-rw-r--r--   0 pawelgabrys  (1000) pawelgabrys  (1000)      494 2024-05-24 08:20:29.000000 conson-3.2.1/setup.py
```

### Comparing `conson-3.1.9/LICENSE.md` & `conson-3.2.1/LICENSE.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [2023] [Paweł Gabryś] [github.com/pgabrys94]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) [2023] [Paweł Gabryś] [github.com/pgabrys94]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `conson-3.1.9/PKG-INFO` & `conson-3.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,74 @@
-Metadata-Version: 2.1
-Name: conson
-Version: 3.1.9
-Summary: A simple json configuration file manager
-Author: Paweł Gabryś
-Author-email: p.gabrys@int.pl
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: cryptography>=41.0.3
-
-Module for creating parameters, saving them and loading from JSON formatted file.
-
-    pip install conson
-
-    from .conson import Conson
-
-Usage:
-
-1. Conson(cfile="config.json", cfilepath=os.getcwd(), salt="ch4ng3M3pl3453"):
-    You can set file name/extension and path to config file directory. By default, current working directory is used.
-
-2. Instance call, parameters:
-   Calling Conson instance will return all kwargs that has already been set by create method.
-   Values modified with .veil method will be encrypted and presented in hex value.
-   Parameters:
-
-        <instance>.file
-        <instance>.file = <filename>, <cfilepath=os.getcwd()>
-
-        <instance>.salt
-        <instance>.salt = <your salt>
-
-3. .create(key, *value): 
-    Creates parameter in key=value pair. Accepts single value or list of values.
-    Example:
-
-        settings = Conson()
-
-        settings.create(key1, value1, value2, value3)
-        settings.create(key2, [value1, value2, value3])
-        settings.create(key3, {"subkey1": "value1", "subkey2": value2, "subkey3": value3})
-
-4. .dispose(key):
-    Removes created parameter from instance.
-
-5. .dump()
-    Removes all created parameters. Useful in case when only one instance is invoked and multiple configuration files
-    are being loaded - allows to prevent mixing parameters simply by dumping them out.
-
-6. .veil(key, index="0"):
-    Passes created value through Fernet SHA-256 encryption. We point the key and value index number.
-    Secret key is based on system-related UUID, so decryption is meant to happen only on device the encryption has place.
-    Example:
-
-       settings.veil("setting1")
-       settings.veil("setting3", 1)
-       settings.veil("setting3", "key")
-   
-   Result print(settings()):
-
-       "setting1": "674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d"
-       "setting3": "value1", "674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d"
-       "setting3": {"key": "674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d"}
-
-7. .unveil(value):
-    Allows to decrypt veiled(encrypted) values. Value must be already present in instance (by .create or .load).
-    Example:
-
-       settings.unveil(settings()["setting1"])
-       settings.unveil(settings()["setting3"][1])
-       settings.unveil(settings()["setting3"]["key"])
-
-8. .save(verbose=False):
-    Saves all parameters created to file. Prints result of operation (success/failure) if verbose parameter has been given.
-
-9. .load(verbose=False):
-    Loads json formatted settings from file. Prints result of operation (success/failure) if verbose parameter has been given.
-
-
-
-   
+Module for creating parameters, saving them and loading from JSON formatted file.
+
+    pip install conson
+
+    from .conson import Conson
+
+Usage:
+
+1. Conson(cfile="config.json", cfilepath=os.getcwd(), salt="ch4ng3M3pl3453"):
+    You can set file name/extension and path to config file directory. By default, current working directory is used.
+
+2. Instance call, parameters:
+   Calling Conson instance will return all kwargs that has already been set by create method.
+   Values modified with .veil method will be encrypted and presented in hex value.
+   Parameters:
+
+        <instance>.file
+        <instance>.file = <filename>, <cfilepath=os.getcwd()>
+
+        <instance>.salt
+        <instance>.salt = <your salt>
+
+3. .create(key, *value): 
+    Creates parameter in key=value pair. Accepts single value or list of values.
+    Example:
+
+        settings = Conson()
+
+        settings.create(key1, value1, value2, value3)
+        settings.create(key2, [value1, value2, value3])
+        settings.create(key3, {"subkey1": "value1", "subkey2": value2, "subkey3": value3})
+
+4. .dispose(key):
+    Removes created parameter from instance.
+
+5. .dump()
+    Removes all created parameters. Useful in case when only one instance is invoked and multiple configuration files
+    are being loaded - allows to prevent mixing parameters simply by dumping them out.
+
+6. .veil(key, index="0", marker=""):
+    Passes created value through Fernet SHA-256 encryption. We point the key and value index number.
+    Secret key is based on system-related UUID, so decryption is meant to happen only on device the encryption has place.
+    If you want to reach value in nested dictionary, you can use subkey OR it's subkey's index number.
+    You can also pass marker char (or chars) to put as first and last char of returned value, it will help with 
+    identifying veiled strings (you can combine unveil with slicing).
+       Example:
+
+          settings.veil("setting1", marker="$")
+          settings.veil("setting3", 1)
+          settings.veil("setting3", "key", "<>") 
+   
+      Result print(settings()):
+
+          "setting1": "$674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d$"
+          "setting3": "value1", "674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d"
+          "setting3": {"key": "<674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d>"}
+
+7. .unveil(value):
+    Allows to decrypt veiled(encrypted) values. Value must be already present in instance (by .create or .load).
+    Example:
+
+       settings.unveil(settings()["setting1"])
+       settings.unveil(settings()["setting3"][1])
+       settings.unveil(settings()["setting3"]["key"])
+
+8. .save(verbose=False):
+    Saves all parameters created to file. Prints result of operation (success/failure) if verbose parameter has been given.
+
+9. .load(verbose=False):
+    Loads json formatted settings from file. Prints result of operation (success/failure) if verbose parameter has been given.
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `conson-3.1.9/conson/conson.py` & `conson-3.2.1/conson/conson.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,214 @@
-import os
-import json
-from cryptography.fernet import Fernet
-import subprocess
-import hashlib
-
-green = "\033[92m"
-red = "\033[91m"
-reset = "\033[0m"
-
-
-class Conson:
-    """
-    Simple configuration file manager. Create parameters, save them to file in json format, load them back.
-    Methods: "create", "create_pwd", "unveil", "save", "load".
-    Default parameters: "self.file" - absolute path to config file,
-                        "self.clean_salt" - salt string value.
-    """
-    def __init__(self, cfile="config.json", cfilepath=os.getcwd(), salt="ch4ng3M3pl3453"):
-        """
-        You can specify configuration file name and location.
-        By default, config file is located in program working directory, named "config.json".
-        :param cfile: string, i.e. "name.json"
-        :param cfilepath: string, path to config file location (without file name)
-        :param salt: string, used for additional encryption hardening.
-        """
-        self.__fullpath = os.path.join(cfilepath, cfile)
-        self.__clean_salt = salt
-        self.__salt = bytes.fromhex("".join(hex(ord(char))[2:] for char in self.__clean_salt))
-
-    def __call__(self):
-        vardict = self.__dict__.copy()
-        del vardict["_Conson__fullpath"]
-        del vardict["_Conson__salt"]
-        del vardict["_Conson__clean_salt"]
-        return vardict
-
-    @property
-    def file(self):
-        return self.__fullpath
-
-    @file.setter
-    def file(self, filename, cfilepath=os.getcwd()):
-        self.__fullpath = os.path.join(cfilepath, filename)
-
-    @property
-    def salt(self):
-        return self.__clean_salt
-
-    @salt.setter
-    def salt(self, salt_value):
-        self.__clean_salt = salt_value
-        self.__salt = bytes.fromhex("".join(hex(ord(char))[2:] for char in self.__clean_salt))
-
-    def __check(self):
-        """
-        Checks if config file exists and has JSON-loadable format.
-        :return: bool
-        """
-        try:
-            with open(self.__fullpath, "r")as config:
-                return isinstance(json.load(config), dict)
-        except (FileNotFoundError, json.decoder.JSONDecodeError):
-            return False
-
-    def create(self, k, *v):
-        """
-        Creates parameter.
-        :param k: key name -> string
-        :param v: values -> string, list
-        """
-        if len(list(v)) > 1:
-            values = []
-            for val in v:
-                values.append(val)
-            v = values
-        else:
-            v = v[0]
-        setattr(self, k, v)
-
-    def dispose(self, key):
-        """
-        Deletes parameter key.
-        :param key: string -> key you want to remove.
-        """
-        delattr(self, key)
-
-    def dump(self):
-        """
-        Deletes all created parameters.
-        """
-        for attr in list(self()):
-            delattr(self, attr)
-
-    def __get_key(self):
-        """
-        Method used for obtaining system UUID for both nt and unix systems.
-        Allows to decrypt data only on system where it was encrypted.
-        :return: String
-        """
-        def create_key(key_input):
-            """
-            Extending 32 to 44 bytes using md5 salt, required by Fernet.
-            """
-            hard_key = (key_input[:16] + supersalt[16:32] + supersalt[:2] + supersalt[5:7] + key_input[7:9]
-                        + supersalt[16:18] + key_input[21:23] + key_input[29] + "=")
-            return hard_key.encode()
-
-        # Converting salt string into md5 hash
-        md5 = hashlib.md5()
-        md5.update(self.__salt)
-        supersalt = md5.hexdigest()
-
-        if os.name == "nt":     # Windows compatibility.
-            key = subprocess.check_output(['wmic', 'csproduct', 'get', 'UUID'], text=True) \
-                .strip().splitlines()[2].replace("-", "")
-
-            return create_key(key)
-        elif os.name != "nt":   # Linux/UNIX compatibility.
-            key = subprocess.check_output(['dmidecode', '-s', 'system-uuid'], text=True) \
-                .strip().replace("-", "")
-            return create_key(key)
-
-    def veil(self, key, index="0"):
-        """
-        Encrypts created parameter.
-        E.g.: for
-        <instance>.create(pc1=["login", "password"])
-        encrypting "password will be:
-        <instance>.veil("pc1", 1)
-        :param key: string -> key containing value you want to encrypt
-        :param index: string -> value index number(list) or key(dictionary)
-        """
-        values = self()[key]
-        if isinstance(values, list):
-            encrypted = Fernet(self.__get_key()).encrypt(values[int(index)].encode()).hex()
-            values.pop(int(index))
-            values.insert(int(index), encrypted)
-            setattr(self, key, values)
-        elif isinstance(values, dict):
-            encrypted = Fernet(self.__get_key()).encrypt(values[index].encode()).hex()
-            values[index] = encrypted
-            setattr(self, key, values)
-        else:
-            encrypted = Fernet(self.__get_key()).encrypt(values.encode()).hex()
-            setattr(self, key, encrypted)
-
-    def unveil(self, encrypted_value):
-        """
-        Allows to decrypt values encrypted with create_pwd method.
-        :param encrypted_value: String containing hexadecimal number.
-        :return: String with decrypted password or "tooSalty".
-        """
-        try:
-            soup = Fernet(self.__get_key()).decrypt(bytes.fromhex(encrypted_value)).decode()
-        except Exception:
-            soup = "tooSalty"
-        return soup
-
-    def save(self, verbose=False):
-        """
-        Saves created parameters to file (default: config.json in working directory)
-        :param verbose: Any -> if not empty, prints result.
-        :return: string - saving result
-        """
-        try:
-            variables = {}
-            with open(self.__fullpath, "w") as config:
-                for k, v in self().items():
-                    if k != "fullpath":
-                        variables[k] = v
-                json.dump(variables, config, indent=4)
-            if verbose:
-                print("{}CONFIG SAVE SUCCESS!{}".format(green, reset))
-        except Exception as err:
-            if verbose:
-                print("{}CONFIG SAVE ERROR:{} {}".format(red, reset, err))
-
-    def load(self, verbose=False):
-        """
-        Loads parameters from file and passes them to instance.
-        :param verbose: Any -> if not empty, prints result.
-        :return: string - loading result
-        """
-        if self.__check():
-            with open(self.__fullpath, "r")as config:
-                variables = json.load(config)
-                for k, v in variables.items():
-                    setattr(self, k, v)
-                    if verbose:
-                        print("{}CONFIG READ SUCCESS{}".format(green, reset))
-        else:
-            if verbose:
-                print("{}CONFIG READ ERROR{}".format(red, reset))
+import os
+import json
+from cryptography.fernet import Fernet
+import subprocess
+import hashlib
+
+green = "\033[92m"
+red = "\033[91m"
+reset = "\033[0m"
+
+
+class Conson:
+    """
+    Simple configuration file manager. Create parameters, save them to file in json format, load them back.
+    Methods: "create", "create_pwd", "unveil", "save", "load".
+    Default parameters: "self.file" - absolute path to config file,
+                        "self.clean_salt" - salt string value.
+    """
+    def __init__(self, cfile="config.json", cfilepath=os.getcwd(), salt="ch4ng3M3pl3453"):
+        """
+        You can specify configuration file name and location.
+        By default, config file is located in program working directory, named "config.json".
+        :param cfile: string, i.e. "name.json"
+        :param cfilepath: string, path to config file location (without file name)
+        :param salt: string, used for additional encryption hardening.
+        """
+        self.__fullpath = os.path.join(cfilepath, cfile)
+        self.__clean_salt = salt
+        self.__salt = bytes.fromhex("".join(hex(ord(char))[2:] for char in self.__clean_salt))
+
+    def __call__(self):
+        vardict = self.__dict__.copy()
+        del vardict["_Conson__fullpath"]
+        del vardict["_Conson__salt"]
+        del vardict["_Conson__clean_salt"]
+        return vardict
+
+    @property
+    def file(self):
+        return self.__fullpath
+
+    @file.setter
+    def file(self, filename, cfilepath=os.getcwd()):
+        self.__fullpath = os.path.join(cfilepath, filename)
+
+    @property
+    def salt(self):
+        return self.__clean_salt
+
+    @salt.setter
+    def salt(self, salt_value):
+        self.__clean_salt = salt_value
+        self.__salt = bytes.fromhex("".join(hex(ord(char))[2:] for char in self.__clean_salt))
+
+    def __check(self):
+        """
+        Checks if config file exists and has JSON-loadable format.
+        :return: bool
+        """
+        try:
+            with open(self.__fullpath, "r")as config:
+                return isinstance(json.load(config), dict)
+        except (FileNotFoundError, json.decoder.JSONDecodeError):
+            return False
+
+    def create(self, k, *v):
+        """
+        Creates parameter.
+        :param k: key name -> string
+        :param v: values -> string, list
+        """
+        if len(list(v)) > 1:
+            values = []
+            for val in v:
+                values.append(val)
+            v = values
+        else:
+            v = v[0]
+        setattr(self, k, v)
+
+    def dispose(self, key):
+        """
+        Deletes parameter key.
+        :param key: string -> key you want to remove.
+        """
+        delattr(self, key)
+
+    def dump(self):
+        """
+        Deletes all created parameters.
+        """
+        for attr in list(self()):
+            delattr(self, attr)
+
+    def __get_key(self):
+        """
+        Method used for obtaining system UUID for both nt and unix systems.
+        Allows to decrypt data only on system where it was encrypted.
+        :return: String
+        """
+        def create_key(key_input):
+            """
+            Extending 32 to 44 bytes using md5 salt, required by Fernet.
+            """
+            hard_key = (key_input[:16] + supersalt[16:32] + supersalt[:2] + supersalt[5:7] + key_input[7:9]
+                        + supersalt[16:18] + key_input[21:23] + key_input[29] + "=")
+            return hard_key.encode()
+
+        # Converting salt string into md5 hash
+        md5 = hashlib.md5()
+        md5.update(self.__salt)
+        supersalt = md5.hexdigest()
+
+        if os.name == "nt":     # Windows compatibility.
+            key = subprocess.check_output(['wmic', 'csproduct', 'get', 'UUID'], text=True) \
+                .strip().splitlines()[2].replace("-", "")
+
+            return create_key(key)
+        elif os.name != "nt":   # Linux/UNIX compatibility.
+            key = subprocess.check_output(['cat', '/sys/class/dmi/id/product_uuid'], text=True) \
+                .strip().replace("-", "")
+            return create_key(key)
+
+    def veil(self, key, index="0", marker=""):
+        """
+        Encrypts created parameter.
+        E.g.: for
+        <instance>.create(pc1=["login", "password"])
+        encrypting "password will be:
+        <instance>.veil("pc1", 1)
+        For dictionary value you can use either subkey or its index.
+        :param key: string -> key containing value you want to encrypt
+        :param index: string -> value index number(list) or key(dictionary)
+        :param marker: String -> String with desired markers to put at beginning and end of veiled string. Single or
+        multiple chars can be used. Multiple chars will be split into half;
+        for uneven length - first char, content, rest of chars.
+        """
+        def mark(content, chars):
+            if len(marker) == 0:
+                return content
+            elif len(chars) == 1:
+                return chars + content + chars
+            elif len(chars) > 1:
+                if len(chars) % 2 == 0:
+                    mid = len(chars) // 2
+                    return chars[:mid] + content + chars[mid:]
+                else:
+                    return chars[:1] + content + chars[1:]
+
+        values = self()[key]
+        if isinstance(values, list):
+            encrypted = Fernet(self.__get_key()).encrypt(values[int(index)].encode()).hex()
+            values.pop(int(index))
+            values.insert(int(index), mark(encrypted, marker))
+            setattr(self, key, values)
+        elif isinstance(values, dict):
+            if index.isnumeric():
+                encrypted = Fernet(self.__get_key()).encrypt(values[list(values)[int(index)]].encode()).hex()
+                values[list(values)[int(index)]] = mark(encrypted, marker)
+            else:
+                encrypted = Fernet(self.__get_key()).encrypt(values[index].encode()).hex()
+                values[index] = mark(encrypted, marker)
+            setattr(self, key, values)
+        else:
+            encrypted = Fernet(self.__get_key()).encrypt(values.encode()).hex()
+            setattr(self, key, mark(encrypted, marker))
+
+    def unveil(self, encrypted_value):
+        """
+        Allows to decrypt values encrypted with create_pwd method.
+        :param encrypted_value: String containing hexadecimal number.
+        :return: String with decrypted password or "tooSalty".
+        """
+        try:
+            soup = Fernet(self.__get_key()).decrypt(bytes.fromhex(encrypted_value)).decode()
+        except Exception:
+            soup = "tooSalty"
+        return soup
+
+    def save(self, verbose=False):
+        """
+        Saves created parameters to file (default: config.json in working directory)
+        :param verbose: Any -> if not empty, prints result.
+        :return: string - saving result
+        """
+        try:
+            variables = {}
+            with open(self.__fullpath, "w") as config:
+                for k, v in self().items():
+                    if k != "fullpath":
+                        variables[k] = v
+                json.dump(variables, config, indent=4)
+            if verbose:
+                print("{}CONFIG SAVE SUCCESS!{}".format(green, reset))
+        except Exception as err:
+            if verbose:
+                print("{}CONFIG SAVE ERROR:{} {}".format(red, reset, err))
+
+    def load(self, verbose=False):
+        """
+        Loads parameters from file and passes them to instance.
+        :param verbose: Any -> if not empty, prints result.
+        :return: string - loading result
+        """
+        if self.__check():
+            with open(self.__fullpath, "r")as config:
+                variables = json.load(config)
+                for k, v in variables.items():
+                    setattr(self, k, v)
+                    if verbose:
+                        print("{}CONFIG READ SUCCESS{}".format(green, reset))
+        else:
+            if verbose:
+                print("{}CONFIG READ ERROR{}".format(red, reset))
```

### Comparing `conson-3.1.9/conson.egg-info/PKG-INFO` & `conson-3.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,84 @@
-Metadata-Version: 2.1
-Name: conson
-Version: 3.1.9
-Summary: A simple json configuration file manager
-Author: Paweł Gabryś
-Author-email: p.gabrys@int.pl
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: cryptography>=41.0.3
-
-Module for creating parameters, saving them and loading from JSON formatted file.
-
-    pip install conson
-
-    from .conson import Conson
-
-Usage:
-
-1. Conson(cfile="config.json", cfilepath=os.getcwd(), salt="ch4ng3M3pl3453"):
-    You can set file name/extension and path to config file directory. By default, current working directory is used.
-
-2. Instance call, parameters:
-   Calling Conson instance will return all kwargs that has already been set by create method.
-   Values modified with .veil method will be encrypted and presented in hex value.
-   Parameters:
-
-        <instance>.file
-        <instance>.file = <filename>, <cfilepath=os.getcwd()>
-
-        <instance>.salt
-        <instance>.salt = <your salt>
-
-3. .create(key, *value): 
-    Creates parameter in key=value pair. Accepts single value or list of values.
-    Example:
-
-        settings = Conson()
-
-        settings.create(key1, value1, value2, value3)
-        settings.create(key2, [value1, value2, value3])
-        settings.create(key3, {"subkey1": "value1", "subkey2": value2, "subkey3": value3})
-
-4. .dispose(key):
-    Removes created parameter from instance.
-
-5. .dump()
-    Removes all created parameters. Useful in case when only one instance is invoked and multiple configuration files
-    are being loaded - allows to prevent mixing parameters simply by dumping them out.
-
-6. .veil(key, index="0"):
-    Passes created value through Fernet SHA-256 encryption. We point the key and value index number.
-    Secret key is based on system-related UUID, so decryption is meant to happen only on device the encryption has place.
-    Example:
-
-       settings.veil("setting1")
-       settings.veil("setting3", 1)
-       settings.veil("setting3", "key")
-   
-   Result print(settings()):
-
-       "setting1": "674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d"
-       "setting3": "value1", "674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d"
-       "setting3": {"key": "674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d"}
-
-7. .unveil(value):
-    Allows to decrypt veiled(encrypted) values. Value must be already present in instance (by .create or .load).
-    Example:
-
-       settings.unveil(settings()["setting1"])
-       settings.unveil(settings()["setting3"][1])
-       settings.unveil(settings()["setting3"]["key"])
-
-8. .save(verbose=False):
-    Saves all parameters created to file. Prints result of operation (success/failure) if verbose parameter has been given.
-
-9. .load(verbose=False):
-    Loads json formatted settings from file. Prints result of operation (success/failure) if verbose parameter has been given.
-
-
-
-   
+Metadata-Version: 2.1
+Name: conson
+Version: 3.2.1
+Summary: A simple json configuration file manager
+Author: Paweł Gabryś
+Author-email: p.gabrys@int.pl
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: cryptography>=41.0.3
+
+Module for creating parameters, saving them and loading from JSON formatted file.
+
+    pip install conson
+
+    from .conson import Conson
+
+Usage:
+
+1. Conson(cfile="config.json", cfilepath=os.getcwd(), salt="ch4ng3M3pl3453"):
+    You can set file name/extension and path to config file directory. By default, current working directory is used.
+
+2. Instance call, parameters:
+   Calling Conson instance will return all kwargs that has already been set by create method.
+   Values modified with .veil method will be encrypted and presented in hex value.
+   Parameters:
+
+        <instance>.file
+        <instance>.file = <filename>, <cfilepath=os.getcwd()>
+
+        <instance>.salt
+        <instance>.salt = <your salt>
+
+3. .create(key, *value): 
+    Creates parameter in key=value pair. Accepts single value or list of values.
+    Example:
+
+        settings = Conson()
+
+        settings.create(key1, value1, value2, value3)
+        settings.create(key2, [value1, value2, value3])
+        settings.create(key3, {"subkey1": "value1", "subkey2": value2, "subkey3": value3})
+
+4. .dispose(key):
+    Removes created parameter from instance.
+
+5. .dump()
+    Removes all created parameters. Useful in case when only one instance is invoked and multiple configuration files
+    are being loaded - allows to prevent mixing parameters simply by dumping them out.
+
+6. .veil(key, index="0", marker=""):
+    Passes created value through Fernet SHA-256 encryption. We point the key and value index number.
+    Secret key is based on system-related UUID, so decryption is meant to happen only on device the encryption has place.
+    If you want to reach value in nested dictionary, you can use subkey OR it's subkey's index number.
+    You can also pass marker char (or chars) to put as first and last char of returned value, it will help with 
+    identifying veiled strings (you can combine unveil with slicing).
+       Example:
+
+          settings.veil("setting1", marker="$")
+          settings.veil("setting3", 1)
+          settings.veil("setting3", "key", "<>") 
+   
+      Result print(settings()):
+
+          "setting1": "$674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d$"
+          "setting3": "value1", "674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d"
+          "setting3": {"key": "<674141414141426c65566a6c6123123330617a41416c6330307a3667794a41535965537733423sdvb347705f464a5648435a39596b586a45304b31506232646b645353355f2d4c4646623546fggf3395a6c4e38595f7358676269513d3d>"}
+
+7. .unveil(value):
+    Allows to decrypt veiled(encrypted) values. Value must be already present in instance (by .create or .load).
+    Example:
+
+       settings.unveil(settings()["setting1"])
+       settings.unveil(settings()["setting3"][1])
+       settings.unveil(settings()["setting3"]["key"])
+
+8. .save(verbose=False):
+    Saves all parameters created to file. Prints result of operation (success/failure) if verbose parameter has been given.
+
+9. .load(verbose=False):
+    Loads json formatted settings from file. Prints result of operation (success/failure) if verbose parameter has been given.
+
+
+
+
```

