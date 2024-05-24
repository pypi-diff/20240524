# Comparing `tmp/pybotters-1.1.1.tar.gz` & `tmp/pybotters-1.2.0.tar.gz`

## Comparing `pybotters-1.1.1.tar` & `pybotters-1.2.0.tar`

### file list

```diff
@@ -1,68 +1,72 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pybotters-1.1.1/.readthedocs.yml
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 pybotters-1.1.1/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.1.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybotters-1.1.1/.github/release.yml
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 pybotters-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pybotters-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pybotters-1.1.1/.vscode/extensions.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pybotters-1.1.1/.vscode/hatch_config.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pybotters-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/Makefile
--rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/advanced.rst
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/conf.py
--rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/contributing.rst
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/examples.rst
--rw-r--r--   0        0        0    16099 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/exchanges.rst
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/favicon.ico
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/index.rst
--rw-r--r--   0        0        0    52834 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/logo.png
--rw-r--r--   0        0        0    16737 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/logo_150.png
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/make.bat
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/reference.rst
--rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/user-guide.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pybotters-1.1.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/binance.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/bitbank.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/bitflyer.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/bitget.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/bybit.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/coincheck.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/gmocoin.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/kucoin.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/okx.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/phemex.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/datastore/requirements.txt
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pybotters-1.1.1/example/trading-bot/bitflyer.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/__version__.py
--rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/auth.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/client.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/request.py
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/store.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/typedefs.py
--rw-r--r--   0        0        0    25835 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/ws.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/__init__.py
--rw-r--r--   0        0        0    31433 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/binance.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bitbank.py
--rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bitflyer.py
--rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bitget.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bitmex.py
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/bybit.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/coincheck.py
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/gmocoin.py
--rw-r--r--   0        0        0    25200 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/kucoin.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/okx.py
--rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/phemex.py
--rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 pybotters-1.1.1/pybotters/models/legacy/gmocoin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0    43212 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_auth.py
--rw-r--r--   0        0        0     9230 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_client.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_request.py
--rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_store.py
--rw-r--r--   0        0        0    45941 2020-02-02 00:00:00.000000 pybotters-1.1.1/tests/test_ws.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pybotters-1.1.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pybotters-1.1.1/LICENCE
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pybotters-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 pybotters-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pybotters-1.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 pybotters-1.2.0/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybotters-1.2.0/.github/release.yml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 pybotters-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pybotters-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pybotters-1.2.0/.vscode/extensions.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pybotters-1.2.0/.vscode/hatch_config.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pybotters-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/advanced.rst
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/conf.py
+-rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/contributing.rst
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/examples.rst
+-rw-r--r--   0        0        0    16771 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/exchanges.rst
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/favicon.ico
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/index.rst
+-rw-r--r--   0        0        0    52834 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/logo.png
+-rw-r--r--   0        0        0    16737 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/logo_150.png
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/reference.rst
+-rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/user-guide.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pybotters-1.2.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/binance.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/bitbank.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/bitflyer.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/bitget.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/bybit.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/coincheck.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/gmocoin.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/kucoin.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/okx.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/phemex.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/datastore/requirements.txt
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/helpers/gmocoin.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pybotters-1.2.0/example/trading-bot/bitflyer.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/__version__.py
+-rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/auth.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/client.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/request.py
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/store.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/typedefs.py
+-rw-r--r--   0        0        0    26046 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/ws.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/helpers/__init__.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/helpers/gmocoin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/__init__.py
+-rw-r--r--   0        0        0    31433 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/binance.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/bitbank.py
+-rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/bitflyer.py
+-rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/bitget.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/bitmex.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/bybit.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/coincheck.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/gmocoin.py
+-rw-r--r--   0        0        0    25200 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/kucoin.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/okx.py
+-rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/phemex.py
+-rw-r--r--   0        0        0    20486 2020-02-02 00:00:00.000000 pybotters-1.2.0/pybotters/models/legacy/gmocoin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybotters-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    43212 2020-02-02 00:00:00.000000 pybotters-1.2.0/tests/test_auth.py
+-rw-r--r--   0        0        0     9230 2020-02-02 00:00:00.000000 pybotters-1.2.0/tests/test_client.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 pybotters-1.2.0/tests/test_helpers.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pybotters-1.2.0/tests/test_request.py
+-rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 pybotters-1.2.0/tests/test_store.py
+-rw-r--r--   0        0        0    49949 2020-02-02 00:00:00.000000 pybotters-1.2.0/tests/test_ws.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pybotters-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pybotters-1.2.0/LICENCE
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pybotters-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 pybotters-1.2.0/PKG-INFO
```

### Comparing `pybotters-1.1.1/README.md` & `pybotters-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/.github/FUNDING.yml` & `pybotters-1.2.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/.github/release.yml` & `pybotters-1.2.0/.github/release.yml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/.github/workflows/ci.yml` & `pybotters-1.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/.github/workflows/publish.yml` & `pybotters-1.2.0/.github/workflows/publish.yml`

 * *Files 19% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 
 permissions:
   contents: read
 
 jobs:
   publish:
     runs-on: ubuntu-latest
+    environment:
+      name: pypi
+      url: https://pypi.org/project/pybotters/
+    permissions:
+      id-token: write
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: "3.x"
     - name: Build package
       run: |
         pipx run --spec build pyproject-build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `pybotters-1.1.1/.vscode/settings.json` & `pybotters-1.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/Makefile` & `pybotters-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/advanced.rst` & `pybotters-1.2.0/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/conf.py` & `pybotters-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/contributing.rst` & `pybotters-1.2.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/examples.rst` & `pybotters-1.2.0/docs/examples.rst`

 * *Files 11% similar despite different names*

```diff
@@ -126,7 +126,25 @@
 
 .. literalinclude:: ../example/datastore/bitget.py
 
 KuCoin
 ~~~~~~
 
 .. literalinclude:: ../example/datastore/kucoin.py
+
+Helpers
+-------
+
+.. _GMOCoinHelper:
+
+GMO Coin
+~~~~~~~~
+
+:class:`.helpers.GMOCoinHelper` を利用したサンプルコードです。
+
+:meth:`~.helpers.GMOCoinHelper.manage_ws_token` を利用することで、`Private WebSocket のアクセストークン <https://api.coin.z.com/docs/#ws-auth-post>`_ を管理します。
+デフォルトでは 5 分ごとにアクセストークンを延長します。 延長が失敗した場合は、アクセストークンを新しく作成します。
+このメソッドは無限ループとなっているので、 :meth:`asyncio.create_task` でタスクとしてスケジュールしてください。
+
+以下は適当なチャンネルを購読して、アクセストークン管理ヘルパーのタスクをスケジュールするサンプルコードです。
+
+.. literalinclude:: ../example/helpers/gmocoin.py
```

### Comparing `pybotters-1.1.1/docs/exchanges.rst` & `pybotters-1.2.0/docs/exchanges.rst`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,27 @@
 * API 認証情報
     * ``{"gmocoin": ["API_KEY", "API_SERCRET"]}``
 * HTTP 認証
     HTTP リクエスト時に取引所が定める認証情報が自動設定されます。
 
     https://api.coin.z.com/docs/#authentication-private
 * WebSocket 認証
-    GMO Coin はトークン認証方式の為、ユーザーコードで URL に「アクセストークン」含める必要があります。
+    GMO Coin はトークン認証方式です。
 
     https://api.coin.z.com/docs/#authentication-private-ws
 
-    ただし :class:`.GMOCoinDataStore` に「アクセストークン」を管理する機能があります。
+    :class:`.helpers.GMOCoinHelper` には「アクセストークン」を管理する機能があります。
 
-    :meth:`.GMOCoinDataStore.initialize` は「アクセストークンを取得」の POST リクエストに対応しています。
-    これにより「アクセストークン」が属性 :attr:`.GMOCoinDataStore.token` に格納されます。
-    この属性を利用するとトークン付き URL を構築するのに便利です。
+    :class:`.helpers.GMOCoinHelper` を利用すると「アクセストークンを延長」と「アクセストークンを取得」を自動で実行します。
+    さらに取得したアクセストークンから Private WebSocket URL を構築して :attr:`.WebSocketApp.url` を自動で更新します。
+    通常、 `GMO コインの定期メンテナンス <https://support.coin.z.com/hc/ja/articles/115007815487-%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E3%83%A1%E3%83%B3%E3%83%86%E3%83%8A%E3%83%B3%E3%82%B9%E6%99%82%E9%96%93%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6%E6%95%99%E3%81%88%E3%81%A6%E3%81%8F%E3%81%A0%E3%81%95%E3%81%84>`_
+    後はアクセストークンは失効して Private WebSocket の再接続は失敗してしまいます。
+    このヘルパーを使うと、失効したアクセストークンを自動で再取得するので、メンテナンス後の再接続を確立するのに便利です。
 
-    また DataStore 側で「アクセストークンを延長」の定期リクエストが有効になる為、ユーザーコードでの延長処理は不要です。
+    利用可能なコードは :ref:`Examples GMOCoinHelper <GMOCoinHelper>` をご覧ください。
 
 WebSocket
 ~~~~~~~~~
 
 * レート制限
     pybotters は GMO コインの WebSocket API の購読レート制限に対応しています。
 
@@ -168,14 +170,18 @@
 
     https://bybit-exchange.github.io/docs/v5/guide#authentication
 * WebSocket 認証
     WebSocket 接続時に取引所が定める認証情報の WebSocket メッセージが自動送信されます。
 
     https://bybit-exchange.github.io/docs/v5/ws/connect#authentication
 
+    また Websocket Trade API におけるメッセージ送信では ``header`` オブジェクトにタイムスタンプ ``X-BAPI-TIMESTAMP`` が自動付与されます。
+
+    https://bybit-exchange.github.io/docs/v5/websocket/trade/guideline
+
 WebSocket
 ~~~~~~~~~
 
 * Ping-Pong
     取引所が定める Ping-Pong メッセージが自動送信されます。
 
     https://bybit-exchange.github.io/docs/v5/ws/connect#how-to-send-the-heartbeat-packet
```

### Comparing `pybotters-1.1.1/docs/favicon.ico` & `pybotters-1.2.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/index.rst` & `pybotters-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/logo.png` & `pybotters-1.2.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/logo_150.png` & `pybotters-1.2.0/docs/logo_150.png`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/make.bat` & `pybotters-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/reference.rst` & `pybotters-1.2.0/docs/reference.rst`

 * *Files 8% similar despite different names*

```diff
@@ -75,7 +75,16 @@
 -------------
 
 .. autosummary::
    :toctree: generated
 
    pybotters.StoreChange
    pybotters.StoreStream
+
+
+Helpers
+-------
+
+.. autosummary::
+   :toctree: generated
+
+   pybotters.helpers.GMOCoinHelper
```

### Comparing `pybotters-1.1.1/docs/user-guide.rst` & `pybotters-1.2.0/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/_templates/autosummary/class.rst` & `pybotters-1.2.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/docs/_templates/autosummary/module.rst` & `pybotters-1.2.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/binance.py` & `pybotters-1.2.0/example/datastore/binance.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/bitbank.py` & `pybotters-1.2.0/example/datastore/bitbank.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/bitflyer.py` & `pybotters-1.2.0/example/datastore/bitflyer.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/bitget.py` & `pybotters-1.2.0/example/datastore/bitget.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/bybit.py` & `pybotters-1.2.0/example/datastore/bybit.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/coincheck.py` & `pybotters-1.2.0/example/datastore/coincheck.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/gmocoin.py` & `pybotters-1.2.0/example/datastore/gmocoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/kucoin.py` & `pybotters-1.2.0/example/datastore/kucoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/okx.py` & `pybotters-1.2.0/example/datastore/okx.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/datastore/phemex.py` & `pybotters-1.2.0/example/datastore/phemex.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/example/trading-bot/bitflyer.py` & `pybotters-1.2.0/example/trading-bot/bitflyer.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/__init__.py` & `pybotters-1.2.0/pybotters/__init__.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/auth.py` & `pybotters-1.2.0/pybotters/auth.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/client.py` & `pybotters-1.2.0/pybotters/client.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/request.py` & `pybotters-1.2.0/pybotters/request.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/store.py` & `pybotters-1.2.0/pybotters/store.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/ws.py` & `pybotters-1.2.0/pybotters/ws.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,14 +190,16 @@
         hdlr_json: list[WsJsonHandler],
         **kwargs: Any,
     ) -> None:
         async with self._session.ws_connect(self._url, autoping=False, **kwargs) as ws:
             self._current_ws = ws
             self._event.set()
 
+            await ws._wait_authtask()
+
             await self._ws_send(ws, send_str, send_bytes, send_json)
 
             await self._ws_receive(ws, hdlr_str, hdlr_bytes, hdlr_json)
 
     async def _ws_send(
         self,
         ws: ClientWebSocketResponse,
@@ -385,18 +387,15 @@
 
         expires = int((time.time() + 5.0) * 1000)
         path = f"GET/realtime{expires}"
         signature = hmac.new(
             secret, path.encode(), digestmod=hashlib.sha256
         ).hexdigest()
 
-        await ws.send_json(
-            {"op": "auth", "args": [key, expires, signature]},
-            _itself=True,
-        )
+        await ws.send_json({"op": "auth", "args": [key, expires, signature]})
         async for msg in ws:
             data = msg.json()
             if data.get("op") == "auth":
                 if not data.get("success"):
                     logger.warning(data)
                 break
 
@@ -420,16 +419,15 @@
                 "params": {
                     "api_key": key,
                     "timestamp": timestamp,
                     "nonce": nonce,
                     "signature": sign,
                 },
                 "id": "auth",
-            },
-            _itself=True,
+            }
         )
         async for msg in ws:
             data = msg.json()
             if data.get("id") == "auth":
                 if "error" in data:
                     logger.warning(data)
                 break
@@ -448,15 +446,15 @@
             secret, f"{key}{expiry}".encode(), digestmod=hashlib.sha256
         ).hexdigest()
         msg = {
             "method": "user.auth",
             "params": ["API", key, signature, expiry],
             "id": 123,
         }
-        await ws.send_json(msg, _itself=True)
+        await ws.send_json(msg)
         async for msg in ws:
             data = msg.json()
             if data.get("id") == 123:
                 if data.get("error"):
                     logger.warning(data)
                 break
 
@@ -484,15 +482,15 @@
                     "apiKey": key,
                     "passphrase": passphrase,
                     "timestamp": timestamp,
                     "sign": sign,
                 }
             ],
         }
-        await ws.send_json(msg, _itself=True)
+        await ws.send_json(msg)
         async for msg in ws:
             try:
                 data = msg.json()
             except json.JSONDecodeError:
                 pass
             else:
                 event = data.get("event")
@@ -527,15 +525,15 @@
                     "api_key": key,
                     "passphrase": passphrase,
                     "timestamp": str(timestamp),
                     "sign": sign,
                 }
             ],
         }
-        await ws.send_json(msg, _itself=True)
+        await ws.send_json(msg)
         async for msg in ws:
             try:
                 data = msg.json()
             except json.JSONDecodeError:
                 pass
             else:
                 event = data.get("event")
@@ -563,15 +561,15 @@
             "method": "login",
             "param": {
                 "apiKey": key,
                 "reqTime": timestamp,
                 "signature": sign,
             },
         }
-        await ws.send_json(msg, _itself=True)
+        await ws.send_json(msg)
 
 
 @dataclass
 class Item:
     name: str
     func: Any
 
@@ -650,18 +648,14 @@
         if self._response.url.host not in RequestLimitHosts.items:
             await super().send_str(*args, **kwargs)
         else:
             super_send_str = super().send_str(*args, **kwargs)
             await RequestLimitHosts.items[self._response.url.host](self, super_send_str)
 
     async def send_json(self, *args, **kwargs) -> None:
-        _itself = kwargs.pop("_itself", False)
-        if not _itself:
-            await self._wait_authtask()
-
         if (
             (kwargs.pop("auth", _Auth) is _Auth)
             and (self._response.url.host in MessageSignHosts.items)
             and (
                 MessageSignHosts.items[self._response.url.host].name
                 in self._response._session.__dict__["_apis"]
             )
@@ -740,13 +734,23 @@
         params["timestamp"] = int(time.time() * 1000)
         payload = "&".join(
             [f"{param}={value}" for param, value in sorted(params.items())]
         )
         signature = hmac.new(secret, payload.encode(), hashlib.sha256).hexdigest()
         params["signature"] = signature
 
+    @staticmethod
+    def bybit(ws: aiohttp.ClientWebSocketResponse, data: dict[str, Any]):
+        if "trade" not in ws._response.url.parts:
+            return
+
+        if "header" not in data:
+            data["header"] = {"X-BAPI-TIMESTAMP": str(int(time.time() * 1000))}
+
 
 class MessageSignHosts:
     items = {
         "ws-api.binance.com": Item("binance", MessageSign.binance),
         "testnet.binance.vision": Item("binancespot_testnet", MessageSign.binance),
+        "stream.bybit.com": Item("bybit", MessageSign.bybit),
+        "stream-testnet.bybit.com": Item("bybit_testnet", MessageSign.bybit),
     }
```

### Comparing `pybotters-1.1.1/pybotters/models/binance.py` & `pybotters-1.2.0/pybotters/models/binance.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/bitbank.py` & `pybotters-1.2.0/pybotters/models/bitbank.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/bitflyer.py` & `pybotters-1.2.0/pybotters/models/bitflyer.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/bitget.py` & `pybotters-1.2.0/pybotters/models/bitget.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/bitmex.py` & `pybotters-1.2.0/pybotters/models/bitmex.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/bybit.py` & `pybotters-1.2.0/pybotters/models/bybit.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/coincheck.py` & `pybotters-1.2.0/pybotters/models/coincheck.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/gmocoin.py` & `pybotters-1.2.0/pybotters/models/gmocoin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import logging
+import warnings
 from typing import Awaitable
 
 import aiohttp
 
 from pybotters.store import DataStore, DataStoreCollection
 from pybotters.typedefs import Item
 
@@ -126,26 +127,25 @@
         self._create("ticker", datastore_class=TickerStore)
         self._create("orderbooks", datastore_class=OrderBookStore)
         self._create("trades", datastore_class=TradeStore)
         self._create("orders", datastore_class=OrderStore)
         self._create("positions", datastore_class=PositionStore)
         self._create("executions", datastore_class=ExecutionStore)
         self._create("position_summary", datastore_class=PositionSummaryStore)
-        self.token: str | None = None
+        self.token: str | None = None  # DeprecationWarning
 
     async def initialize(self, *aws: Awaitable[aiohttp.ClientResponse]) -> None:
         """Initialize DataStore from HTTP response data.
 
         対応エンドポイント
 
         - GET /private/v1/latestExecutions (:attr:`.CoincheckDataStore.executions`)
         - GET /private/v1/activeOrders (:attr:`.CoincheckDataStore.orders`)
         - GET /private/v1/openPositions (:attr:`.CoincheckDataStore.positions`)
         - GET /private/v1/positionSummary (:attr:`.CoincheckDataStore.position_summary`)
-        - POST /private/v1/ws-auth (:attr:`.CoincheckDataStore.token`)
         """
         for f in asyncio.as_completed(aws):
             resp = await f
             data = await resp.json()
 
             if data.get("status") != 0:
                 raise ValueError(
@@ -164,15 +164,22 @@
             if resp.url.path == "/private/v1/openPositions" and "list" in data["data"]:
                 self.positions._onresponse(data["data"]["list"])
             if (
                 resp.url.path == "/private/v1/positionSummary"
                 and "list" in data["data"]
             ):
                 self.position_summary._onresponse(data["data"]["list"])
-            if resp.url.path == "/private/v1/ws-auth":
+            if resp.url.path == "/private/v1/ws-auth":  # DeprecationWarning
+                warnings.warn(
+                    "Initializing `POST /private/v1/ws-auth` with this method is deprecated. "
+                    "Please migrate to helpers.GMOCoinHelper.",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+
                 self.token = data["data"]
                 asyncio.create_task(self._token(resp.__dict__["_raw_session"]))
 
     def _onmessage(self, msg: Item, ws: ClientWebSocketResponse) -> None:
         if "error" in msg:
             logger.warning(msg)
         if "channel" in msg:
@@ -191,15 +198,15 @@
             elif channel == "orderEvents":
                 self.orders._onmessage(msg)
             elif channel == "positionEvents":
                 self.positions._onmessage(msg)
             elif channel == "positionSummaryEvents":
                 self.position_summary._onmessage(msg)
 
-    async def _token(self, session: aiohttp.ClientSession):
+    async def _token(self, session: aiohttp.ClientSession):  # DeprecationWarning
         while not session.closed:
             await session.put(
                 "https://api.coin.z.com/private/v1/ws-auth",
                 data={"token": self.token},
                 auth=Auth,
             )
             await asyncio.sleep(1800.0)  # 30 minutes
```

### Comparing `pybotters-1.1.1/pybotters/models/kucoin.py` & `pybotters-1.2.0/pybotters/models/kucoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/okx.py` & `pybotters-1.2.0/pybotters/models/okx.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/phemex.py` & `pybotters-1.2.0/pybotters/models/phemex.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pybotters/models/legacy/gmocoin.py` & `pybotters-1.2.0/pybotters/models/legacy/gmocoin.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/tests/test_auth.py` & `pybotters-1.2.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/tests/test_client.py` & `pybotters-1.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/tests/test_request.py` & `pybotters-1.2.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/tests/test_store.py` & `pybotters-1.2.0/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/tests/test_ws.py` & `pybotters-1.2.0/tests/test_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import functools
 import json
 import logging
+import sys
 from unittest.mock import ANY, AsyncMock, MagicMock, PropertyMock, call
 
 import aiohttp
 import pytest
 import pytest_asyncio
 import pytest_mock
 from aiohttp import web
@@ -248,14 +249,15 @@
 
     assert list(m_ws_connect.call_args) == [
         tuple([websocketapp._url]),
         dict(autoping=False, heartbeat=10.0),
     ]
     assert websocketapp._event.is_set()
 
+    assert m_wsresp._wait_authtask.call_args == call()
     assert m_wsresp.send_str.call_args == call("spam")
     assert m_wsresp.send_bytes.call_args == call(b"egg")
     assert m_wsresp.send_json.call_args == call({"bacon": "tomato"})
 
     assert hdlr_str.call_args_list == [
         call('{"spam":"egg"}', m_wsresp),
         call("__TEXT__", m_wsresp),
@@ -564,15 +566,15 @@
         autoping=True,
         loop=asyncio.get_running_loop(),
     )
 
     assert m_auth.called is expected["called"]
     if expected["called"]:
         assert m_auth.call_args == call(wsresp)
-        await asyncio.wait_for(wsresp.__dict__["_authtask"], timeout=5.0)
+        await asyncio.wait_for(wsresp._wait_authtask(), timeout=5.0)
         assert wsresp.__dict__["_authtask"].done()
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     (
         "test_input",
@@ -611,40 +613,32 @@
     if expected:
         assert m_ratelimit.call_args == call(wsresp, ANY)
         # Avoid the "coroutine was never awaited" warning
         await m_ratelimit.call_args.args[1]
 
 
 @pytest.mark.asyncio
-async def test_wsresponse_send_json_itself(mocker: pytest_mock.MockerFixture):
-    m_auth = AsyncMock()
-    items = {
-        "example.com": pybotters.ws.Item("example", m_auth),
-    }
-    mocker.patch.object(pybotters.ws.AuthHosts, "items", items)
+async def test_wsresponse_send_json():
     m_resp = MagicMock()
-    m_resp.__dict__["_auth"] = pybotters.auth.Auth
-    m_resp.url = URL("ws://example.com")
-    m_resp._session.__dict__["_apis"] = {"example": ["KEY", b"SECRET"]}
+    m_resp._auth = None
+    m_writer = AsyncMock()
 
     wsresp = pybotters.ws.ClientWebSocketResponse(
         reader=AsyncMock(),
-        writer=AsyncMock(),
+        writer=m_writer,
         protocol=None,
         response=m_resp,
         timeout=10.0,
         autoclose=True,
         autoping=True,
         loop=asyncio.get_running_loop(),
     )
-    await asyncio.wait_for(wsresp.send_json({"foo": "bar"}, _itself=False), timeout=5.0)
+    await asyncio.wait_for(wsresp.send_json({"foo": "bar"}), timeout=5.0)
 
-    assert m_auth.called
-    assert m_auth.call_args == call(wsresp)
-    assert wsresp.__dict__["_authtask"].done()
+    assert m_writer.send.call_args == call('{"foo": "bar"}', binary=ANY, compress=ANY)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     (
         "test_input",
         "expected",
@@ -854,16 +848,15 @@
                     {
                         "op": "auth",
                         "args": [
                             "77SQfUG7X33JhYZ3Jswpx5To",
                             2085848901000,
                             "a8bcd91ad5f8efdaefaf4ca6f38e551d739d6b42c2b54c85667fb181ecbc29a4",
                         ],
-                    },
-                    _itself=True,
+                    }
                 ),
                 "records": [],
             },
         ),
         # signed - testnet
         (
             {
@@ -888,16 +881,15 @@
                     {
                         "op": "auth",
                         "args": [
                             "77SQfUG7X33JhYZ3Jswpx5To",
                             2085848901000,
                             "a8bcd91ad5f8efdaefaf4ca6f38e551d739d6b42c2b54c85667fb181ecbc29a4",
                         ],
-                    },
-                    _itself=True,
+                    }
                 ),
                 "records": [],
             },
         ),
         # invalid signature
         (
             {
@@ -922,16 +914,15 @@
                     {
                         "op": "auth",
                         "args": [
                             "77SQfUG7X33JhYZ3Jswpx5To",
                             2085848901000,
                             "a8bcd91ad5f8efdaefaf4ca6f38e551d739d6b42c2b54c85667fb181ecbc29a4",
                         ],
-                    },
-                    _itself=True,
+                    }
                 ),
                 "records": [("pybotters.ws", logging.WARNING, ANY)],
             },
         ),
         # not signed
         (
             {
@@ -1049,16 +1040,15 @@
                 "timestamp": 2085848896000,
                 "nonce": "d73b41172d6deca2285e8e58533db082",
                 "signature": (
                     "f47526dec80c4773815fb1121058c2e3bcc531d1224b683e8babf76e52b0ba9c"
                 ),
             },
             "id": "auth",
-        },
-        _itself=True,
+        }
     )
     assert caplog.record_tuples == expected["records"]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     (
@@ -1167,18 +1157,47 @@
             "params": [
                 "API",
                 "9kYxQXZ6PrR8h17lsVdDcpnJ",
                 "196f317edfa0662ec3d388099683b40a25607919ca3546b131108b9ee5cbed4a",
                 2085848956,
             ],
             "id": 123,
-        },
-        _itself=True,
+        }
     )
-    assert caplog.record_tuples == expected["records"]
+
+    # NOTE: Unresolvable CI error, Unclosed client session ... Bug ?
+
+    if sys.version_info >= (3, 9):
+        assert caplog.record_tuples == expected["records"]
+    else:
+        assert [x for x in caplog.record_tuples if x[0] == "pybotters.ws"] == expected[
+            "records"
+        ]
+
+    # >       assert caplog.record_tuples == expected["records"]
+    # E       AssertionError: assert [('asyncio', ...f8c5ba91f0>')] == []
+    # E
+    # E         Left contains one more item: ('asyncio', 40, 'Unclosed client session\nclient_session: <aiohttp.client.ClientSession object at 0x7ff8c5ba91f0>')
+    # E
+    # E         Full diff:
+    # E         - []
+    # E         + [
+    # E         +     (
+    # E         +         'asyncio',
+    # E         +         40,
+    # E         +         'Unclosed client session\n'
+    # E         +         'client_session: <aiohttp.client.ClientSession object at '
+    # E         +         '0x7ff8c5ba91f0>',
+    # E         +     ),
+    # E         + ]
+
+    # tests/test_ws.py:1169: AssertionError
+    # ------------------------------ Captured log call -------------------------------
+    # ERROR    asyncio:base_events.py:1707 Unclosed client session
+    # client_session: <aiohttp.client.ClientSession object at 0x7ff8c5ba91f0>
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     (
         "test_input",
         "expected",
@@ -1298,16 +1317,15 @@
                 {
                     "apiKey": "gYmX9fr0kqqxptUlDKESxetg",
                     "passphrase": "MyPassphrase123",
                     "timestamp": "2085848896",
                     "sign": "6QVd7Mgd70We2/oDJr0+KnqxXZ+Gf1zIIl3qJk/Pqx8=",
                 }
             ],
-        },
-        _itself=True,
+        }
     )
     assert caplog.record_tuples == expected["records"]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     (
@@ -1380,16 +1398,15 @@
                 {
                     "api_key": "jbcfbye8AJzXxXwMKluXM12t",
                     "passphrase": "MyPassphrase123",
                     "timestamp": "2085848896",
                     "sign": "RmRhCixsMce8H7j2uyvR6sk11tCRbYenohbd87nchH8=",
                 }
             ],
-        },
-        _itself=True,
+        }
     )
     assert caplog.record_tuples == expected["records"]
 
 
 @pytest.mark.asyncio
 async def test_auth_mexc_ws(mocker: pytest_mock.MockerFixture):
     mocker.patch("time.time", return_value=2085848896.0)
@@ -1409,16 +1426,15 @@
         {
             "method": "login",
             "param": {
                 "apiKey": "0uVJRVNmR2ZHiCXtf6yEwrwy",
                 "reqTime": "2085848896",
                 "signature": "cd92edf98d52d973e96ffdce6f845c930f9900c5e4aa47ca4ef81d80533ab882",
             },
-        },
-        _itself=True,
+        }
     )
 
 
 @pytest.mark.asyncio
 async def test_ratelimit_gmocoin(mocker: pytest_mock.MockerFixture):
     m_sleep = mocker.patch("asyncio.sleep")
 
@@ -1571,7 +1587,111 @@
         ),
     }
     m_wsresp._response.url = test_input["url"]
 
     pybotters.ws.MessageSign.binance(m_wsresp, test_input["data"])
 
     assert test_input["data"] == expected["data"]
+
+
+@pytest.mark.parametrize(
+    ("test_input", "expected"),
+    [
+        # testnet
+        (
+            {
+                "url": URL("wss://stream-testnet.bybit.com/v5/trade"),
+                "data": {
+                    "op": "order.create",
+                    "args": [
+                        {
+                            "symbol": "ETHUSDT",
+                            "side": "Buy",
+                            "orderType": "Limit",
+                            "qty": "0.2",
+                            "price": "2800",
+                            "category": "linear",
+                            "timeInForce": "PostOnly",
+                        }
+                    ],
+                },
+            },
+            {
+                "data": {
+                    "op": "order.create",
+                    "args": [
+                        {
+                            "symbol": "ETHUSDT",
+                            "side": "Buy",
+                            "orderType": "Limit",
+                            "qty": "0.2",
+                            "price": "2800",
+                            "category": "linear",
+                            "timeInForce": "PostOnly",
+                        }
+                    ],
+                    "header": {
+                        "X-BAPI-TIMESTAMP": "2085848896000",
+                    },
+                }
+            },
+        ),
+        # mainnet
+        (
+            {
+                "url": URL("wss://stream.bybit.com/v5/trade"),
+                "data": {
+                    "op": "order.create",
+                    "args": [
+                        {
+                            "symbol": "ETHUSDT",
+                            "side": "Buy",
+                            "orderType": "Limit",
+                            "qty": "0.2",
+                            "price": "2800",
+                            "category": "linear",
+                            "timeInForce": "PostOnly",
+                        }
+                    ],
+                },
+            },
+            {
+                "data": {
+                    "op": "order.create",
+                    "args": [
+                        {
+                            "symbol": "ETHUSDT",
+                            "side": "Buy",
+                            "orderType": "Limit",
+                            "qty": "0.2",
+                            "price": "2800",
+                            "category": "linear",
+                            "timeInForce": "PostOnly",
+                        }
+                    ],
+                    "header": {
+                        "X-BAPI-TIMESTAMP": "2085848896000",
+                    },
+                }
+            },
+        ),
+        # not /v5/trade
+        (
+            {
+                "url": URL("wss://stream.bybit.com/v5/private"),
+                "data": {"op": "ping"},
+            },
+            {
+                "data": {"op": "ping"},
+            },
+        ),
+    ],
+)
+def test_msgsign_bybit(mocker: pytest_mock.MockerFixture, test_input, expected):
+    mocker.patch("time.time", return_value=2085848896.0)
+
+    m_wsresp = AsyncMock()
+    m_wsresp._response.url = test_input["url"]
+
+    pybotters.ws.MessageSign.bybit(m_wsresp, test_input["data"])
+
+    assert test_input["data"] == expected["data"]
```

### Comparing `pybotters-1.1.1/.gitignore` & `pybotters-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/LICENCE` & `pybotters-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/pyproject.toml` & `pybotters-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybotters-1.1.1/PKG-INFO` & `pybotters-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pybotters
-Version: 1.1.1
+Version: 1.2.0
 Summary: An advanced API client for python crypto bot traders
 Project-URL: Documentation, https://pybotters.readthedocs.io/ja/stable/
 Project-URL: Repository, https://github.com/pybotters/pybotters
 Author-email: MtkN1 <51289448+MtkN1@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: aiohttp,crypto,exchange,trading
```

