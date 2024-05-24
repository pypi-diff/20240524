# Comparing `tmp/DNA_SE-0.1.0.tar.gz` & `tmp/dna_se-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DNA_SE-0.1.0.tar", last modified: Fri May 24 06:01:03 2024, max compression
+gzip compressed data, was "dna_se-0.1.1.tar", last modified: Fri May 24 06:20:59 2024, max compression
```

## Comparing `DNA_SE-0.1.0.tar` & `dna_se-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/
-drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/DNA_SE/
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     6251 2024-05-23 19:16:22.000000 DNA_SE-0.1.0/DNA_SE/DNA_SE.py
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)       25 2024-05-08 12:46:34.000000 DNA_SE-0.1.0/DNA_SE/__init__.py
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      208 2024-05-23 18:18:05.000000 DNA_SE-0.1.0/DNA_SE/image.py
-drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/DNA_SE.egg-info/
--rw-r--r--   0 qsliu     (1003) qsliu     (1003)     5202 2024-05-24 06:01:03.000000 DNA_SE-0.1.0/DNA_SE.egg-info/PKG-INFO
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      202 2024-05-24 06:01:03.000000 DNA_SE-0.1.0/DNA_SE.egg-info/SOURCES.txt
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)        1 2024-05-24 06:01:03.000000 DNA_SE-0.1.0/DNA_SE.egg-info/dependency_links.txt
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)        7 2024-05-24 06:01:03.000000 DNA_SE-0.1.0/DNA_SE.egg-info/top_level.txt
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     1091 2024-05-08 12:46:34.000000 DNA_SE-0.1.0/LICENSE.txt
--rw-r--r--   0 qsliu     (1003) qsliu     (1003)     5202 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/PKG-INFO
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     4783 2024-05-09 08:11:12.000000 DNA_SE-0.1.0/README.md
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)       38 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/setup.cfg
--rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      686 2024-05-24 06:00:00.000000 DNA_SE-0.1.0/setup.py
+drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:20:59.833136 dna_se-0.1.1/
+drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:20:59.833136 dna_se-0.1.1/DNA_SE/
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     6277 2024-05-24 06:20:11.000000 dna_se-0.1.1/DNA_SE/DNA_SE.py
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)       25 2024-05-08 12:46:34.000000 dna_se-0.1.1/DNA_SE/__init__.py
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      208 2024-05-23 18:18:05.000000 dna_se-0.1.1/DNA_SE/image.py
+drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:20:59.833136 dna_se-0.1.1/DNA_SE.egg-info/
+-rw-r--r--   0 qsliu     (1003) qsliu     (1003)     5202 2024-05-24 06:20:59.000000 dna_se-0.1.1/DNA_SE.egg-info/PKG-INFO
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      202 2024-05-24 06:20:59.000000 dna_se-0.1.1/DNA_SE.egg-info/SOURCES.txt
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)        1 2024-05-24 06:20:59.000000 dna_se-0.1.1/DNA_SE.egg-info/dependency_links.txt
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)        7 2024-05-24 06:20:59.000000 dna_se-0.1.1/DNA_SE.egg-info/top_level.txt
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     1091 2024-05-08 12:46:34.000000 dna_se-0.1.1/LICENSE.txt
+-rw-r--r--   0 qsliu     (1003) qsliu     (1003)     5202 2024-05-24 06:20:59.833136 dna_se-0.1.1/PKG-INFO
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     4783 2024-05-09 08:11:12.000000 dna_se-0.1.1/README.md
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)       38 2024-05-24 06:20:59.833136 dna_se-0.1.1/setup.cfg
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      686 2024-05-24 06:20:37.000000 dna_se-0.1.1/setup.py
```

### Comparing `DNA_SE-0.1.0/DNA_SE/DNA_SE.py` & `dna_se-0.1.1/DNA_SE/DNA_SE.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,31 +133,31 @@
 
     if esti_mask == 1:
         return model_b, beta.data()
     else:
         return model_b
 
 # a simple example
-p = 1
-Oi = torch.rand(1000,1)
-BATCHSIZE = 100
-EPOCH = 200
-M = 1000
-B = 10000
-input_dim = 1
-output_dim = 1
-hidden_dim = 5
-depth = 2
-ones_B = torch.ones(BATCHSIZE,1).to(torch.device('cuda' if torch.cuda.is_available() else 'cpu'))
+# p = 1
+# Oi = torch.rand(1000,1)
+# BATCHSIZE = 100
+# EPOCH = 200
+# M = 1000
+# B = 10000
+# input_dim = 1
+# output_dim = 1
+# hidden_dim = 5
+# depth = 2
+# ones_B = torch.ones(M,1).to(torch.device('cuda' if torch.cuda.is_available() else 'cpu'))
 
-def K_func(x,y,Oi,b):
-    return y * torch.kron(ones_B,x).reshape(BATCHSIZE,M)
-def C_func(x,Oi,b):
-    return -torch.exp(x)
-output = dna(p, Oi, BATCHSIZE, EPOCH, M, B, input_dim, hidden_dim, output_dim, K_func, C_func, depth)
-print(output)
+# def K_func(x,y,Oi,b):
+#     return y * torch.kron(ones_B,x).reshape(BATCHSIZE,M)
+# def C_func(x,Oi,b):
+#     return -torch.exp(x)
+# output = dna(p, Oi, BATCHSIZE, EPOCH, M, B, input_dim, hidden_dim, output_dim, K_func, C_func, depth)
+# print(output)
 
 '''
 beta.data() is used to get the value of beta
 '''
 
 # Path: DNA-SE/package/DNA_SE/DNA_SE.py
```

### Comparing `DNA_SE-0.1.0/DNA_SE.egg-info/PKG-INFO` & `dna_se-0.1.1/DNA_SE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: DNA-SE
-Version: 0.1.0
+Name: DNA_SE
+Version: 0.1.1
 Summary: A small example package
 Home-page: https://github.com/liuqs111/DNA-SE
 Author: Qinshuo
 Author-email: u3008680@connect.hku.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DNA_SE-0.1.0/LICENSE.txt` & `dna_se-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DNA_SE-0.1.0/PKG-INFO` & `dna_se-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DNA_SE
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small example package
 Home-page: https://github.com/liuqs111/DNA-SE
 Author: Qinshuo
 Author-email: u3008680@connect.hku.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DNA_SE-0.1.0/README.md` & `dna_se-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `DNA_SE-0.1.0/setup.py` & `dna_se-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DNA_SE", # Replace with your own username
-    version="0.1.0",
+    version="0.1.1",
     author="Qinshuo",
     author_email="u3008680@connect.hku.hk",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liuqs111/DNA-SE",
     packages=setuptools.find_packages(),
```

