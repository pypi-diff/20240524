# Comparing `tmp/logbesselk-3.2.0.tar.gz` & `tmp/logbesselk-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logbesselk-3.2.0.tar", max compression
+gzip compressed data, was "logbesselk-3.2.1.tar", max compression
```

## Comparing `logbesselk-3.2.0.tar` & `logbesselk-3.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-01-21 18:09:13.662752 logbesselk-3.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2265 2023-01-21 18:09:13.662752 logbesselk-3.2.0/README.md
--rw-r--r--   0        0        0     2190 2023-01-21 18:09:13.678752 logbesselk-3.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-21 18:09:13.678752 logbesselk-3.2.0/src/logbesselk/__init__.py
--rw-r--r--   0        0        0      186 2023-01-21 18:09:13.678752 logbesselk-3.2.0/src/logbesselk/jax/__init__.py
--rw-r--r--   0        0        0     1826 2023-01-21 18:09:13.678752 logbesselk-3.2.0/src/logbesselk/jax/asymptotic.py
--rw-r--r--   0        0        0     1829 2023-01-21 18:09:13.678752 logbesselk-3.2.0/src/logbesselk/jax/cfraction.py
--rw-r--r--   0        0        0     2715 2023-01-21 18:09:13.678752 logbesselk-3.2.0/src/logbesselk/jax/integral.py
--rw-r--r--   0        0        0     1865 2023-01-21 18:09:13.678752 logbesselk-3.2.0/src/logbesselk/jax/math.py
--rw-r--r--   0        0        0      789 2023-01-21 18:09:13.678752 logbesselk-3.2.0/src/logbesselk/jax/misc.py
--rw-r--r--   0        0        0     1804 2023-01-21 18:09:13.678752 logbesselk-3.2.0/src/logbesselk/jax/sca.py
--rw-r--r--   0        0        0     2482 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/jax/series.py
--rw-r--r--   0        0        0     2375 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/jax/utils.py
--rw-r--r--   0        0        0     2457 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/jax/wrap.py
--rw-r--r--   0        0        0      186 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/__init__.py
--rw-r--r--   0        0        0     2017 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/asymptotic.py
--rw-r--r--   0        0        0     1944 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/cfraction.py
--rw-r--r--   0        0        0     2878 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/integral.py
--rw-r--r--   0        0        0     2218 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/math.py
--rw-r--r--   0        0        0      861 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/misc.py
--rw-r--r--   0        0        0     1890 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/sca.py
--rw-r--r--   0        0        0     2568 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/series.py
--rw-r--r--   0        0        0     3289 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/utils.py
--rw-r--r--   0        0        0     2202 2023-01-21 18:09:13.682752 logbesselk-3.2.0/src/logbesselk/tensorflow/wrap.py
--rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 logbesselk-3.2.0/setup.py
--rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 logbesselk-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 04:48:20.673878 logbesselk-3.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2265 2024-05-24 04:48:20.673878 logbesselk-3.2.1/README.md
+-rw-r--r--   0        0        0     2190 2024-05-24 04:48:20.689878 logbesselk-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/__init__.py
+-rw-r--r--   0        0        0     1826 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/asymptotic.py
+-rw-r--r--   0        0        0     1829 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/cfraction.py
+-rw-r--r--   0        0        0     2715 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/integral.py
+-rw-r--r--   0        0        0     1865 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/math.py
+-rw-r--r--   0        0        0      789 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/misc.py
+-rw-r--r--   0        0        0     1804 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/sca.py
+-rw-r--r--   0        0        0     2482 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/series.py
+-rw-r--r--   0        0        0     2375 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/utils.py
+-rw-r--r--   0        0        0     2457 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/wrap.py
+-rw-r--r--   0        0        0      186 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/__init__.py
+-rw-r--r--   0        0        0     2017 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/asymptotic.py
+-rw-r--r--   0        0        0     1944 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/cfraction.py
+-rw-r--r--   0        0        0     2878 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/integral.py
+-rw-r--r--   0        0        0     2218 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/math.py
+-rw-r--r--   0        0        0      861 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/misc.py
+-rw-r--r--   0        0        0     1890 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/sca.py
+-rw-r--r--   0        0        0     2568 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/series.py
+-rw-r--r--   0        0        0     3289 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/utils.py
+-rw-r--r--   0        0        0     2202 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/wrap.py
+-rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 logbesselk-3.2.1/setup.py
+-rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 logbesselk-3.2.1/PKG-INFO
```

### Comparing `logbesselk-3.2.0/LICENSE.txt` & `logbesselk-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/README.md` & `logbesselk-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/pyproject.toml` & `logbesselk-3.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "logbesselk"
-version = "3.2.0"
+version = "3.2.1"
 description = "Provide function to calculate the modified Bessel function of the second kind"
 license = "Apache-2.0"
 authors = ["TAKEKAWA Takashi <takekawa@tk2lab.org>"]
 readme = "README.md"
 repository = "https://github.com/tk2lab/logbesselk"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8,<3.13"
 #tensorflow = ">=2.6,<2.12"
 #jax = "^0.2+cuda"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
```

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/asymptotic.py` & `logbesselk-3.2.1/src/logbesselk/jax/asymptotic.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/cfraction.py` & `logbesselk-3.2.1/src/logbesselk/jax/cfraction.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/integral.py` & `logbesselk-3.2.1/src/logbesselk/jax/integral.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/math.py` & `logbesselk-3.2.1/src/logbesselk/jax/math.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/misc.py` & `logbesselk-3.2.1/src/logbesselk/jax/misc.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/sca.py` & `logbesselk-3.2.1/src/logbesselk/jax/sca.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/series.py` & `logbesselk-3.2.1/src/logbesselk/jax/series.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/utils.py` & `logbesselk-3.2.1/src/logbesselk/jax/utils.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/jax/wrap.py` & `logbesselk-3.2.1/src/logbesselk/jax/wrap.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/asymptotic.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/asymptotic.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/cfraction.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/cfraction.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/integral.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/integral.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/math.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/misc.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/misc.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/sca.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/sca.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/series.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/series.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/utils.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/utils.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/src/logbesselk/tensorflow/wrap.py` & `logbesselk-3.2.1/src/logbesselk/tensorflow/wrap.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.0/setup.py` & `logbesselk-3.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ['logbesselk', 'logbesselk.jax', 'logbesselk.tensorflow']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'logbesselk',
-    'version': '3.2.0',
+    'version': '3.2.1',
     'description': 'Provide function to calculate the modified Bessel function of the second kind',
     'long_description': '# logbesselk\nProvide function to calculate the modified Bessel function of the second kind\nand its derivatives.\n\n## Reference\nTakashi Takekawa, Fast parallel calculation of modified Bessel function\nof the second kind and its derivatives, SoftwareX, 17, 100923, 2022.\n\n## Author\nTAKEKAWA Takashi <takekawa@tk2lab.org>\n\n\n## For Tensorflow\n\n### Require\n- Python (>=3.8)\n- Tensorflow (>=2.6)\n\n### Installation\n```shell\npip install tensorflow logbesselk\n```\n\n### Examples\n```python\nimport tensorflow as tf\nfrom logbesselk.tensorflow import log_bessel_k as logk\nfrom logbesselk.jax import bessel_ke as ke\nfrom logbesselk.jax import bessel_kratio as kratio\n\nv = 1.0\nx = 1.0\na = logk(v, x)\n\nv = jnp.linspace(1, 10, 10)\nx = jnp.linspace(1, 10, 10)\nb = logk(v, x)\n\n# gradient\nwith tf.GradientTape() as g:\n    g.watch(v, x)\n    f = logk(v, x)\ndlogkdv = g.gradient(f, v)\ndlogkdx = g.gradient(f, x)\n\n# use tf.function\nlogk = tf.function(logk)\n\n# advanced version\nfrom logbesselk.tensorflow import log_abs_deriv_bessel_k\n\nlogk = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 0)\nlogdkdv = lambda v, x: log_abs_deriv_bessel_k(v, x, 1, 0)\nlogdkdx = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 1)\n```\n\n\n## For jax\n\n### Require\n- Python (>=3.8)\n- jax (>=0.3)\n\n### Installation\n```shell\npip install jax[cuda] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html\npip install logbesselk\n```\n\n### Examples\n```python\nimport jax\nimport jax.numpy as jnp\nfrom logbesselk.jax import log_bessel_k as logk\nfrom logbesselk.jax import bessel_ke as ke\nfrom logbesselk.jax import bessel_kratio as kratio\n\n# scalar func and grad\nv = 1.0\nx = 1.0\na = logk(v, x)\n\n# dlogK/dv = (dK/dv) / K\ndlogkdv = jax.grad(logk, 0)\nb = dlogkdv(v, x)\n\n# dlogK/dx = (dK/dx) / K\ndlogkdx = jax.grad(logk, 1)\nc = dlogkdx(v, x)\n\n# misc\nd = ke(v, x)\ne = kratio(v, x, d=1)\n\n# vectorize\nlogk_vec = jax.vmap(logk)\n\nv = jnp.linspace(1, 10, 10)\nx = jnp.linspace(1, 10, 10)\nf = logk_vec(v)\n\n# use jit\nlogk_vec_jit = jax.jit(logk_vec)\n\n# advanced version\nfrom logbesselk.jax import log_abs_devel_bessel_k\n\nlog_dkdv = lambda v, x: log_abs_deriv_bessel_k(v, x, 1, 0)\nlog_dkdx = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 1)\n\nlog_dkdv_jit = jax.jit(jax.vmap(log_dkdv))\nlog_dkdx_jit = jax.jit(jax.vmap(log_dkdx))\n```\n',
     'author': 'TAKEKAWA Takashi',
     'author_email': 'takekawa@tk2lab.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tk2lab/logbesselk',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>=3.8,<3.13',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `logbesselk-3.2.0/PKG-INFO` & `logbesselk-3.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: logbesselk
-Version: 3.2.0
+Version: 3.2.1
 Summary: Provide function to calculate the modified Bessel function of the second kind
 Home-page: https://github.com/tk2lab/logbesselk
 License: Apache-2.0
 Author: TAKEKAWA Takashi
 Author-email: takekawa@tk2lab.org
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/tk2lab/logbesselk
```

