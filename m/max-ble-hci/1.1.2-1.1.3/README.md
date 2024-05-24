# Comparing `tmp/max_ble_hci-1.1.2.tar.gz` & `tmp/max_ble_hci-1.1.3.tar.gz`

## Comparing `max_ble_hci-1.1.2.tar` & `max_ble_hci-1.1.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/install.bat
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/install.sh
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.github/workflows/black-format-check.yml
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.github/workflows/black-format-run.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.github/workflows/pypi-deploy.yml
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.github/workflows/requirements.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.github/workflows/test-installer.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/make.bat
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/ble_hci.rst
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/ble_standard.rst
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/constants.rst
--rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/controller_cmds.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/data_params.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/examples.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/hci_packets.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/hci_reference.rst
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/index.rst
--rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/informational_cmds.rst
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/installation.rst
--rw-r--r--   0        0        0   236831 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/le_controller_cmds.rst
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/link_control_cmds.rst
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/modules.rst
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/overview.rst
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/packet_codes.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/packet_defs.rst
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/status_cmds.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/utils.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/vendor_spec.rst
--rw-r--r--   0        0        0    95227 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/vendor_spec_cmds.rst
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/examples/connection.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/examples/dtm.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/examples/hello_hci.py
--rw-r--r--   0        0        0    38521 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/docs/source/images/ble_stack_diagram.jpeg
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/examples/connection.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/examples/dtm.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/examples/hello_hci.py
--rw-r--r--   0        0        0    25454 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci_cli.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/__init__.py
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/_hci_logger.py
--rw-r--r--   0        0        0    14622 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/_transport.py
--rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/ble_hci.py
--rw-r--r--   0        0        0    22517 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/ble_standard_cmds.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/constants.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/data_params.py
--rw-r--r--   0        0        0    19610 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/hci_packets.py
--rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/packet_codes.py
--rw-r--r--   0        0        0    19548 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/packet_defs.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/utils.py
--rw-r--r--   0        0        0    56073 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/src/max_ble_hci/vendor_spec_cmds.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/tests/test.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/LICENSE
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/README.md
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 max_ble_hci-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/install.bat
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/install.sh
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.github/workflows/black-format-check.yml
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.github/workflows/black-format-run.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.github/workflows/pypi-deploy.yml
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.github/workflows/requirements.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.github/workflows/test-installer.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/make.bat
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/ble_hci.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/ble_standard.rst
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/conf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/constants.rst
+-rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/controller_cmds.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/data_params.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/examples.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/hci_packets.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/hci_reference.rst
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/index.rst
+-rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/informational_cmds.rst
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/installation.rst
+-rw-r--r--   0        0        0   236831 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/le_controller_cmds.rst
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/link_control_cmds.rst
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/modules.rst
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/overview.rst
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/packet_codes.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/packet_defs.rst
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/status_cmds.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/utils.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/vendor_spec.rst
+-rw-r--r--   0        0        0    95227 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/vendor_spec_cmds.rst
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/examples/connection.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/examples/dtm.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/examples/hello_hci.py
+-rw-r--r--   0        0        0    38521 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/docs/source/images/ble_stack_diagram.jpeg
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/examples/connection.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/examples/dtm.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/examples/hello_hci.py
+-rw-r--r--   0        0        0    25862 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci_cli.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/__init__.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/_hci_logger.py
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/_transport.py
+-rw-r--r--   0        0        0    14711 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/ble_hci.py
+-rw-r--r--   0        0        0    22517 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/ble_standard_cmds.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/constants.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/data_params.py
+-rw-r--r--   0        0        0    19610 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/hci_packets.py
+-rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/packet_codes.py
+-rw-r--r--   0        0        0    19548 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/packet_defs.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/utils.py
+-rw-r--r--   0        0        0    56073 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/src/max_ble_hci/vendor_spec_cmds.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/tests/test.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 max_ble_hci-1.1.3/PKG-INFO
```

### Comparing `max_ble_hci-1.1.2/.github/workflows/black-format-run.yml` & `max_ble_hci-1.1.3/.github/workflows/black-format-run.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/.github/workflows/documentation.yml` & `max_ble_hci-1.1.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/.github/workflows/pylint.yml` & `max_ble_hci-1.1.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/.github/workflows/pypi-deploy.yml` & `max_ble_hci-1.1.3/.github/workflows/pypi-deploy.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 name: deploy-pypi
 on: [workflow_dispatch]
 jobs:
   deploy:
-    name: runner / linux
-    runs-on: ubuntu-latest
+    # name: runner / linux
+    runs-on: [self-hosted]
     steps:
     # - name: build
     #   run: |
     #     pip3 install --upgrade build 
     #     python3 -m build
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - run: |
+        set -e
         pip3 install --upgrade build 
         python3 -m build
-
-        # set -e
-        # python3 -m pip install --upgrade twine
-        # sudo chmod +x install.sh
-        # ./install.sh
+        python3 -m pip install --upgrade twine
         # python3 -m twine upload --repository testpypi dist/*
-        # python3 -m twine upload --repository pypi dist/*
-        # set +e
-    - name: Publish package to TestPyPI
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-        repository-url: https://test.pypi.org/legacy/
+        python3 -m twine upload --repository pypi dist/*
+        set +e
+    # - name: Publish package to TestPyPI
+    #   uses: pypa/gh-action-pypi-publish@release/v1
+    #   with:
+    #     password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+    #     repository-url: https://test.pypi.org/legacy/
```

### Comparing `max_ble_hci-1.1.2/.github/workflows/python-package-conda.yml` & `max_ble_hci-1.1.3/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/.github/workflows/test-installer.yml` & `max_ble_hci-1.1.3/.github/workflows/test-installer.yml`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/Makefile` & `max_ble_hci-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/make.bat` & `max_ble_hci-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/conf.py` & `max_ble_hci-1.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/controller_cmds.rst` & `max_ble_hci-1.1.3/docs/source/controller_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/examples.rst` & `max_ble_hci-1.1.3/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/index.rst` & `max_ble_hci-1.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/informational_cmds.rst` & `max_ble_hci-1.1.3/docs/source/informational_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/installation.rst` & `max_ble_hci-1.1.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/le_controller_cmds.rst` & `max_ble_hci-1.1.3/docs/source/le_controller_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/link_control_cmds.rst` & `max_ble_hci-1.1.3/docs/source/link_control_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/overview.rst` & `max_ble_hci-1.1.3/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/status_cmds.rst` & `max_ble_hci-1.1.3/docs/source/status_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/vendor_spec_cmds.rst` & `max_ble_hci-1.1.3/docs/source/vendor_spec_cmds.rst`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/examples/connection.py` & `max_ble_hci-1.1.3/docs/source/examples/connection.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/examples/dtm.py` & `max_ble_hci-1.1.3/docs/source/examples/dtm.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/examples/hello_hci.py` & `max_ble_hci-1.1.3/docs/source/examples/hello_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/docs/source/images/ble_stack_diagram.jpeg` & `max_ble_hci-1.1.3/docs/source/images/ble_stack_diagram.jpeg`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/examples/connection.py` & `max_ble_hci-1.1.3/examples/connection.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/examples/dtm.py` & `max_ble_hci-1.1.3/examples/dtm.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/examples/hello_hci.py` & `max_ble_hci-1.1.3/examples/hello_hci.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci_cli.py` & `max_ble_hci-1.1.3/src/max_ble_hci_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         """
 
     # Parse the command line arguments
     parser = argparse.ArgumentParser(
         description=cli_description, formatter_class=RawTextHelpFormatter
     )
 
-    parser.add_argument("--version", action="version", version="%(prog)s 1.0.0")
+    parser.add_argument("--version", action="version", version="%(prog)s 1.1.0")
 
     parser.add_argument("serial_port", help="Serial port path or COM#")
     parser.add_argument(
         "-b",
         "--baud",
         dest="baudRate",
         type=int,
@@ -298,16 +298,16 @@
         formatter_class=RawTextHelpFormatter,
     )
 
     memstats_parser.set_defaults(func=lambda _: print(hci.get_memory_stats()))
 
     #### ADV PARSER ####
     adv_parser = subparsers.add_parser(
-        "adv",
-        help="Send the advertising commands",
+        "adv-start",
+        help="Start advertising",
         formatter_class=RawTextHelpFormatter,
     )
     adv_parser.add_argument(
         "-i",
         "--interval",
         dest="adv_interval",
         type=_hex_int,
@@ -317,26 +317,34 @@
     )
     adv_parser.add_argument(
         "--no-connect",
         dest="connect",
         action="store_false",
         help="Disable advertising as a connectable device.",
     )
+
     adv_parser.set_defaults(
         func=lambda args: print(
             hci.start_advertising(
                 connect=args.connect,
                 adv_params=AdvParams(
+                    adv_type=0 if args.connect else 0x3,
                     interval_min=args.adv_interval,
                     interval_max=args.adv_interval,
                 ),
-            ),
+            )
         ),
         which="adv",
     )
+    adv_stop_parser = subparsers.add_parser(
+        "adv-stop",
+        help="Stop advertising",
+        formatter_class=RawTextHelpFormatter,
+    )
+    adv_stop_parser.set_defaults(func=lambda _: print(hci.enable_adv(False)))
 
     #### SCAN PARSER ####
     scan_parser = subparsers.add_parser(
         "scan",
         help="Send scanning commands and print scan reports, ctrl-c to exit.",
         formatter_class=RawTextHelpFormatter,
     )
@@ -385,18 +393,19 @@
         default=DEFAULT_SUP_TIMEOUT,
         help=f"""Supervision timeout in units of 10ms, 16-bit hex number 0x000A - 0x0C80.
         "Default: {hex(DEFAULT_SUP_TIMEOUT)}""",
     )
     init_parser.set_defaults(
         func=lambda args: print(
             hci.init_connection(
-                args.addr,
+                # just toggle some bit to get a different address
+                addr=int(args.addr.replace(":", ""), 16) ^ 0xA,
                 interval=args.conn_interval,
                 sup_timeout=args.sup_timeout,
-                conn_params=ConnParams(peer_addr=args.addr),
+                conn_params=ConnParams(peer_addr=int(args.addr.replace(":", ""), 16)),
             )
         )
     )
 
     datalen_parser = subparsers.add_parser(
         "data-len", help="Set the max data length", formatter_class=RawTextHelpFormatter
     )
```

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/__init__.py` & `max_ble_hci-1.1.3/src/max_ble_hci/__init__.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/_hci_logger.py` & `max_ble_hci-1.1.3/src/max_ble_hci/_hci_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,14 +110,16 @@
         logging.DEBUG: white + format_debug + reset,
         logging.INFO: green + format_info + reset,
         logging.WARNING: yellow + format_str + reset,
         logging.ERROR: red + format_str + reset,
         logging.CRITICAL: bold_red + format_str + reset,
     }
 
+    precise_time = False
+
     def format(self, record: logging.LogRecord) -> str:
         """Creates and returns formatted log message.
 
         Paremeters
         ----------
         record : logging.LogRecord
             Object containing the log record to be formatted.
@@ -125,19 +127,26 @@
         Returns
         -------
         str
             The formatted log message.
 
         """
         log_fmt = self.FORMATS.get(record.levelno)
-        formatter = logging.Formatter(log_fmt)
+
+        if not self.precise_time:
+            formatter = logging.Formatter(fmt=log_fmt, datefmt="%Y-%m-%d %H:%M:%S")
+        else:
+            formatter = logging.Formatter(fmt=log_fmt)
+
         return formatter.format(record)
 
 
-def get_formatted_logger(log_level=logging.INFO, name="BLE-HCI") -> logging.Logger:
+def get_formatted_logger(
+    log_level=logging.INFO, name="BLE-HCI", precise_time=False
+) -> logging.Logger:
     """Retrieves logger with basic custom format.
 
     The custom formatted logger applies basic coloring
     for logging of different levels.
 
 
     Parameters
@@ -151,13 +160,17 @@
     if logger.hasHandlers():
         return logger
 
     logger.setLevel(log_level)
 
     custom_handler = logging.StreamHandler()
     custom_handler.setLevel(log_level)
-    custom_handler.setFormatter(_CustomFormatter())
+
+    formatter = _CustomFormatter()
+    formatter.precise_time = precise_time
+
+    custom_handler.setFormatter(formatter)
 
     if not logger.handlers:
         logger.addHandler(custom_handler)
 
     return logger
```

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/_transport.py` & `max_ble_hci-1.1.3/src/max_ble_hci/_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,50 +344,60 @@
 
     def _read(self, kill_evt: Event) -> None:
         """Process executed by the port read thread.
 
         PRIVATE
 
         """
+        log_exception = True
         while not kill_evt.is_set():
             # pylint: disable=consider-using-with
-            if self.port.in_waiting and self._port_lock.acquire(blocking=False):
-                pkt_type = self.port.read(1)
-                if pkt_type[0] == PacketType.ASYNC.value:
-                    read_data = self.port.read(4)
-                    data_len = read_data[2] | (read_data[3] << 8)
-                else:
-                    read_data = self.port.read(2)
-                    data_len = read_data[1]
-
-                read_data += self.port.read(data_len)
-                self._port_lock.release()
-                self.logger.info(
-                    "%s  %s<%02X%s",
-                    datetime.datetime.now(),
-                    self.id_tag,
-                    pkt_type[0],
-                    read_data.hex(),
-                )
-
-                with self._data_lock:
-                    if pkt_type[0] == PacketType.ASYNC.value and self.async_callback:
-                        self.async_callback(AsyncPacket.from_bytes(read_data))
+            try:
+                if self.port.in_waiting and self._port_lock.acquire(blocking=False):
+                    log_exception = True
+                    pkt_type = self.port.read(1)
+                    if pkt_type[0] == PacketType.ASYNC.value:
+                        read_data = self.port.read(4)
+                        data_len = read_data[2] | (read_data[3] << 8)
                     else:
-                        pkt = EventPacket.from_bytes(read_data)
-                        if pkt.evt_code in {
-                            EventCode.COMMAND_COMPLETE,
-                            EventCode.COMMAND_STATUS,
-                        }:
-                            # only need one command event at a time
-                            if self._event_packets:
-                                self._event_packets.pop(0)
-                            self._event_packets.append(pkt)
-                        elif self.evt_callback:
-                            self.evt_callback(pkt)
+                        read_data = self.port.read(2)
+                        data_len = read_data[1]
+
+                    read_data += self.port.read(data_len)
+                    self._port_lock.release()
+                    self.logger.info(
+                        "%s  %s<%02X%s",
+                        datetime.datetime.now(),
+                        self.id_tag,
+                        pkt_type[0],
+                        read_data.hex(),
+                    )
+
+                    with self._data_lock:
+                        if (
+                            pkt_type[0] == PacketType.ASYNC.value
+                            and self.async_callback
+                        ):
+                            self.async_callback(AsyncPacket.from_bytes(read_data))
+                        else:
+                            pkt = EventPacket.from_bytes(read_data)
+                            if pkt.evt_code in {
+                                EventCode.COMMAND_COMPLETE,
+                                EventCode.COMMAND_STATUS,
+                            }:
+                                # only need one command event at a time
+                                if self._event_packets:
+                                    self._event_packets.pop(0)
+                                self._event_packets.append(pkt)
+                            elif self.evt_callback:
+                                self.evt_callback(pkt)
+            except OSError:
+                if log_exception:
+                    self.logger.error("OSError")
+                log_exception = False
 
     def _retrieve(
         self,
         timeout: Optional[float],
     ) -> EventPacket:
         """Reads an event from serial port.
```

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/ble_hci.py` & `max_ble_hci-1.1.3/src/max_ble_hci/ble_hci.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
 
         self.reset_connection_stats()
         self.set_default_phy(all_phys=0, tx_phys=7, rx_phys=7)
 
         if adv_params is None:
             adv_type = 0 if connect else 3
             adv_params = AdvParams(adv_type=adv_type)
+
         self.set_adv_params(adv_params)
 
         status = self.enable_adv(True)
 
         return status
 
     def init_connection(
@@ -284,14 +285,15 @@
         ------
         ValueError
             If both `addr` and `conn_params` are None.
         ValueError
             If `addr` is more than 6 bytes in size.
 
         """
+        print(addr)
         if conn_params is None:
             if addr is None:
                 raise ValueError(
                     "Either connection parameters or address must be provided."
                 )
 
             if max((addr.bit_length() + 7) // 8, 1) > 6:
```

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/ble_standard_cmds.py` & `max_ble_hci-1.1.3/src/max_ble_hci/ble_standard_cmds.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/constants.py` & `max_ble_hci-1.1.3/src/max_ble_hci/constants.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/data_params.py` & `max_ble_hci-1.1.3/src/max_ble_hci/data_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     interval_min: int = 0x60
     """Minimum advertising interval."""
 
     interval_max: int = 0x60
     """Maximum advertising interval."""
 
-    adv_type: int = 0x3
+    adv_type: int = 0x0
     """Advertising type."""
 
     own_addr_type: AddrType = AddrType.PUBLIC
     """Own device address type."""
 
     peer_addr_type: AddrType = AddrType.PUBLIC
     """Connectable peer device address type."""
```

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/hci_packets.py` & `max_ble_hci-1.1.3/src/max_ble_hci/hci_packets.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/packet_codes.py` & `max_ble_hci-1.1.3/src/max_ble_hci/packet_codes.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/packet_defs.py` & `max_ble_hci-1.1.3/src/max_ble_hci/packet_defs.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/utils.py` & `max_ble_hci-1.1.3/src/max_ble_hci/utils.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/src/max_ble_hci/vendor_spec_cmds.py` & `max_ble_hci-1.1.3/src/max_ble_hci/vendor_spec_cmds.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/tests/test.py` & `max_ble_hci-1.1.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/LICENSE` & `max_ble_hci-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/README.md` & `max_ble_hci-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `max_ble_hci-1.1.2/pyproject.toml` & `max_ble_hci-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["src/max_ble_hci", "src/max_ble_hci_cli.py"]
 
 [project]
 name = "max_ble_hci"
-version = "1.1.2"
+version = "1.1.3"
 dependencies = [
     "pyserial",
     "pyreadline3 ; platform_system == 'Windows'",
     "gnureadline ; platform_system == 'Darwin'",
     "colorlog"
 ]
 requires-python = ">=3.8"
```

### Comparing `max_ble_hci-1.1.2/PKG-INFO` & `max_ble_hci-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: max_ble_hci
-Version: 1.1.2
+Version: 1.1.3
 Summary: BLE HCI Test interface for controllers capable of the UART transport
 Project-URL: Homepage, https://github.com/Analog-Devices-MSDK/BLE-HCI
 Project-URL: Repository, https://github.com/Analog-Devices-MSDK/BLE-HCI
 Project-URL: Documentation, https://analog-devices-msdk.github.io/MAX-BLE-HCI/
 Project-URL: Bug Tracker, https://github.com/Analog-Devices-MSDK/BLE-HCI/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
```

