# Comparing `tmp/i2c_gui2-0.0.1.tar.gz` & `tmp/i2c_gui2-0.0.2.tar.gz`

## Comparing `i2c_gui2-0.0.1.tar` & `i2c_gui2-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,32 @@
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/.readthedocs.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/README.rst
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/pytest.ini
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/authors.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/changelog.rst
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/contributing.rst
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/index.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/installation.rst
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/readme.rst
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/requirements.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/docs/usage.rst
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/src/i2c_gui2/__init__.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/src/i2c_gui2/etroc1_gui.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/src/i2c_gui2/etroc2_gui.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/tests/test_global.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/.gitignore
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/AUTHORS.rst
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/LICENSE
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/PyPIREADME.md
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 i2c_gui2-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/.bumpversion.cfg
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/README.rst
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/pytest.ini
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/authors.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/changelog.rst
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/contributing.rst
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/index.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/installation.rst
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/readme.rst
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/docs/usage.rst
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/src/i2c_gui2/__init__.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/src/i2c_gui2/etroc1_gui.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/src/i2c_gui2/etroc2_gui.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/src/i2c_gui2/i2c_messages.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/tests/test_global.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/tests/test_i2c_connection_helper.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/tests/test_i2c_messages.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/tests/chips/test_address_space_controller_class.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/.gitignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/LICENSE
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/PyPIREADME.md
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 i2c_gui2-0.0.2/PKG-INFO
```

### Comparing `i2c_gui2-0.0.1/.bumpversion.cfg` & `i2c_gui2-0.0.2/.bumpversion.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.1
+current_version = 0.0.2
 commit = True
 tag = True
 
 [bumpversion:file:src/i2c_gui2/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `i2c_gui2-0.0.1/.pre-commit-config.yaml` & `i2c_gui2-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `i2c_gui2-0.0.1/.readthedocs.yml` & `i2c_gui2-0.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `i2c_gui2-0.0.1/CONTRIBUTING.rst` & `i2c_gui2-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `i2c_gui2-0.0.1/README.rst` & `i2c_gui2-0.0.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 |pre-commit|
 
 |black| |flake8| |isort|
 
 |docs|
 
+|version| |wheel| |supported-versions| |supported-implementations|
+
 |commits-since|
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000
     :target: https://github.com/psf/black
     :alt: black
 
 .. |flake8| image:: https://img.shields.io/badge/flake8-checked-blueviolet
@@ -28,17 +30,33 @@
     :target: https://github.com/pre-commit/pre-commit
     :alt: pre-commit
 
 .. |docs| image:: https://readthedocs.org/projects/i2c-gui2/badge/?version=latest
     :target: https://i2c-gui2.readthedocs.io/
     :alt: Documentation Status
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/cbeiraod/I2C-GUI2/v0.0.1.svg
+.. |version| image:: https://img.shields.io/pypi/v/I2C-GUI2.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/I2C-GUI2
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/I2C-GUI2.svg
+    :alt: PyPI Wheel
+    :target: https://pypi.org/project/I2C-GUI2
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/I2C-GUI2.svg
+    :alt: Supported versions
+    :target: https://pypi.org/project/I2C-GUI2
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/I2C-GUI2.svg
+    :alt: Supported implementations
+    :target: https://pypi.org/project/I2C-GUI2
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/cbeiraod/I2C-GUI2/v0.0.2.svg
     :alt: Commits since latest release
-    :target: https://github.com/cbeiraod/I2c-GUI2/compare/v0.0.1...main
+    :target: https://github.com/cbeiraod/I2c-GUI2/compare/v0.0.2...main
 
 .. end-badges
 
 A new and improved I2C library with a GUI
 
 * Free software: Zlib license
 
@@ -83,14 +101,15 @@
 ----------------------
 If you are working on developing the code for ETROC-DAQ++ you will need to follow the "Running the Software" instructions for setup and then for installing use the "From Source" instructions but instead of the install command in the "Dependencies" instructions, use the following command: ``python -m pip install -e .``.
 Then install a few other dependencies which are only used in development:
 
 .. code:: bash
 
   python -m pip install --upgrade pytest
+  python -m pip install --upgrade pytest-cov
   python -m pip install --upgrade pre-commit
   python -m pip install --upgrade bump2version
   python -m pip install --upgrade black
   python -m pip install --upgrade flake8-pyproject
   python -m pip install --upgrade isort
   python -m pip install --upgrade build
   python -m pip install --upgrade twine
@@ -112,14 +131,18 @@
 
 pytest
 ------
 We are using pytest to run unit tests on the software.
 See `here <https://docs.pytest.org/en/7.4.x/getting-started.html>`_ for ideas on how to get started.
 Use the command ``pytest`` to run all the tests.
 
+We use the pytest-cov plugin to get coverage reports from pytest.
+Use the command ``pytest --cov --cov-report term-missing`` to run all the tests and get a coverage report.
+Use the command ``pytest --cov --cov-report term-missing --cov-report html`` to get an html report with detailed information.
+
 pre-commit
 ----------
 **pre-commit may need to be installed in the global python environment for things to work correctly.**
 This tool allows to setup hooks into the git workflow, in particular for the Pre-Commit Hook, allowing to run automated tests before committing code.
 This functionality is used to automatically run black, flake8 and isort before any commit is made, thus guaranteeing a consistent style and formatting for all committed code (according to these tools).
 If you want to run all the checks individually as if a commit were about to be made, you can use ``pre-commit run --all-files``.
 You can find more information on pre-commit `here <https://pre-commit.com/>`_.
```

### Comparing `i2c_gui2-0.0.1/pytest.ini` & `i2c_gui2-0.0.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `i2c_gui2-0.0.1/.github/workflows/publish-to-test-pypi.yml` & `i2c_gui2-0.0.2/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `i2c_gui2-0.0.1/docs/conf.py` & `i2c_gui2-0.0.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'I2C-GUI2'
 year = '2024'
 author = 'Cristóvão B. da Cruz e Silva'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '0.0.1'
+version = release = '0.0.2'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/cbeiraod/I2C-GUI2/issues/%s', '#'),
     'pr': ('https://github.com/cbeiraod/I2C-GUI2/pull/%s', 'PR #'),
 }
```

### Comparing `i2c_gui2-0.0.1/src/i2c_gui2/__init__.py` & `i2c_gui2-0.0.2/src/i2c_gui2/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #############################################################################
 # zlib License
 #
-# (C) 2023 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
+# (C) 2024 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
 #
 # This software is provided 'as-is', without any express or implied
 # warranty.  In no event will the authors be held liable for any damages
 # arising from the use of this software.
 #
 # Permission is granted to anyone to use this software for any purpose,
 # including commercial applications, and to alter it and redistribute it
@@ -19,10 +19,12 @@
 # 2. Altered source versions must be plainly marked as such, and must not be
 #    misrepresented as being the original software.
 # 3. This notice may not be removed or altered from any source distribution.
 #############################################################################
 
 from __future__ import annotations
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
-__all__ = []
+from .i2c_messages import I2CMessages
+
+__all__ = ["I2CMessages"]
```

### Comparing `i2c_gui2-0.0.1/src/i2c_gui2/etroc1_gui.py` & `i2c_gui2-0.0.2/src/i2c_gui2/etroc1_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #############################################################################
 # zlib License
 #
-# (C) 2023 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
+# (C) 2024 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
 #
 # This software is provided 'as-is', without any express or implied
 # warranty.  In no event will the authors be held liable for any damages
 # arising from the use of this software.
 #
 # Permission is granted to anyone to use this software for any purpose,
 # including commercial applications, and to alter it and redistribute it
```

### Comparing `i2c_gui2-0.0.1/src/i2c_gui2/etroc2_gui.py` & `i2c_gui2-0.0.2/src/i2c_gui2/etroc2_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #############################################################################
 # zlib License
 #
-# (C) 2023 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
+# (C) 2024 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
 #
 # This software is provided 'as-is', without any express or implied
 # warranty.  In no event will the authors be held liable for any damages
 # arising from the use of this software.
 #
 # Permission is granted to anyone to use this software for any purpose,
 # including commercial applications, and to alter it and redistribute it
```

### Comparing `i2c_gui2-0.0.1/tests/test_global.py` & `i2c_gui2-0.0.2/tests/test_global.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #############################################################################
 # zlib License
 #
-# (C) 2023 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
+# (C) 2024 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
 #
 # This software is provided 'as-is', without any express or implied
 # warranty.  In no event will the authors be held liable for any damages
 # arising from the use of this software.
 #
 # Permission is granted to anyone to use this software for any purpose,
 # including commercial applications, and to alter it and redistribute it
@@ -23,12 +23,12 @@
 
 import pytest
 
 
 def test_version():
     import i2c_gui2
 
-    version = '0.0.1'
+    version = '0.0.2'
 
     pytest.param
 
     assert version == i2c_gui2.__version__
```

### Comparing `i2c_gui2-0.0.1/LICENSE` & `i2c_gui2-0.0.2/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 zlib License
 
-(C) 2023 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
+(C) 2024 Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
 
 This software is provided 'as-is', without any express or implied
 warranty.  In no event will the authors be held liable for any damages
 arising from the use of this software.
 
 Permission is granted to anyone to use this software for any purpose,
 including commercial applications, and to alter it and redistribute it
```

### Comparing `i2c_gui2-0.0.1/pyproject.toml` & `i2c_gui2-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "I2C-GUI2"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Cristóvão Beirão da Cruz e Silva", email="cbeiraod@cern.ch" },
 ]
 maintainers = [
 ]
 description = "A new and improved I2C library with a GUI"
 readme = "PyPIREADME.md"
```

### Comparing `i2c_gui2-0.0.1/PKG-INFO` & `i2c_gui2-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: I2C-GUI2
-Version: 0.0.1
+Version: 0.0.2
 Summary: A new and improved I2C library with a GUI
 Project-URL: Homepage, https://github.com/cbeiraod/I2C-GUI2
 Project-URL: Documentation, https://i2c-gui2.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/cbeiraod/I2C-GUI2/issues
 Author-email: Cristóvão Beirão da Cruz e Silva <cbeiraod@cern.ch>
 License-File: AUTHORS.rst
 License-File: LICENSE
@@ -21,7 +21,9 @@
 
 # I2C-GUI++
 A new and improved I2C communication library with a GUI
 
 This is currently a placeholder for the I2C-GUI++ project.
 
 You can install the I2C-GUI++ libraries and GUI with: `python -m pip install I2C-GUI2`
+
+After installation, you can run the individual chip GUIs with dedicated commands such as: `etroc2_gui`
```

