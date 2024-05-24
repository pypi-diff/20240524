# Comparing `tmp/alibabacloud_credentials-0.3.1.tar.gz` & `tmp/alibabacloud_credentials-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_credentials-0.3.1.tar", last modified: Wed Feb  1 08:16:02 2023, max compression
+gzip compressed data, was "dist/alibabacloud_credentials-0.3.2.tar", last modified: Tue Feb 28 03:49:51 2023, max compression
```

## Comparing `alibabacloud_credentials-0.3.1.tar` & `alibabacloud_credentials-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:16:02.000000 alibabacloud_credentials-0.3.1/
--rw-r--r--   0 root         (0) root         (0)    15126 2023-02-01 08:16:02.000000 alibabacloud_credentials-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11914 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:16:02.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3463 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/client.py
--rw-r--r--   0 root         (0) root         (0)    14926 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/credentials.py
--rw-r--r--   0 root         (0) root         (0)      193 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6494 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/models.py
--rw-r--r--   0 root         (0) root         (0)    28469 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:16:02.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/utils/auth_constant.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/utils/auth_util.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials/utils/parameter_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:16:02.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15126 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      667 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/alibabacloud_credentials.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-01 08:16:02.000000 alibabacloud_credentials-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2351 2023-02-01 08:16:01.000000 alibabacloud_credentials-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)    15134 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11922 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/client.py
+-rw-r--r--   0 root         (0) root         (0)    14926 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/credentials.py
+-rw-r--r--   0 root         (0) root         (0)      193 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6494 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/models.py
+-rw-r--r--   0 root         (0) root         (0)    28952 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/utils/auth_constant.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/utils/auth_util.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials/utils/parameter_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15134 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      667 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/alibabacloud_credentials.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 03:49:51.000000 alibabacloud_credentials-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-02-28 03:49:50.000000 alibabacloud_credentials-0.3.2/setup.py
```

### Comparing `alibabacloud_credentials-0.3.1/PKG-INFO` & `alibabacloud_credentials-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_credentials
-Version: 0.3.1
+Version: 0.3.2
 Summary: The alibabacloud credentials module of alibabaCloud Python SDK.
 Home-page: https://github.com/aliyun/credentials-python
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -230,15 +230,15 @@
         
         1. Environment Credentials
         
         Look for environment credentials in environment variable. If the `ALIBABA_CLOUD_ACCESS_KEY_ID` and `ALIBABA_CLOUD_ACCESS_KEY_SECRET` environment variables are defined and are not empty, the program will use them to create default credentials.
         
         2. Credentials File
         
-        If there is `~/.alibabacloud/credentials default file (Windows shows C:\Users\USER_NAME\.alibabacloud\credentials)`, the program automatically creates credentials with the specified type and name. The default file is not necessarily exist, but a parse error will throw an exception. The name of configuration item is lowercase.This configuration file can be shared between different projects and between different tools. Because it is outside of the project and will not be accidentally committed to the version control. The path to the default file can be modified by defining the `ALIBABA_CLOUD_CREDENTIALS_FILE` environment variable. If not configured, use the default configuration `default`. You can also set the environment variables `ALIBABA_CLOUD_PROFILE` to use the configuration.
+        If there is `~/.alibabacloud/credentials.ini default file (Windows shows C:\Users\USER_NAME\.alibabacloud\credentials.ini)`, the program automatically creates credentials with the specified type and name. The default file is not necessarily exist, but a parse error will throw an exception. The name of configuration item is lowercase.This configuration file can be shared between different projects and between different tools. Because it is outside of the project and will not be accidentally committed to the version control. The path to the default file can be modified by defining the `ALIBABA_CLOUD_CREDENTIALS_FILE` environment variable. If not configured, use the default configuration `default`. You can also set the environment variables `ALIBABA_CLOUD_PROFILE` to use the configuration.
         
         ```ini
         [default]                          # default setting
         enable = true                      # Enable，Enabled by default if this option is not present
         type = access_key                  # Certification type: access_key
         access_key_id = foo                # Key
         access_key_secret = bar            # Secret
```

### Comparing `alibabacloud_credentials-0.3.1/README.md` & `alibabacloud_credentials-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 
 1. Environment Credentials
 
 Look for environment credentials in environment variable. If the `ALIBABA_CLOUD_ACCESS_KEY_ID` and `ALIBABA_CLOUD_ACCESS_KEY_SECRET` environment variables are defined and are not empty, the program will use them to create default credentials.
 
 2. Credentials File
 
-If there is `~/.alibabacloud/credentials default file (Windows shows C:\Users\USER_NAME\.alibabacloud\credentials)`, the program automatically creates credentials with the specified type and name. The default file is not necessarily exist, but a parse error will throw an exception. The name of configuration item is lowercase.This configuration file can be shared between different projects and between different tools. Because it is outside of the project and will not be accidentally committed to the version control. The path to the default file can be modified by defining the `ALIBABA_CLOUD_CREDENTIALS_FILE` environment variable. If not configured, use the default configuration `default`. You can also set the environment variables `ALIBABA_CLOUD_PROFILE` to use the configuration.
+If there is `~/.alibabacloud/credentials.ini default file (Windows shows C:\Users\USER_NAME\.alibabacloud\credentials.ini)`, the program automatically creates credentials with the specified type and name. The default file is not necessarily exist, but a parse error will throw an exception. The name of configuration item is lowercase.This configuration file can be shared between different projects and between different tools. Because it is outside of the project and will not be accidentally committed to the version control. The path to the default file can be modified by defining the `ALIBABA_CLOUD_CREDENTIALS_FILE` environment variable. If not configured, use the default configuration `default`. You can also set the environment variables `ALIBABA_CLOUD_PROFILE` to use the configuration.
 
 ```ini
 [default]                          # default setting
 enable = true                      # Enable，Enabled by default if this option is not present
 type = access_key                  # Certification type: access_key
 access_key_id = foo                # Key
 access_key_secret = bar            # Secret
```

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials/client.py` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials/credentials.py` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials/models.py` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials/providers.py` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,16 +485,23 @@
         self._set_arg('file_path', path)
 
     def parse_ini(self):
         file_path = self.file_path if self.file_path else au.environment_credentials_file
         if file_path is None:
             if not ac.HOME:
                 return
-            file_path = os.path.join(ac.HOME, "/.alibabacloud/credentials.ini")
-        if len(file_path) == 0:
+            if os.path.exists(os.path.join(ac.HOME, "/.alibabacloud/credentials.ini")):
+                # Support '/.alibabacloud/credentials.ini' is due to historical mistakes.
+                # Please try to use '~/.alibabacloud/credentials.ini'.
+                file_path = os.path.join(ac.HOME, "/.alibabacloud/credentials.ini")
+            elif os.path.exists(os.path.join(ac.HOME, ".alibabacloud/credentials.ini")):
+                file_path = os.path.join(ac.HOME, ".alibabacloud/credentials.ini")
+        if file_path is None:
+            return
+        elif len(file_path) == 0:
             raise CredentialException("The specified credentials file is empty")
 
         # loads ini
         conf = configparser.ConfigParser()
         conf.read(file_path, encoding='utf-8')
         ini_map = dict(conf._sections)
         for k in dict(conf._sections):
```

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials/utils/auth_constant.py` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials/utils/auth_constant.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials/utils/auth_util.py` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials/utils/auth_util.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials/utils/parameter_helper.py` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials/utils/parameter_helper.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials.egg-info/PKG-INFO` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-credentials
-Version: 0.3.1
+Version: 0.3.2
 Summary: The alibabacloud credentials module of alibabaCloud Python SDK.
 Home-page: https://github.com/aliyun/credentials-python
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -230,15 +230,15 @@
         
         1. Environment Credentials
         
         Look for environment credentials in environment variable. If the `ALIBABA_CLOUD_ACCESS_KEY_ID` and `ALIBABA_CLOUD_ACCESS_KEY_SECRET` environment variables are defined and are not empty, the program will use them to create default credentials.
         
         2. Credentials File
         
-        If there is `~/.alibabacloud/credentials default file (Windows shows C:\Users\USER_NAME\.alibabacloud\credentials)`, the program automatically creates credentials with the specified type and name. The default file is not necessarily exist, but a parse error will throw an exception. The name of configuration item is lowercase.This configuration file can be shared between different projects and between different tools. Because it is outside of the project and will not be accidentally committed to the version control. The path to the default file can be modified by defining the `ALIBABA_CLOUD_CREDENTIALS_FILE` environment variable. If not configured, use the default configuration `default`. You can also set the environment variables `ALIBABA_CLOUD_PROFILE` to use the configuration.
+        If there is `~/.alibabacloud/credentials.ini default file (Windows shows C:\Users\USER_NAME\.alibabacloud\credentials.ini)`, the program automatically creates credentials with the specified type and name. The default file is not necessarily exist, but a parse error will throw an exception. The name of configuration item is lowercase.This configuration file can be shared between different projects and between different tools. Because it is outside of the project and will not be accidentally committed to the version control. The path to the default file can be modified by defining the `ALIBABA_CLOUD_CREDENTIALS_FILE` environment variable. If not configured, use the default configuration `default`. You can also set the environment variables `ALIBABA_CLOUD_PROFILE` to use the configuration.
         
         ```ini
         [default]                          # default setting
         enable = true                      # Enable，Enabled by default if this option is not present
         type = access_key                  # Certification type: access_key
         access_key_id = foo                # Key
         access_key_secret = bar            # Secret
```

### Comparing `alibabacloud_credentials-0.3.1/alibabacloud_credentials.egg-info/SOURCES.txt` & `alibabacloud_credentials-0.3.2/alibabacloud_credentials.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_credentials-0.3.1/setup.py` & `alibabacloud_credentials-0.3.2/setup.py`

 * *Files identical despite different names*

