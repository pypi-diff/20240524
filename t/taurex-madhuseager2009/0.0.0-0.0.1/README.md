# Comparing `tmp/taurex_madhuseager2009-0.0.0.tar.gz` & `tmp/taurex_madhuseager2009-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taurex_madhuseager2009-0.0.0.tar", max compression
+gzip compressed data, was "taurex_madhuseager2009-0.0.1.tar", max compression
```

## Comparing `taurex_madhuseager2009-0.0.0.tar` & `taurex_madhuseager2009-0.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1868 2023-06-29 10:16:16.317596 taurex_madhuseager2009-0.0.0/README.md
--rw-r--r--   0        0        0      816 2024-05-24 11:19:40.197096 taurex_madhuseager2009-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-16 19:08:54.445446 taurex_madhuseager2009-0.0.0/taurex_madhuseager2009/.DS_Store
--rw-r--r--   0        0        0     8213 2023-07-03 14:30:16.642748 taurex_madhuseager2009-0.0.0/taurex_madhuseager2009/MadhuSeager2009.py
--rw-r--r--   0        0        0       45 2023-06-16 19:03:52.752348 taurex_madhuseager2009-0.0.0/taurex_madhuseager2009/__init__.py
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 taurex_madhuseager2009-0.0.0/setup.py
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 taurex_madhuseager2009-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1971 2024-05-24 11:24:49.190892 taurex_madhuseager2009-0.0.1/README.md
+-rw-r--r--   0        0        0      823 2024-05-24 11:35:23.021558 taurex_madhuseager2009-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-16 19:08:54.445446 taurex_madhuseager2009-0.0.1/taurex_madhuseager2009/.DS_Store
+-rw-r--r--   0        0        0     8213 2023-07-03 14:30:16.642748 taurex_madhuseager2009-0.0.1/taurex_madhuseager2009/MadhuSeager2009.py
+-rw-r--r--   0        0        0       45 2023-06-16 19:03:52.752348 taurex_madhuseager2009-0.0.1/taurex_madhuseager2009/__init__.py
+-rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 taurex_madhuseager2009-0.0.1/setup.py
+-rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 taurex_madhuseager2009-0.0.1/PKG-INFO
```

### Comparing `taurex_madhuseager2009-0.0.0/README.md` & `taurex_madhuseager2009-0.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 ## Requirements
 
 - You will need a working installation of TauREx 3.1 on your machine or computer server, with associated required Python packages: https://taurex3-public.readthedocs.io/
 
 ## Installation
 
+You can install _MadhuSeager2009_ with PyPi:
+
+```console
+pip install taurex-madhuseager2009
+```
+
 You can install _MadhuSeager2009_ by cloning this Github and installing via the terminal. This is done by:
 
 Cloning the directory using:
 
 ```console
 $ git clone https://github.com/michellebieger/MadhuSeager2009
 ```
@@ -40,21 +46,21 @@
 
 If there are no errors, you have been successful!
 
 ## Usage
 
 You can use the ExampleNotebook in the repository, which runs this PT profile with TauREx as a forward model in a Jupyter Notebook. You can further modify the Notebook and include retrievals if desired.
 
-To use the MadhuSeager2009 PT profile in a .par file and run TauREx on a command line, you can call the profile with either the keywords 'MadhuSeager2009' or 'madhuseager2009' under the [Temperature] parameter:
+To use the MadhuSeager2009 PT profile in a `.par` file and run TauREx on a command line, you can call the profile with either the keywords 'MadhuSeager2009' or 'madhuseager2009' under the "[Temperature]" parameter:
 
 ```console
 $ profile_type = MadhuSeager2009
 ```
 
-An example .par file exists in this repository with all the parameters relevant to this PT profile--just add in your desired values/further parameters as normal when using TauREx and any other TauREx plugins.
+An example `.par` file exists in this repository with all the parameters relevant to this PT profile--just add in your desired values/further parameters as normal when using TauREx and any other TauREx plugins.
 
 ## License
 
 Distributed under the terms of the [GPL 3.0 license][license],
 _MadhuSeager2009_ is free and open source software.
 
 ## Issues
```

### Comparing `taurex_madhuseager2009-0.0.0/pyproject.toml` & `taurex_madhuseager2009-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taurex_MadhuSeager2009"
-version = "0.0.0"
+version = "0.0.1"
 description = "MadhuSeager2009"
 authors = ["M. F. Bieger <mb987@exeter.ac.uk>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/michellebieger/MadhuSeager2009"
 repository = "https://github.com/michellebieger/MadhuSeager2009"
 classifiers = ["Development Status :: 1 - Planning"]
@@ -18,12 +18,12 @@
 
 [tool.poetry.group.dev.dependencies]
 black = { version = "^22.10.0", allow-prereleases = true }
 ipython = "^8.6.0"
 jupyterlab = "^3.5.0"
 
 [tool.poetry.plugins."taurex.plugins"]
-MadhuSeager2009 = "MadhuSeager2009.taurex"
+taurex_MadhuSeager2009 = "MadhuSeager2009.taurex"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `taurex_madhuseager2009-0.0.0/taurex_madhuseager2009/.DS_Store` & `taurex_madhuseager2009-0.0.1/taurex_madhuseager2009/.DS_Store`

 * *Files identical despite different names*

### Comparing `taurex_madhuseager2009-0.0.0/taurex_madhuseager2009/MadhuSeager2009.py` & `taurex_madhuseager2009-0.0.1/taurex_madhuseager2009/MadhuSeager2009.py`

 * *Files identical despite different names*

### Comparing `taurex_madhuseager2009-0.0.0/setup.py` & `taurex_madhuseager2009-0.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['taurex>=3.1.1a0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['MadhuSeager2009 = MadhuSeager2009.__main__:main'],
- 'taurex.plugins': ['MadhuSeager2009 = MadhuSeager2009.taurex']}
+ 'taurex.plugins': ['taurex_MadhuSeager2009 = MadhuSeager2009.taurex']}
 
 setup_kwargs = {
     'name': 'taurex-madhuseager2009',
-    'version': '0.0.0',
+    'version': '0.0.1',
     'description': 'MadhuSeager2009',
-    'long_description': '# MadhuSeager2009: a TauREx 3.1 plugin to replicate the Madhusudhan Seager 2009 temperature-pressure profile\n\n## Requirements\n\n- You will need a working installation of TauREx 3.1 on your machine or computer server, with associated required Python packages: https://taurex3-public.readthedocs.io/\n\n## Installation\n\nYou can install _MadhuSeager2009_ by cloning this Github and installing via the terminal. This is done by:\n\nCloning the directory using:\n\n```console\n$ git clone https://github.com/michellebieger/MadhuSeager2009\n```\n\nMove into the downloaded folder:\n\n```console\n$ cd MadhuSeager2009\n```\n\nInstall by then typing in:\n\n```console\n$ pip install .\n```\n\nYou can check the installation by importing the plugin into Python:\n\n```console\n$ python -c "import MadhuSeager2009"\n```\n\nTo check that TauREx 3.1 has correctly registered your plugin:\n\n```console\n$ taurex --plugins\n```\n\nIf there are no errors, you have been successful!\n\n## Usage\n\nYou can use the ExampleNotebook in the repository, which runs this PT profile with TauREx as a forward model in a Jupyter Notebook. You can further modify the Notebook and include retrievals if desired.\n\nTo use the MadhuSeager2009 PT profile in a .par file and run TauREx on a command line, you can call the profile with either the keywords \'MadhuSeager2009\' or \'madhuseager2009\' under the [Temperature] parameter:\n\n```console\n$ profile_type = MadhuSeager2009\n```\n\nAn example .par file exists in this repository with all the parameters relevant to this PT profile--just add in your desired values/further parameters as normal when using TauREx and any other TauREx plugins.\n\n## License\n\nDistributed under the terms of the [GPL 3.0 license][license],\n_MadhuSeager2009_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems, please email michellebieger@live.com with a detailed description of the issue.\n',
+    'long_description': '# MadhuSeager2009: a TauREx 3.1 plugin to replicate the Madhusudhan Seager 2009 temperature-pressure profile\n\n## Requirements\n\n- You will need a working installation of TauREx 3.1 on your machine or computer server, with associated required Python packages: https://taurex3-public.readthedocs.io/\n\n## Installation\n\nYou can install _MadhuSeager2009_ with PyPi:\n\n```console\npip install taurex-madhuseager2009\n```\n\nYou can install _MadhuSeager2009_ by cloning this Github and installing via the terminal. This is done by:\n\nCloning the directory using:\n\n```console\n$ git clone https://github.com/michellebieger/MadhuSeager2009\n```\n\nMove into the downloaded folder:\n\n```console\n$ cd MadhuSeager2009\n```\n\nInstall by then typing in:\n\n```console\n$ pip install .\n```\n\nYou can check the installation by importing the plugin into Python:\n\n```console\n$ python -c "import MadhuSeager2009"\n```\n\nTo check that TauREx 3.1 has correctly registered your plugin:\n\n```console\n$ taurex --plugins\n```\n\nIf there are no errors, you have been successful!\n\n## Usage\n\nYou can use the ExampleNotebook in the repository, which runs this PT profile with TauREx as a forward model in a Jupyter Notebook. You can further modify the Notebook and include retrievals if desired.\n\nTo use the MadhuSeager2009 PT profile in a `.par` file and run TauREx on a command line, you can call the profile with either the keywords \'MadhuSeager2009\' or \'madhuseager2009\' under the "[Temperature]" parameter:\n\n```console\n$ profile_type = MadhuSeager2009\n```\n\nAn example `.par` file exists in this repository with all the parameters relevant to this PT profile--just add in your desired values/further parameters as normal when using TauREx and any other TauREx plugins.\n\n## License\n\nDistributed under the terms of the [GPL 3.0 license][license],\n_MadhuSeager2009_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems, please email michellebieger@live.com with a detailed description of the issue.\n',
     'author': 'M. F. Bieger',
     'author_email': 'mb987@exeter.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/michellebieger/MadhuSeager2009',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `taurex_madhuseager2009-0.0.0/PKG-INFO` & `taurex_madhuseager2009-0.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taurex-madhuseager2009
-Version: 0.0.0
+Version: 0.0.1
 Summary: MadhuSeager2009
 Home-page: https://github.com/michellebieger/MadhuSeager2009
 License: GPL-3.0
 Author: M. F. Bieger
 Author-email: mb987@exeter.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -22,14 +22,20 @@
 
 ## Requirements
 
 - You will need a working installation of TauREx 3.1 on your machine or computer server, with associated required Python packages: https://taurex3-public.readthedocs.io/
 
 ## Installation
 
+You can install _MadhuSeager2009_ with PyPi:
+
+```console
+pip install taurex-madhuseager2009
+```
+
 You can install _MadhuSeager2009_ by cloning this Github and installing via the terminal. This is done by:
 
 Cloning the directory using:
 
 ```console
 $ git clone https://github.com/michellebieger/MadhuSeager2009
 ```
@@ -60,21 +66,21 @@
 
 If there are no errors, you have been successful!
 
 ## Usage
 
 You can use the ExampleNotebook in the repository, which runs this PT profile with TauREx as a forward model in a Jupyter Notebook. You can further modify the Notebook and include retrievals if desired.
 
-To use the MadhuSeager2009 PT profile in a .par file and run TauREx on a command line, you can call the profile with either the keywords 'MadhuSeager2009' or 'madhuseager2009' under the [Temperature] parameter:
+To use the MadhuSeager2009 PT profile in a `.par` file and run TauREx on a command line, you can call the profile with either the keywords 'MadhuSeager2009' or 'madhuseager2009' under the "[Temperature]" parameter:
 
 ```console
 $ profile_type = MadhuSeager2009
 ```
 
-An example .par file exists in this repository with all the parameters relevant to this PT profile--just add in your desired values/further parameters as normal when using TauREx and any other TauREx plugins.
+An example `.par` file exists in this repository with all the parameters relevant to this PT profile--just add in your desired values/further parameters as normal when using TauREx and any other TauREx plugins.
 
 ## License
 
 Distributed under the terms of the [GPL 3.0 license][license],
 _MadhuSeager2009_ is free and open source software.
 
 ## Issues
```

