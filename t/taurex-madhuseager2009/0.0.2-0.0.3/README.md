# Comparing `tmp/taurex_madhuseager2009-0.0.2.tar.gz` & `tmp/taurex_madhuseager2009-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taurex_madhuseager2009-0.0.2.tar", max compression
+gzip compressed data, was "taurex_madhuseager2009-0.0.3.tar", max compression
```

## Comparing `taurex_madhuseager2009-0.0.2.tar` & `taurex_madhuseager2009-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1971 2024-05-24 11:24:49.190892 taurex_madhuseager2009-0.0.2/README.md
--rw-r--r--   0        0        0      830 2024-05-24 11:42:12.040448 taurex_madhuseager2009-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-16 19:08:54.445446 taurex_madhuseager2009-0.0.2/taurex_madhuseager2009/.DS_Store
--rw-r--r--   0        0        0     8213 2023-07-03 14:30:16.642748 taurex_madhuseager2009-0.0.2/taurex_madhuseager2009/MadhuSeager2009.py
--rw-r--r--   0        0        0       45 2023-06-16 19:03:52.752348 taurex_madhuseager2009-0.0.2/taurex_madhuseager2009/__init__.py
--rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 taurex_madhuseager2009-0.0.2/setup.py
--rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 taurex_madhuseager2009-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1971 2024-05-24 11:24:49.190892 taurex_madhuseager2009-0.0.3/README.md
+-rw-r--r--   0        0        0      844 2024-05-24 11:44:58.793215 taurex_madhuseager2009-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-16 19:08:54.445446 taurex_madhuseager2009-0.0.3/taurex_madhuseager2009/.DS_Store
+-rw-r--r--   0        0        0       52 2024-05-24 11:44:42.209081 taurex_madhuseager2009-0.0.3/taurex_madhuseager2009/__init__.py
+-rw-r--r--   0        0        0     8213 2023-07-03 14:30:16.642748 taurex_madhuseager2009-0.0.3/taurex_madhuseager2009/taurex_MadhuSeager2009.py
+-rw-r--r--   0        0        0     2963 1970-01-01 00:00:00.000000 taurex_madhuseager2009-0.0.3/setup.py
+-rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 taurex_madhuseager2009-0.0.3/PKG-INFO
```

### Comparing `taurex_madhuseager2009-0.0.2/README.md` & `taurex_madhuseager2009-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `taurex_madhuseager2009-0.0.2/pyproject.toml` & `taurex_madhuseager2009-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "taurex_MadhuSeager2009"
-version = "0.0.2"
+version = "0.0.3"
 description = "MadhuSeager2009"
 authors = ["M. F. Bieger <mb987@exeter.ac.uk>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/michellebieger/MadhuSeager2009"
 repository = "https://github.com/michellebieger/MadhuSeager2009"
 classifiers = ["Development Status :: 1 - Planning"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 taurex = "^3.1.1a0"
 
 [tool.poetry.scripts]
-MadhuSeager2009 = "MadhuSeager2009.__main__:main"
+taurex_MadhuSeager2009 = "taurex_MadhuSeager2009.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 black = { version = "^22.10.0", allow-prereleases = true }
 ipython = "^8.6.0"
 jupyterlab = "^3.5.0"
 
 [tool.poetry.plugins."taurex.plugins"]
```

### Comparing `taurex_madhuseager2009-0.0.2/taurex_madhuseager2009/.DS_Store` & `taurex_madhuseager2009-0.0.3/taurex_madhuseager2009/.DS_Store`

 * *Files identical despite different names*

### Comparing `taurex_madhuseager2009-0.0.2/taurex_madhuseager2009/MadhuSeager2009.py` & `taurex_madhuseager2009-0.0.3/taurex_madhuseager2009/taurex_MadhuSeager2009.py`

 * *Files identical despite different names*

### Comparing `taurex_madhuseager2009-0.0.2/setup.py` & `taurex_madhuseager2009-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['taurex>=3.1.1a0,<4.0.0']
 
 entry_points = \
-{'console_scripts': ['MadhuSeager2009 = MadhuSeager2009.__main__:main'],
+{'console_scripts': ['taurex_MadhuSeager2009 = '
+                     'taurex_MadhuSeager2009.__main__:main'],
  'taurex.plugins': ['taurex_MadhuSeager2009 = taurex_MadhuSeager2009.taurex']}
 
 setup_kwargs = {
     'name': 'taurex-madhuseager2009',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'MadhuSeager2009',
     'long_description': '# MadhuSeager2009: a TauREx 3.1 plugin to replicate the Madhusudhan Seager 2009 temperature-pressure profile\n\n## Requirements\n\n- You will need a working installation of TauREx 3.1 on your machine or computer server, with associated required Python packages: https://taurex3-public.readthedocs.io/\n\n## Installation\n\nYou can install _MadhuSeager2009_ with PyPi:\n\n```console\npip install taurex-madhuseager2009\n```\n\nYou can install _MadhuSeager2009_ by cloning this Github and installing via the terminal. This is done by:\n\nCloning the directory using:\n\n```console\n$ git clone https://github.com/michellebieger/MadhuSeager2009\n```\n\nMove into the downloaded folder:\n\n```console\n$ cd MadhuSeager2009\n```\n\nInstall by then typing in:\n\n```console\n$ pip install .\n```\n\nYou can check the installation by importing the plugin into Python:\n\n```console\n$ python -c "import MadhuSeager2009"\n```\n\nTo check that TauREx 3.1 has correctly registered your plugin:\n\n```console\n$ taurex --plugins\n```\n\nIf there are no errors, you have been successful!\n\n## Usage\n\nYou can use the ExampleNotebook in the repository, which runs this PT profile with TauREx as a forward model in a Jupyter Notebook. You can further modify the Notebook and include retrievals if desired.\n\nTo use the MadhuSeager2009 PT profile in a `.par` file and run TauREx on a command line, you can call the profile with either the keywords \'MadhuSeager2009\' or \'madhuseager2009\' under the "[Temperature]" parameter:\n\n```console\n$ profile_type = MadhuSeager2009\n```\n\nAn example `.par` file exists in this repository with all the parameters relevant to this PT profile--just add in your desired values/further parameters as normal when using TauREx and any other TauREx plugins.\n\n## License\n\nDistributed under the terms of the [GPL 3.0 license][license],\n_MadhuSeager2009_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems, please email michellebieger@live.com with a detailed description of the issue.\n',
     'author': 'M. F. Bieger',
     'author_email': 'mb987@exeter.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/michellebieger/MadhuSeager2009',
```

### Comparing `taurex_madhuseager2009-0.0.2/PKG-INFO` & `taurex_madhuseager2009-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taurex-madhuseager2009
-Version: 0.0.2
+Version: 0.0.3
 Summary: MadhuSeager2009
 Home-page: https://github.com/michellebieger/MadhuSeager2009
 License: GPL-3.0
 Author: M. F. Bieger
 Author-email: mb987@exeter.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
```

