# Comparing `tmp/lgw-1.2.2.tar.gz` & `tmp/lgw-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lgw-1.2.2.tar", last modified: Wed Jun 10 13:20:31 2020, max compression
+gzip compressed data, was "lgw-1.2.3.tar", max compression
```

## Comparing `lgw-1.2.2.tar` & `lgw-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    11357 2019-12-01 20:32:22.000000 lgw-1.2.2/LICENSE
--rw-r--r--   0        0        0     8974 2020-06-10 13:19:22.335463 lgw-1.2.2/README.md
--rw-r--r--   0        0        0       36 2019-12-01 20:32:22.000000 lgw-1.2.2/lgw/__init__.py
--rw-r--r--   0        0        0     5773 2020-05-09 21:51:33.363654 lgw-1.2.2/lgw/api_gateway.py
--rw-r--r--   0        0        0     3585 2019-12-06 01:21:30.000000 lgw-1.2.2/lgw/api_gateway_domain.py
--rw-r--r--   0        0        0     5805 2020-05-09 02:48:15.347577 lgw-1.2.2/lgw/lambda_bundle.py
--rw-r--r--   0        0        0     8764 2020-06-10 13:19:22.335837 lgw-1.2.2/lgw/lambda_util.py
--rw-r--r--   0        0        0     8717 2020-06-10 13:19:22.336160 lgw-1.2.2/lgw/main.py
--rw-r--r--   0        0        0     2283 2020-05-11 10:48:51.680802 lgw-1.2.2/lgw/route53.py
--rw-r--r--   0        0        0      478 2019-12-01 20:32:22.000000 lgw-1.2.2/lgw/s3.py
--rw-r--r--   0        0        0     1402 2020-06-10 13:19:22.336412 lgw-1.2.2/lgw/settings.py
--rw-r--r--   0        0        0      284 2019-12-01 20:32:22.000000 lgw-1.2.2/lgw/util.py
--rw-r--r--   0        0        0       22 2020-06-10 13:20:25.885482 lgw-1.2.2/lgw/version.py
--rw-r--r--   0        0        0     1175 2020-06-10 13:20:24.276888 lgw-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    10233 2020-06-10 13:20:31.594527 lgw-1.2.2/setup.py
--rw-r--r--   0        0        0     9857 2020-06-10 13:20:31.594962 lgw-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 13:59:06.775185 lgw-1.2.3/LICENSE
+-rw-r--r--   0        0        0     8974 2024-05-24 13:59:06.775859 lgw-1.2.3/README.md
+-rw-r--r--   0        0        0       36 2024-05-24 13:59:06.776063 lgw-1.2.3/lgw/__init__.py
+-rw-r--r--   0        0        0     5773 2024-05-24 13:59:06.776222 lgw-1.2.3/lgw/api_gateway.py
+-rw-r--r--   0        0        0     3585 2024-05-24 13:59:06.776367 lgw-1.2.3/lgw/api_gateway_domain.py
+-rw-r--r--   0        0        0     5805 2024-05-24 13:59:06.776634 lgw-1.2.3/lgw/lambda_bundle.py
+-rw-r--r--   0        0        0     8764 2024-05-24 13:59:06.776803 lgw-1.2.3/lgw/lambda_util.py
+-rw-r--r--   0        0        0     8717 2024-05-24 13:59:06.776949 lgw-1.2.3/lgw/main.py
+-rw-r--r--   0        0        0     2283 2024-05-24 13:59:06.777091 lgw-1.2.3/lgw/route53.py
+-rw-r--r--   0        0        0      478 2024-05-24 13:59:06.777234 lgw-1.2.3/lgw/s3.py
+-rw-r--r--   0        0        0     1402 2024-05-24 13:59:06.777425 lgw-1.2.3/lgw/settings.py
+-rw-r--r--   0        0        0      284 2024-05-24 13:59:06.777777 lgw-1.2.3/lgw/util.py
+-rw-r--r--   0        0        0       22 2024-05-24 15:14:25.306300 lgw-1.2.3/lgw/version.py
+-rw-r--r--   0        0        0     1227 2024-05-24 15:14:17.946984 lgw-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    10056 1970-01-01 00:00:00.000000 lgw-1.2.3/PKG-INFO
```

### Comparing `lgw-1.2.2/LICENSE` & `lgw-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/README.md` & `lgw-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/lgw/api_gateway.py` & `lgw-1.2.3/lgw/api_gateway.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/lgw/api_gateway_domain.py` & `lgw-1.2.3/lgw/api_gateway_domain.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/lgw/lambda_bundle.py` & `lgw-1.2.3/lgw/lambda_bundle.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/lgw/lambda_util.py` & `lgw-1.2.3/lgw/lambda_util.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/lgw/main.py` & `lgw-1.2.3/lgw/main.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/lgw/route53.py` & `lgw-1.2.3/lgw/route53.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/lgw/settings.py` & `lgw-1.2.3/lgw/settings.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.2/pyproject.toml` & `lgw-1.2.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "lgw"
-version = "1.2.2"
+version = "1.2.3"
 description = "Configure an AWS Gateway in front of a Lambda function."
 authors = ["Edward Q. Bridges <ebridges@roja.cc>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ebridges/lgw"
 documentation = "https://github.com/ebridges/lgw/blob/master/README.md"
 classifiers = ["Topic :: Software Development :: Build Tools"]
 exclude = ["tests", "vscode.env", "NOTES.md"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.8,<4.0"
 docopt = "^0.6.2"
 everett = "^1.0"
 boto3 = "^1.10"
 docker = "^4.1"
-python-dotenv = "^0.10.3"
+python-dotenv = "^1"
 tld = "^0.12.1"
+moto = {version = "^5.0.7", extras = ["lambda", "apigateway"]}
 
 [tool.poetry.dev-dependencies]
 black = {version = "^19.3b0", allow-prereleases = true}
-pytest = "^3.0"
+pytest = "^8"
 pre-commit = "^1.20"
-moto = { git = "https://github.com/spulec/moto.git", branch = "master" }
+moto = {version = "^5.0.7", extras = ["lambda", "apigateway"]}
 assertpy = "^0.15.0"
 
 [tool.poetry.scripts]
 lgw = 'lgw.main:main'
 
 [tool.black]
 line-length = 100
```

### Comparing `lgw-1.2.2/PKG-INFO` & `lgw-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: lgw
-Version: 1.2.2
+Version: 1.2.3
 Summary: Configure an AWS Gateway in front of a Lambda function.
 Home-page: https://github.com/ebridges/lgw
 License: Apache-2.0
 Author: Edward Q. Bridges
 Author-email: ebridges@roja.cc
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: boto3 (>=1.10,<2.0)
 Requires-Dist: docker (>=4.1,<5.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: everett (>=1.0,<2.0)
-Requires-Dist: python-dotenv (>=0.10.3,<0.11.0)
+Requires-Dist: moto[apigateway,lambda] (>=5.0.7,<6.0.0)
+Requires-Dist: python-dotenv (>=1,<2)
 Requires-Dist: tld (>=0.12.1,<0.13.0)
 Project-URL: Documentation, https://github.com/ebridges/lgw/blob/master/README.md
 Description-Content-Type: text/markdown
 
 [![PyPi License](https://img.shields.io/pypi/l/lgw?color=blue)](https://github.com/ebridges/lgw/blob/master/LICENSE)
 [![PyPi](https://img.shields.io/pypi/v/lgw.svg?style=flat-square)](https://pypi.org/project/lgw/)
```

#### html2text {}

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1 Name: lgw Version: 1.2.2 Summary: Configure an AWS
+Metadata-Version: 2.1 Name: lgw Version: 1.2.3 Summary: Configure an AWS
 Gateway in front of a Lambda function. Home-page: https://github.com/ebridges/
 lgw License: Apache-2.0 Author: Edward Q. Bridges Author-email:
-ebridges@roja.cc Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
+ebridges@roja.cc Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Topic :: Software Development :: Build
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Software Development :: Build
 Tools Requires-Dist: boto3 (>=1.10,<2.0) Requires-Dist: docker (>=4.1,<5.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0) Requires-Dist: everett (>=1.0,<2.0)
-Requires-Dist: python-dotenv (>=0.10.3,<0.11.0) Requires-Dist: tld
-(>=0.12.1,<0.13.0) Project-URL: Documentation, https://github.com/ebridges/lgw/
-blob/master/README.md Description-Content-Type: text/markdown [![PyPi License]
-(https://img.shields.io/pypi/l/lgw?color=blue)](https://github.com/ebridges/
-lgw/blob/master/LICENSE) [![PyPi](https://img.shields.io/pypi/v/
-lgw.svg?style=flat-square)](https://pypi.org/project/lgw/) # Lambda Gateway
-Configure an AWS Gateway in front of a Lambda function. ## Usage ``` Lambda
-Gateway. Usage: lgw gw-deploy [--verbose] [--config-file=] lgw gw-undeploy [--
-verbose] [--config-file=] lgw domain-add [--verbose] [--config-file=] lgw
-domain-remove [--verbose] [--config-file=] lgw lambda-deploy [--verbose] [--
-config-file=] [--lambda-file=] lgw lambda-invoke [--verbose] --lambda-name= [--
-payload=] lgw lambda-delete [--verbose] --lambda-name= lgw lambda-archive [--
-verbose] [--config-file=] Options: -h --help Show this screen. --version Show
-version. --verbose Enable DEBUG-level logging. --config-file= Override defaults
-with these settings. --lambda-file= Path to zip file with executable lambda
-code. --lambda-name= Name of the lambda to invoke or delete. --payload= Path to
-a file of type json with data to send with the lambda invocation. ``` ##
-Configuration Parameters Configuration params are read in the following order,
-with the first read of it overriding subsequent configs: 1. Read from
-environment. 2. Read from `.env` file in current folder. 3. Read from flat file
-named via `--config-file` CLI param. 4. Read from `lgw.settings.defaults()`
-Defaults are configured in `lgw.settings`.
+Requires-Dist: moto[apigateway,lambda] (>=5.0.7,<6.0.0) Requires-Dist: python-
+dotenv (>=1,<2) Requires-Dist: tld (>=0.12.1,<0.13.0) Project-URL:
+Documentation, https://github.com/ebridges/lgw/blob/master/README.md
+Description-Content-Type: text/markdown [![PyPi License](https://
+img.shields.io/pypi/l/lgw?color=blue)](https://github.com/ebridges/lgw/blob/
+master/LICENSE) [![PyPi](https://img.shields.io/pypi/v/lgw.svg?style=flat-
+square)](https://pypi.org/project/lgw/) # Lambda Gateway Configure an AWS
+Gateway in front of a Lambda function. ## Usage ``` Lambda Gateway. Usage: lgw
+gw-deploy [--verbose] [--config-file=] lgw gw-undeploy [--verbose] [--config-
+file=] lgw domain-add [--verbose] [--config-file=] lgw domain-remove [--
+verbose] [--config-file=] lgw lambda-deploy [--verbose] [--config-file=] [--
+lambda-file=] lgw lambda-invoke [--verbose] --lambda-name= [--payload=] lgw
+lambda-delete [--verbose] --lambda-name= lgw lambda-archive [--verbose] [--
+config-file=] Options: -h --help Show this screen. --version Show version. --
+verbose Enable DEBUG-level logging. --config-file= Override defaults with these
+settings. --lambda-file= Path to zip file with executable lambda code. --
+lambda-name= Name of the lambda to invoke or delete. --payload= Path to a file
+of type json with data to send with the lambda invocation. ``` ## Configuration
+Parameters Configuration params are read in the following order, with the first
+read of it overriding subsequent configs: 1. Read from environment. 2. Read
+from `.env` file in current folder. 3. Read from flat file named via `--config-
+file` CLI param. 4. Read from `lgw.settings.defaults()` Defaults are configured
+in `lgw.settings`.
 RReellaatteedd TTaasskk   KKeeyy                                 DDeessccrriippttiioonn                          DDeeffaauulltt
 ((ss))
     * All      AWS_REGION                          AWS region.                          us-east-1
     * gw-
       deploy
     * gw-
       undeploy AWS_API_NAME                        Name for the created API gateway.    N/A
```

