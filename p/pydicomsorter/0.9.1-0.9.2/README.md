# Comparing `tmp/pydicomsorter-0.9.1.tar.gz` & `tmp/pydicomsorter-0.9.2.tar.gz`

## Comparing `pydicomsorter-0.9.1.tar` & `pydicomsorter-0.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0   237059 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/pixi.lock
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/mkdocs.yaml
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/releaserc.toml
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/ruff.toml
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/docs/index.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/cli.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/dicomsort.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/options.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/sandbox/dicomsort.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/tests/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/LICENSE
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/README.md
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   373889 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/pixi.lock
+-rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/config/releaserc.toml
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/config/ruff.toml
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/docs/index.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/cli.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/dicomsort.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/options.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/tests/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/README.md
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 pydicomsorter-0.9.2/PKG-INFO
```

### Comparing `pydicomsorter-0.9.1/.pre-commit-config.yaml` & `pydicomsorter-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/pixi.lock` & `pydicomsorter-0.9.2/pixi.lock`

 * *Files 18% similar despite different names*

```diff
@@ -919,14 +919,946 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.22.0-py312h01d794b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
+  py310:
+    channels:
+    - url: https://conda.anaconda.org/conda-forge/
+    indexes:
+    - https://pypi.org/simple
+    packages:
+      linux-64:
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.5.1-py310hc51659f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py310hc6cd4ac_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py310hff52083_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h77fa898_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h77fa898_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-hc0a3c3a_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py310h2372a71_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.10.14-hd12c33a_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.10-4_cp310.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.3-py310h6883aea_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py310h2372a71_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h75354e8_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/a6/a5/c351d83454267964d24b79e9116d716157071df4682f865d1274235a0cac/pydantic_core-2.18.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      osx-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.5.1-py310h56a41de_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py310h5daac23_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py310h2ec42d9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/krb5-1.21.2-hb884880_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-17.0.6-h88467a6_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py310hb372a2b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.10.14-h00d2728_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.10-4_cp310.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.3-py310he0bbd50_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py310hb372a2b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-hde137ed_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/d8/3d/ae9491c1f071f7f49c8bc7b161325e658ea53f72a12ec5fd7a4ea4fa01ee/pydantic_core-2.18.2-cp310-cp310-macosx_10_12_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      osx-arm64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.5.1-py310ha6dd24b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py310h692a8b6_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py310hbe9552e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/krb5-1.21.2-h92f50d5_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-17.0.6-h5f092b4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libedit-3.1.20191231-hc8eb9b7_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py310hd125d64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.10.14-h2469fbe_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.10-4_cp310.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.3-py310h16e08c9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py310hd125d64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zeromq-4.3.5-hcc0f68c_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/79/b8/8be6e21881344ab91df49dcd6f7ef34729c2868019f503699b2724f4195a/pydantic_core-2.18.2-cp310-cp310-macosx_11_0_arm64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      win-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.1-py310ha8f682b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py310h00ffb61_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyha63f2e9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh7428d3b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py310h5588dad_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/krb5-1.21.2-heb0366b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-h2466b09_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py310h8d17308_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.10.14-h4de0772_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.10-4_cp310.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py310h00ffb61_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.3-py310h656833d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py310h8d17308_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-ha32ba9b_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33135-h835141b_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33135-h22015db_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-he1f189c_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c0/94/55f5b643992a57a244f7f7119b5eabebe9e592c3c8282a132ac21c965812/pydantic_core-2.18.2-cp310-none-win_amd64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+  py311:
+    channels:
+    - url: https://conda.anaconda.org/conda-forge/
+    indexes:
+    - https://pypi.org/simple
+    packages:
+      linux-64:
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.5.1-py311h331c9d8_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py311hb755f60_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py311h38be061_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h77fa898_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h77fa898_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-hc0a3c3a_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py311h459d7ec_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.11.9-hb806964_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-4_cp311.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.3-py311h08a0b41_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py311h459d7ec_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h75354e8_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/80/b8/b93d756b36425f7ad378dcb9fdf5f6a03b88afaae0476f7bdb31dd8964be/pydantic_core-2.18.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      osx-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.5.1-py311h42a8b16_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py311hdd0406b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py311h6eed73b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/krb5-1.21.2-hb884880_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-17.0.6-h88467a6_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py311he705e18_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.11.9-h657bba9_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-4_cp311.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.3-py311h89e2aaa_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py311he705e18_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-hde137ed_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ce/9c/6ba3121fecd4c8a0ae48d87e02a87d97ec8831eb978c53bcbfa0b2e43600/pydantic_core-2.18.2-cp311-cp311-macosx_10_12_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      osx-arm64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.5.1-py311hd3f4193_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py311h92babd0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py311h267d04e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/krb5-1.21.2-h92f50d5_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-17.0.6-h5f092b4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libedit-3.1.20191231-hc8eb9b7_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py311h05b510d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.11.9-h932a869_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.11-4_cp311.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.3-py311h9bed540_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py311h05b510d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zeromq-4.3.5-hcc0f68c_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/5d/61/bfc32484eac102051ef85f5e648c9777f57398c83e5f87e3c0a420a6550b/pydantic_core-2.18.2-cp311-cp311-macosx_11_0_arm64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      win-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.1-py311he736701_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py311h12c1d0e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyha63f2e9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh7428d3b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py311h1ea47a8_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/krb5-1.21.2-heb0366b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-h2466b09_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py311ha68e1ae_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.11.9-h631f459_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-4_cp311.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py311h12c1d0e_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.3-py311h484c95c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py311ha68e1ae_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-ha32ba9b_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33135-h835141b_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33135-h22015db_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-he1f189c_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/9d/b0/e8bebe8fd08ea6ec027b7304c84f4652f2933514caf9f6a418d259d2a950/pydantic_core-2.18.2-cp311-none-win_amd64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+  py312:
+    channels:
+    - url: https://conda.anaconda.org/conda-forge/
+    indexes:
+    - https://pypi.org/simple
+    packages:
+      linux-64:
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.5.1-py312h9a8786e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py312h30efb56_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py312h7900ff3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.2-h659d440_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h77fa898_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h77fa898_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-hc0a3c3a_7.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.3-py312h8fd38d8_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h75354e8_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      osx-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.5.1-py312h520dd33_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py312hede676d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py312hb401068_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/krb5-1.21.2-hb884880_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-17.0.6-h88467a6_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.3-py312ha04878a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-hde137ed_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      osx-arm64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.5.1-py312h7e5086c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py312h20a0b95_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py312h81bd7bf_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/krb5-1.21.2-h92f50d5_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-17.0.6-h5f092b4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libedit-3.1.20191231-hc8eb9b7_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py312he37b823_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.3-py312hfa13136_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py312he37b823_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zeromq-4.3.5-hcc0f68c_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
+      win-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.1-py312h4389bb4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py312h53d5487_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyha63f2e9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.24.0-pyh7428d3b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py312h2e8e312_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/krb5-1.21.2-heb0366b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-h2466b09_3.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.3-py312hd7027bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-ha32ba9b_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33135-h835141b_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33135-h22015db_20.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-he1f189c_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
+      - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
+      - pypi: .
 packages:
 - kind: conda
   name: _libgcc_mutex
   version: '0.1'
   build: conda_forge
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
@@ -1497,14 +2429,172 @@
   purls:
   - pkg:pypi/comm?source=conda-forge-mapping
   size: 12134
   timestamp: 1710320435158
 - kind: conda
   name: coverage
   version: 7.5.1
+  build: py310h56a41de_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.5.1-py310h56a41de_0.conda
+  sha256: 2ee3619a6ec18fb195f3660639b740a6431db6c62812b04b37ef8ca6a79c608f
+  md5: 1240a91d7d13db8a6b4b64527a93b676
+  depends:
+  - __osx >=10.9
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - tomli
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/coverage?source=conda-forge-mapping
+  size: 289240
+  timestamp: 1714846882510
+- kind: conda
+  name: coverage
+  version: 7.5.1
+  build: py310ha6dd24b_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.5.1-py310ha6dd24b_0.conda
+  sha256: 010494a7d92a6582de5b9f27a1f0864f29476d98d33c5a9a3c9fd2e04a8dedb3
+  md5: 4a70ce624f79362577b8a2f6ea0a1735
+  depends:
+  - __osx >=11.0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - tomli
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/coverage?source=conda-forge-mapping
+  size: 289635
+  timestamp: 1714846937217
+- kind: conda
+  name: coverage
+  version: 7.5.1
+  build: py310ha8f682b_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.1-py310ha8f682b_0.conda
+  sha256: 7667b46829ac7ead2925f6c2ea8fca27eb7619df688647e244971a662e3d4209
+  md5: e28a9a8c6ef3d80712ceb3b86b9e2ad4
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - tomli
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/coverage?source=conda-forge-mapping
+  size: 307973
+  timestamp: 1714847190472
+- kind: conda
+  name: coverage
+  version: 7.5.1
+  build: py310hc51659f_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.5.1-py310hc51659f_0.conda
+  sha256: 56ce76f5687a397fcb5ac93282b1d82e1f30fa3fd7452e21ab84cafcd61e5716
+  md5: 64f82ee7706c57c55e61d267134786bf
+  depends:
+  - libgcc-ng >=12
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - tomli
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/coverage?source=conda-forge-mapping
+  size: 290906
+  timestamp: 1714846740685
+- kind: conda
+  name: coverage
+  version: 7.5.1
+  build: py311h331c9d8_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.5.1-py311h331c9d8_0.conda
+  sha256: 2ecb21dc0efec42419c50f63daf1db0d6910f47db1b2653ebc5c43f76302024e
+  md5: 9f35e13e3b9e05e153b78f42662061f6
+  depends:
+  - libgcc-ng >=12
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - tomli
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/coverage?source=conda-forge-mapping
+  size: 369007
+  timestamp: 1714846741185
+- kind: conda
+  name: coverage
+  version: 7.5.1
+  build: py311h42a8b16_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.5.1-py311h42a8b16_0.conda
+  sha256: d2ca14f7d750652eb3a4f7a674b5a8ce65bae3586a699b613a83e66d879eef5d
+  md5: 043b439c3c4ae4b8a91aba062ef27d10
+  depends:
+  - __osx >=10.9
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - tomli
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/coverage?source=conda-forge-mapping
+  size: 367115
+  timestamp: 1714846868088
+- kind: conda
+  name: coverage
+  version: 7.5.1
+  build: py311hd3f4193_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.5.1-py311hd3f4193_0.conda
+  sha256: 6eaa811402fc3433bd891179410a434d0826da1f44579eccccc9dbb632769403
+  md5: 81834421a20531c880f6c0a5342f3922
+  depends:
+  - __osx >=11.0
+  - python >=3.11,<3.12.0a0
+  - python >=3.11,<3.12.0a0 *_cpython
+  - python_abi 3.11.* *_cp311
+  - tomli
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/coverage?source=conda-forge-mapping
+  size: 368146
+  timestamp: 1714846963260
+- kind: conda
+  name: coverage
+  version: 7.5.1
+  build: py311he736701_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.1-py311he736701_0.conda
+  sha256: 844aea7ee1ff29d72f20406debb68b2e9bdd51f83299e6fb2e0b1f9b97e7e8e0
+  md5: 44beec11cad6c9cd78fdd3594d62817b
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - tomli
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/coverage?source=conda-forge-mapping
+  size: 385417
+  timestamp: 1714847169739
+- kind: conda
+  name: coverage
+  version: 7.5.1
   build: py312h4389bb4_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.1-py312h4389bb4_0.conda
   sha256: ce8f96da9dfbe0e3ed080fdcaa0a358639f8699e91742b99d3921a80f2ca39bc
   md5: 56d1519253eaf0ccd65fa26ec8b0fc60
   depends:
   - python >=3.12,<3.13.0a0
@@ -1613,14 +2703,174 @@
   license: GPL-2.0-or-later
   license_family: GPL
   size: 618596
   timestamp: 1640112124844
 - kind: conda
   name: debugpy
   version: 1.8.1
+  build: py310h00ffb61_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py310h00ffb61_0.conda
+  sha256: 070a4d308dace7903e749ed09177315265e6b2dab5d6bb6a0e853fa1fd2e3502
+  md5: 0496f1dc805c8a53a7be7fc2f5ca61cc
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy?source=conda-forge-mapping
+  - pkg:pypi/bytecode?source=conda-forge-mapping
+  size: 2812534
+  timestamp: 1707445209927
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py310h5daac23_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py310h5daac23_0.conda
+  sha256: 4d8e2f3019ed8f6141745d027d8a4f778dd71008848ee4bfaa81842da2e0b42f
+  md5: 3364c88f90fc0a8354a165f44dd9dd5c
+  depends:
+  - libcxx >=16
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy?source=conda-forge-mapping
+  - pkg:pypi/bytecode?source=conda-forge-mapping
+  size: 1866627
+  timestamp: 1707444787702
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py310h692a8b6_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py310h692a8b6_0.conda
+  sha256: 1da521b369006188c4a4326352664e7fff1cebf3ba6bfa3228a33e1f2cd64f59
+  md5: 18b44acb58f6d0b13d694067112545bf
+  depends:
+  - libcxx >=16
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy?source=conda-forge-mapping
+  - pkg:pypi/bytecode?source=conda-forge-mapping
+  size: 1852663
+  timestamp: 1707444865528
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py310hc6cd4ac_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py310hc6cd4ac_0.conda
+  sha256: 69d3970a9bb62d4e1e187f82248cc1cc924589c06100a6f1a065e063f4155978
+  md5: 1ea80564b80390fa25da16e4211eb801
+  depends:
+  - libgcc-ng >=12
+  - libstdcxx-ng >=12
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy?source=conda-forge-mapping
+  - pkg:pypi/bytecode?source=conda-forge-mapping
+  size: 1917514
+  timestamp: 1707444642761
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py311h12c1d0e_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py311h12c1d0e_0.conda
+  sha256: 22f390668ab9edc90132dba7a20e58949c12eb5d6f9cc6c0d3766bebdc0ec009
+  md5: 61fae6d8dae07c4384ea7672913be528
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy?source=conda-forge-mapping
+  - pkg:pypi/bytecode?source=conda-forge-mapping
+  size: 3243396
+  timestamp: 1707445208626
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py311h92babd0_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py311h92babd0_0.conda
+  sha256: bb6e0aa6b7ee46a1dc1145db94a30ccc6cb5db2bc59948a2baa8982a708dbb70
+  md5: a3d772ae41c1ef4ea1fa01daf307832c
+  depends:
+  - libcxx >=16
+  - python >=3.11,<3.12.0a0
+  - python >=3.11,<3.12.0a0 *_cpython
+  - python_abi 3.11.* *_cp311
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy?source=conda-forge-mapping
+  - pkg:pypi/bytecode?source=conda-forge-mapping
+  size: 2272457
+  timestamp: 1707444947065
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py311hb755f60_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py311hb755f60_0.conda
+  sha256: e69fe7d453389d54fa68fb6fb75ac85f882b2ab4bc745b02c7ff8cd83aee2a5b
+  md5: 17b98238cbbfbebacd46b79b7fc629a9
+  depends:
+  - libgcc-ng >=12
+  - libstdcxx-ng >=12
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy?source=conda-forge-mapping
+  - pkg:pypi/bytecode?source=conda-forge-mapping
+  size: 2302395
+  timestamp: 1707444677899
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py311hdd0406b_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py311hdd0406b_0.conda
+  sha256: 0df1ca336d468accadb2a1d617aac7c5a5c4c7d63d0d847ab237772f8ff1e93b
+  md5: 19779dab342c45f8acb28caa00b07637
+  depends:
+  - libcxx >=16
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy?source=conda-forge-mapping
+  - pkg:pypi/bytecode?source=conda-forge-mapping
+  size: 2241280
+  timestamp: 1707444917914
+- kind: conda
+  name: debugpy
+  version: 1.8.1
   build: py312h20a0b95_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py312h20a0b95_0.conda
   sha256: d8ae528ddf391511387bb4c67d7dd4ad3cb808ee9b093429379803cf58a13807
   md5: d850abbd9eeedbe2e734e397038f3f76
   depends:
   - libcxx >=16
@@ -2487,14 +3737,193 @@
   license: BSD-3-Clause
   license_family: BSD
   purls:
   - pkg:pypi/jupyter-client?source=conda-forge-mapping
   size: 106042
   timestamp: 1710255955150
 - kind: conda
+  name: jupyter_client
+  version: 8.6.2
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.2-pyhd8ed1ab_0.conda
+  sha256: 634f065cdd1d0aacd4bb6848ebf240dcebc8578135d65f4ad4aa42b2276c4e0c
+  md5: 3cdbb2fa84490e5fd44c9f9806c0d292
+  depends:
+  - importlib_metadata >=4.8.3
+  - jupyter_core >=4.12,!=5.0.*
+  - python >=3.8
+  - python-dateutil >=2.8.2
+  - pyzmq >=23.0
+  - tornado >=6.2
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-client?source=conda-forge-mapping
+  size: 106248
+  timestamp: 1716472312833
+- kind: conda
+  name: jupyter_core
+  version: 5.7.2
+  build: py310h2ec42d9_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py310h2ec42d9_0.conda
+  sha256: ab2f20f7532322b2393220846cad453ee47848491971ec306755e7c1010b4e0a
+  md5: cc37456f73db17d159de1b07a26e91cc
+  depends:
+  - platformdirs >=2.5
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-core?source=conda-forge-mapping
+  size: 80504
+  timestamp: 1710257739574
+- kind: conda
+  name: jupyter_core
+  version: 5.7.2
+  build: py310h5588dad_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py310h5588dad_0.conda
+  sha256: 220a6fe571d3e9a5b5f4467d7f2fb22080b96f7143c9b2703528032528338d50
+  md5: 6646c59c6c096e0b99c53dc9d3deaada
+  depends:
+  - platformdirs >=2.5
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - pywin32 >=300
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-core?source=conda-forge-mapping
+  size: 97082
+  timestamp: 1710257770270
+- kind: conda
+  name: jupyter_core
+  version: 5.7.2
+  build: py310hbe9552e_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py310hbe9552e_0.conda
+  sha256: 9e351b25482c50c49fdf0e2203e238c5f04fed0cf192e227915fec955c5d890f
+  md5: bd7737fbd26eecd0f39cafb52a956f9e
+  depends:
+  - platformdirs >=2.5
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-core?source=conda-forge-mapping
+  size: 80605
+  timestamp: 1710257888050
+- kind: conda
+  name: jupyter_core
+  version: 5.7.2
+  build: py310hff52083_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py310hff52083_0.conda
+  sha256: 837039256d39a249b5bec850f87948e1967c47c9e747056df8155d80c4d3b094
+  md5: cb92c27600d5716fd526a206aa43342c
+  depends:
+  - platformdirs >=2.5
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-core?source=conda-forge-mapping
+  size: 79565
+  timestamp: 1710257392136
+- kind: conda
+  name: jupyter_core
+  version: 5.7.2
+  build: py311h1ea47a8_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py311h1ea47a8_0.conda
+  sha256: 59a353a47826a4bf136dec1100c90604a6a9fd06f3c203da73d4ea8bbe359aab
+  md5: 191bcd5e85d4f305510e46893de9ae08
+  depends:
+  - platformdirs >=2.5
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - pywin32 >=300
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-core?source=conda-forge-mapping
+  size: 111749
+  timestamp: 1710257755792
+- kind: conda
+  name: jupyter_core
+  version: 5.7.2
+  build: py311h267d04e_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py311h267d04e_0.conda
+  sha256: 0606c9f5a0a9de1e3d8348df4639b7f9dc493a7cf641fd4e9c956af5a33d2b7a
+  md5: f9e296ff8724469af7117f453824a6de
+  depends:
+  - platformdirs >=2.5
+  - python >=3.11,<3.12.0a0
+  - python >=3.11,<3.12.0a0 *_cpython
+  - python_abi 3.11.* *_cp311
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-core?source=conda-forge-mapping
+  size: 96069
+  timestamp: 1710257757802
+- kind: conda
+  name: jupyter_core
+  version: 5.7.2
+  build: py311h38be061_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py311h38be061_0.conda
+  sha256: 49834d76e70d6461e19c265296b0f492578f63360d0e4799b06bbe2c0d018a7a
+  md5: f85e78497dfed6f6a4b865191f42de2e
+  depends:
+  - platformdirs >=2.5
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-core?source=conda-forge-mapping
+  size: 95226
+  timestamp: 1710257482063
+- kind: conda
+  name: jupyter_core
+  version: 5.7.2
+  build: py311h6eed73b_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py311h6eed73b_0.conda
+  sha256: 3078f27009ce1f3cdd46dc97bd4f3f51277aa5957f6a90e300c613bd848767b7
+  md5: 582fe977a5a6b9f37a72ff34a753381e
+  depends:
+  - platformdirs >=2.5
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/jupyter-core?source=conda-forge-mapping
+  size: 95661
+  timestamp: 1710257750738
+- kind: conda
   name: jupyter_core
   version: 5.7.2
   build: py312h2e8e312_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py312h2e8e312_0.conda
   sha256: bf2a315febec297e05fa77e39bd371d53553bd1c347e495ac34198fec18afb11
   md5: 3ed5c1981d05f125696f392407d36ce2
@@ -3588,14 +5017,34 @@
   license: Apache-2.0
   license_family: Apache
   size: 8330419
   timestamp: 1716288210872
 - kind: conda
   name: openssl
   version: 3.3.0
+  build: h2466b09_3
+  build_number: 3
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-h2466b09_3.conda
+  sha256: 11b2513fceb20102bdc7f7656a59005acb9ecd0886b7cbfb9c13c2c953f2429b
+  md5: d7fec5d3bb8fc0c8e266bf1ad350cec5
+  depends:
+  - ca-certificates
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
+  size: 8368468
+  timestamp: 1716471282135
+- kind: conda
+  name: openssl
+  version: 3.3.0
   build: h4ab18f5_2
   build_number: 2
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_2.conda
   sha256: e56d9121f553f16ef21d2664c569cd50336291fa1458be5e5c654553a43737e7
   md5: b8934d399b56d73e323403e183d009c5
   depends:
@@ -3606,14 +5055,32 @@
   license: Apache-2.0
   license_family: Apache
   size: 2894882
   timestamp: 1716285197781
 - kind: conda
   name: openssl
   version: 3.3.0
+  build: h4ab18f5_3
+  build_number: 3
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_3.conda
+  sha256: 33dcea0ed3a61b2de6b66661cdd55278640eb99d676cd129fbff3e53641fa125
+  md5: 12ea6d0d4ed54530eaed18e4835c1f7c
+  depends:
+  - ca-certificates
+  - libgcc-ng >=12
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
+  size: 2891147
+  timestamp: 1716468354865
+- kind: conda
+  name: openssl
+  version: 3.3.0
   build: h87427d6_2
   build_number: 2
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_2.conda
   sha256: 8a690c05bf3e1016a7dfc44d9b508e9883bbc7bcf5569e9e808c1e028ebb72ab
   md5: fa4859f58b1810d77089b0482c886da0
   depends:
@@ -3624,14 +5091,32 @@
   license: Apache-2.0
   license_family: Apache
   size: 2543706
   timestamp: 1716285526027
 - kind: conda
   name: openssl
   version: 3.3.0
+  build: h87427d6_3
+  build_number: 3
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_3.conda
+  sha256: 58ffbdce44ac18c6632a2ce1531d06e3fb2e855d40728ba3a2b709158b9a1c33
+  md5: ec504fefb403644d893adffb6e7a2dbe
+  depends:
+  - __osx >=10.13
+  - ca-certificates
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
+  size: 2542959
+  timestamp: 1716468436467
+- kind: conda
+  name: openssl
+  version: 3.3.0
   build: hfb2fe0b_2
   build_number: 2
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_2.conda
   sha256: 503b34722d53224c5ebbabd0ffba2681287a810f9b129adb717dc6f6eb193752
   md5: c9602073e34599f40b8c4ce9e19cabf6
   depends:
@@ -3640,14 +5125,32 @@
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
   size: 2892345
   timestamp: 1716285397137
 - kind: conda
+  name: openssl
+  version: 3.3.0
+  build: hfb2fe0b_3
+  build_number: 3
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_3.conda
+  sha256: 6f41c163ab57e7499dff092be4498614651f0f6432e12c2b9f06859a8bc39b75
+  md5: 730f618b008b3c13c1e3f973408ddd67
+  depends:
+  - __osx >=11.0
+  - ca-certificates
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
+  size: 2893954
+  timestamp: 1716468329572
+- kind: conda
   name: packaging
   version: '24.0'
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
   sha256: a390182d74c31dfd713c16db888c92c277feeb6d1fe96ff9d9c105f9564be48a
@@ -3820,14 +5323,160 @@
   purls:
   - pkg:pypi/prompt-toolkit?source=conda-forge-mapping
   size: 270398
   timestamp: 1702399557137
 - kind: conda
   name: psutil
   version: 5.9.8
+  build: py310h2372a71_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py310h2372a71_0.conda
+  sha256: f1866425aa67f3fe1e3f6e07562a4bc986fd487e01146a91eb1bdbe5ec16a836
+  md5: bd19b3096442ea342c4a5208379660b1
+  depends:
+  - libgcc-ng >=12
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
+  size: 368328
+  timestamp: 1705722544490
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py310h8d17308_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py310h8d17308_0.conda
+  sha256: f1ec2d213b2a45831ede5d794eb5c4d5adf072f24d12eb6f07df207bcc9de0fb
+  md5: f85b83fad1e1c12c212f27039f823138
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
+  size: 386373
+  timestamp: 1705722865736
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py310hb372a2b_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py310hb372a2b_0.conda
+  sha256: 6c52cb3ea7e9e42a9fe2e2ddf9d91093fb13f067982878edc96035601ff477c0
+  md5: ec3a8263961880a89f9587670aad5c81
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
+  size: 375259
+  timestamp: 1705722685866
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py310hd125d64_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py310hd125d64_0.conda
+  sha256: 8d303673271d8a32a79956a5cf7b941a5fa4f9ef7f093a29efc871a6c8e69aa4
+  md5: 0fb7c0c32b4212cc783aa315ea4fc173
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
+  size: 376671
+  timestamp: 1705722806535
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py311h05b510d_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py311h05b510d_0.conda
+  sha256: 2b6e485c761fa3e7271c44a070c0d08e79a6758ac4d7a660eaff0ed0a60c6f2b
+  md5: 970ef0edddc6c2cfeb16b7225a28a1f4
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python >=3.11,<3.12.0a0 *_cpython
+  - python_abi 3.11.* *_cp311
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
+  size: 513415
+  timestamp: 1705722847446
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py311h459d7ec_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py311h459d7ec_0.conda
+  sha256: 467788418a2c71fb3df9ac0a6282ae693d1070a6cb47cb59bdb529b53acaee1c
+  md5: 9bc62d25dcf64eec484974a3123c9d57
+  depends:
+  - libgcc-ng >=12
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
+  size: 505516
+  timestamp: 1705722586221
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py311ha68e1ae_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py311ha68e1ae_0.conda
+  sha256: 77760f2ce0d2be9339d94d0fb5b3d102659355563f5b6471a1231525e63ff581
+  md5: 17e48538806e7c682d2ffcbd5c9f9aa0
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
+  size: 520242
+  timestamp: 1705723070638
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py311he705e18_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py311he705e18_0.conda
+  sha256: fcff83f4d265294b54821656a10be62421da377885ab2e9811a80eb76419b3fe
+  md5: 31aa294c58b3058c179a7a9593e99e18
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
+  size: 513371
+  timestamp: 1705722716862
+- kind: conda
+  name: psutil
+  version: 5.9.8
   build: py312h41838bb_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
   sha256: 12e5053d19bddaf7841e59cbe9ba98fa5d4d8502ceccddad80888515e1366107
   md5: 03926e7089a5e61b77043b470ae7b553
   depends:
   - python >=3.12,<3.13.0a0
@@ -3982,14 +5631,22 @@
   sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
+  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
   url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
   sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
@@ -3998,16 +5655,72 @@
   sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
+  url: https://files.pythonhosted.org/packages/c0/94/55f5b643992a57a244f7f7119b5eabebe9e592c3c8282a132ac21c965812/pydantic_core-2.18.2-cp310-none-win_amd64.whl
+  sha256: e23ec367a948b6d812301afc1b13f8094ab7b2c280af66ef450efc357d2ae543
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/79/b8/8be6e21881344ab91df49dcd6f7ef34729c2868019f503699b2724f4195a/pydantic_core-2.18.2-cp310-cp310-macosx_11_0_arm64.whl
+  sha256: f0a21cbaa69900cbe1a2e7cad2aa74ac3cf21b10c3efb0fa0b80305274c0e8a2
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/a6/a5/c351d83454267964d24b79e9116d716157071df4682f865d1274235a0cac/pydantic_core-2.18.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 553ef617b6836fc7e4df130bb851e32fe357ce36336d897fd6646d6058d980af
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/d8/3d/ae9491c1f071f7f49c8bc7b161325e658ea53f72a12ec5fd7a4ea4fa01ee/pydantic_core-2.18.2-cp310-cp310-macosx_10_12_x86_64.whl
+  sha256: 9e08e867b306f525802df7cd16c44ff5ebbe747ff0ca6cf3fde7f36c05a59a81
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/9d/b0/e8bebe8fd08ea6ec027b7304c84f4652f2933514caf9f6a418d259d2a950/pydantic_core-2.18.2-cp311-none-win_amd64.whl
+  sha256: 800d60565aec896f25bc3cfa56d2277d52d5182af08162f7954f938c06dc4ee3
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/80/b8/b93d756b36425f7ad378dcb9fdf5f6a03b88afaae0476f7bdb31dd8964be/pydantic_core-2.18.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 470b94480bb5ee929f5acba6995251ada5e059a5ef3e0dfc63cca287283ebfa6
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/ce/9c/6ba3121fecd4c8a0ae48d87e02a87d97ec8831eb978c53bcbfa0b2e43600/pydantic_core-2.18.2-cp311-cp311-macosx_10_12_x86_64.whl
+  sha256: 219da3f096d50a157f33645a1cf31c0ad1fe829a92181dd1311022f986e5fbe3
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/5d/61/bfc32484eac102051ef85f5e648c9777f57398c83e5f87e3c0a420a6550b/pydantic_core-2.18.2-cp311-cp311-macosx_11_0_arm64.whl
+  sha256: cc1cfd88a64e012b74e94cd00bbe0f9c6df57049c97f02bb07d39e9c852e19a4
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: conda
   name: pydantic-core
   version: 2.18.2
   build: py312h2615798_0
@@ -4104,23 +5817,23 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.9.1
+  version: 0.9.2
   path: .
-  sha256: 3ff057f04884da1a7268b9a059201795eec8ae7974486f37474e649f80299824
+  sha256: cfa693fc7710ece488449147ea350b572d224caeef4431ee7d05e771daea9291
   requires_dist:
   - rich
   - rich-click
   - pydicom
   - pydantic
-  requires_python: '>=3.12'
+  requires_python: '>=3.10'
   editable: true
 - kind: pypi
   name: pygments
   version: 2.18.0
   url: https://files.pythonhosted.org/packages/f7/3f/01c8b82017c199075f8f788d0d906b9ffbbc5a47dc9918a945e13d5a2bda/pygments-2.18.0-py3-none-any.whl
   sha256: b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
   requires_dist:
@@ -4246,14 +5959,223 @@
   license_family: MIT
   purls:
   - pkg:pypi/pytest-xdist?source=conda-forge-mapping
   size: 36516
   timestamp: 1700593072448
 - kind: conda
   name: python
+  version: 3.10.14
+  build: h00d2728_0_cpython
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.10.14-h00d2728_0_cpython.conda
+  sha256: 00c1de2d46ede26609ef4e84a44b83be7876ba6a0215b7c83bff41a0656bf694
+  md5: 0a1cddc4382c5c171e791c70740546dd
+  depends:
+  - bzip2 >=1.0.8,<2.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.10.* *_cp310
+  license: Python-2.0
+  size: 11890228
+  timestamp: 1710940046031
+- kind: conda
+  name: python
+  version: 3.10.14
+  build: h2469fbe_0_cpython
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.10.14-h2469fbe_0_cpython.conda
+  sha256: 454d609fe25daedce9e886efcbfcadad103ed0362e7cb6d2bcddec90b1ecd3ee
+  md5: 4ae999c8227c6d8c7623d32d51d25ea9
+  depends:
+  - bzip2 >=1.0.8,<2.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.10.* *_cp310
+  license: Python-2.0
+  size: 12336005
+  timestamp: 1710939659384
+- kind: conda
+  name: python
+  version: 3.10.14
+  build: h4de0772_0_cpython
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.10.14-h4de0772_0_cpython.conda
+  sha256: 332f97d9927b65857d6d2d4d50d66dce9b37da81edb67833ae6b88ad52acbd0c
+  md5: 4a00e84f29d1eb418d84970598c444e1
+  depends:
+  - bzip2 >=1.0.8,<2.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.2.1,<4.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - vc >=14.1,<15
+  - vc14_runtime >=14.16.27033
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.10.* *_cp310
+  license: Python-2.0
+  size: 15864027
+  timestamp: 1710938888352
+- kind: conda
+  name: python
+  version: 3.10.14
+  build: hd12c33a_0_cpython
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.10.14-hd12c33a_0_cpython.conda
+  sha256: 76a5d12e73542678b70a94570f7b0f7763f9a938f77f0e75d9ea615ef22aa84c
+  md5: 2b4ba962994e8bd4be9ff5b64b75aff2
+  depends:
+  - bzip2 >=1.0.8,<2.0a0
+  - ld_impl_linux-64 >=2.36.1
+  - libffi >=3.4,<4.0a0
+  - libgcc-ng >=12
+  - libnsl >=2.0.1,<2.1.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libuuid >=2.38.1,<3.0a0
+  - libxcrypt >=4.4.36
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.10.* *_cp310
+  license: Python-2.0
+  size: 25517742
+  timestamp: 1710939725109
+- kind: conda
+  name: python
+  version: 3.11.9
+  build: h631f459_0_cpython
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.11.9-h631f459_0_cpython.conda
+  sha256: 23698d4eb24970f74911d120204318d48384fabbb25e1e57773ad74fcd38fb12
+  md5: d7ed1e7c4e2dcdfd4599bd42c0613e6c
+  depends:
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.3,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.2.1,<4.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.11.* *_cp311
+  license: Python-2.0
+  size: 18232422
+  timestamp: 1713551717924
+- kind: conda
+  name: python
+  version: 3.11.9
+  build: h657bba9_0_cpython
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.11.9-h657bba9_0_cpython.conda
+  sha256: 3b50a5abb3b812875beaa9ab792dbd1bf44f335c64e9f9fedcf92d953995651c
+  md5: 612763bc5ede9552e4233ec518b9c9fb
+  depends:
+  - __osx >=10.9
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.3,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.11.* *_cp311
+  license: Python-2.0
+  size: 15503226
+  timestamp: 1713553747073
+- kind: conda
+  name: python
+  version: 3.11.9
+  build: h932a869_0_cpython
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.11.9-h932a869_0_cpython.conda
+  sha256: a436ceabde1f056a0ac3e347dadc780ee2a135a421ddb6e9a469370769829e3c
+  md5: 293e0713ae804b5527a673e7605c04fc
+  depends:
+  - __osx >=11.0
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.3,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.11.* *_cp311
+  license: Python-2.0
+  size: 14644189
+  timestamp: 1713552154779
+- kind: conda
+  name: python
+  version: 3.11.9
+  build: hb806964_0_cpython
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.11.9-hb806964_0_cpython.conda
+  sha256: 177f33a1fb8d3476b38f73c37b42f01c0b014fa0e039a701fd9f83d83aae6d40
+  md5: ac68acfa8b558ed406c75e98d3428d7b
+  depends:
+  - bzip2 >=1.0.8,<2.0a0
+  - ld_impl_linux-64 >=2.36.1
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libgcc-ng >=12
+  - libnsl >=2.0.1,<2.1.0a0
+  - libsqlite >=3.45.3,<4.0a0
+  - libuuid >=2.38.1,<3.0a0
+  - libxcrypt >=4.4.36
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.11.* *_cp311
+  license: Python-2.0
+  size: 30884494
+  timestamp: 1713553104915
+- kind: conda
+  name: python
   version: 3.12.3
   build: h1411813_0_cpython
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
   sha256: 3b327ffc152a245011011d1d730781577a8274fde1cf6243f073749ead8f1c2a
   md5: df1448ec6cbf8eceb03d29003cf72ae6
   depends:
@@ -4420,14 +6342,134 @@
   license_family: MIT
   purls:
   - pkg:pypi/python-semantic-release?source=conda-forge-mapping
   size: 61197
   timestamp: 1715814738178
 - kind: conda
   name: python_abi
+  version: '3.10'
+  build: 4_cp310
+  build_number: 4
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.10-4_cp310.conda
+  sha256: 456bec815bfc2b364763084d08b412fdc4c17eb9ccc66a36cb775fa7ac3cbaec
+  md5: 26322ec5d7712c3ded99dd656142b8ce
+  constrains:
+  - python 3.10.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6398
+  timestamp: 1695147363189
+- kind: conda
+  name: python_abi
+  version: '3.10'
+  build: 4_cp310
+  build_number: 4
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.10-4_cp310.conda
+  sha256: abc26b3b5a62f9c8112a2303d24b0c590d5f7fc9470521f5a520472d59c2223e
+  md5: b15c816c5a86abcc4d1458dd63aa4c65
+  constrains:
+  - python 3.10.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6484
+  timestamp: 1695147705581
+- kind: conda
+  name: python_abi
+  version: '3.10'
+  build: 4_cp310
+  build_number: 4
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.10-4_cp310.conda
+  sha256: f69bac2f28082a275ef67313968b2c366d8236c3a6869b9cdf5cdb97a5821812
+  md5: 1a3d9c6bb5f0b1b22d9e9296c127e8c7
+  constrains:
+  - python 3.10.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6490
+  timestamp: 1695147522999
+- kind: conda
+  name: python_abi
+  version: '3.10'
+  build: 4_cp310
+  build_number: 4
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.10-4_cp310.conda
+  sha256: 19066c462fd0e32c64503c688f77cb603beb4019b812caf855d03f2a5447960b
+  md5: b41195997c14fb7473d26637ea4c3946
+  constrains:
+  - python 3.10.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6773
+  timestamp: 1695147715814
+- kind: conda
+  name: python_abi
+  version: '3.11'
+  build: 4_cp311
+  build_number: 4
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-4_cp311.conda
+  sha256: 0be3ac1bf852d64f553220c7e6457e9c047dfb7412da9d22fbaa67e60858b3cf
+  md5: d786502c97404c94d7d58d258a445a65
+  constrains:
+  - python 3.11.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6385
+  timestamp: 1695147338551
+- kind: conda
+  name: python_abi
+  version: '3.11'
+  build: 4_cp311
+  build_number: 4
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-4_cp311.conda
+  sha256: f56dfe2a57b3b27bad3f9527f943548e8b2526e949d9d6fc0a383020d9359afe
+  md5: fef7a52f0eca6bae9e8e2e255bc86394
+  constrains:
+  - python 3.11.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6478
+  timestamp: 1695147518012
+- kind: conda
+  name: python_abi
+  version: '3.11'
+  build: 4_cp311
+  build_number: 4
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.11-4_cp311.conda
+  sha256: 4837089c477b9b84fa38a17f453e6634e68237267211b27a8a2f5ccd847f4e55
+  md5: 8d3751bc73d3bbb66f216fa2331d5649
+  constrains:
+  - python 3.11.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6492
+  timestamp: 1695147509940
+- kind: conda
+  name: python_abi
+  version: '3.11'
+  build: 4_cp311
+  build_number: 4
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-4_cp311.conda
+  sha256: 67c2aade3e2160642eec0742384e766b20c766055e3d99335681e3e05d88ed7b
+  md5: 70513332c71b56eace4ee6441e66c012
+  constrains:
+  - python 3.11.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6755
+  timestamp: 1695147711935
+- kind: conda
+  name: python_abi
   version: '3.12'
   build: 4_cp312
   build_number: 4
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
   sha256: 182a329de10a4165f6e8a3804caf751f918f6ea6176dd4e5abcdae1ed3095bf6
   md5: dccc2d142812964fcc6abdc97b672dff
@@ -4481,14 +6523,56 @@
   license: BSD-3-Clause
   license_family: BSD
   size: 6785
   timestamp: 1695147430513
 - kind: conda
   name: pywin32
   version: '306'
+  build: py310h00ffb61_2
+  build_number: 2
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py310h00ffb61_2.conda
+  sha256: 24fd15c118974da18c38870380195e633d2452a7fb7dbc0ecb96b44416989b33
+  md5: a65056c5f52aa83455577958872e4776
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: PSF-2.0
+  license_family: PSF
+  purls:
+  - pkg:pypi/pywin32?source=conda-forge-mapping
+  size: 5689476
+  timestamp: 1695974437046
+- kind: conda
+  name: pywin32
+  version: '306'
+  build: py311h12c1d0e_2
+  build_number: 2
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py311h12c1d0e_2.conda
+  sha256: 79d942817bdaf384602113e5fcb9158dc45cae4044bed308918a5db97f141fdb
+  md5: 25df0fc55722ea1a94494f41302e2d1c
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: PSF-2.0
+  license_family: PSF
+  purls:
+  - pkg:pypi/pywin32?source=conda-forge-mapping
+  size: 6124285
+  timestamp: 1695974706892
+- kind: conda
+  name: pywin32
+  version: '306'
   build: py312h53d5487_2
   build_number: 2
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
   sha256: d0ff1cd887b626a125f8323760736d8fab496bf2a400e825cce55361e7631264
   md5: f44c8f35c3f99eca30d6f5b68ddb0f42
   depends:
@@ -4619,14 +6703,186 @@
   purls:
   - pkg:pypi/pyyaml-env-tag?source=conda-forge-mapping
   size: 7473
   timestamp: 1624389117412
 - kind: conda
   name: pyzmq
   version: 26.0.3
+  build: py310h16e08c9_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.3-py310h16e08c9_0.conda
+  sha256: ab68d301d71f6520e42b3cc808a69b101c3b2697832f205b346de185761d847f
+  md5: 0788836c393aef2b46851f83416fd0d7
+  depends:
+  - __osx >=11.0
+  - libcxx >=16
+  - libsodium >=1.0.18,<1.0.19.0a0
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  - zeromq >=4.3.5,<4.4.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/pyzmq?source=conda-forge-mapping
+  size: 366478
+  timestamp: 1715024599862
+- kind: conda
+  name: pyzmq
+  version: 26.0.3
+  build: py310h656833d_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.3-py310h656833d_0.conda
+  sha256: 2e582fd6637243d751bd1cbc76ccb4b82aeecaa5c10dc6d493de67cbfde5b64c
+  md5: 8add222e6a146d96ac213db83d854f7d
+  depends:
+  - libsodium >=1.0.18,<1.0.19.0a0
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  - zeromq >=4.3.5,<4.3.6.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/pyzmq?source=conda-forge-mapping
+  size: 368528
+  timestamp: 1715025077475
+- kind: conda
+  name: pyzmq
+  version: 26.0.3
+  build: py310h6883aea_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.3-py310h6883aea_0.conda
+  sha256: 64a1b5362c070ccae0687651dee40987540e43d4a968a41b3de85f7fd8ef340d
+  md5: af2e86793164f8bd11e892142d0faa4c
+  depends:
+  - libgcc-ng >=12
+  - libsodium >=1.0.18,<1.0.19.0a0
+  - libstdcxx-ng >=12
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - zeromq >=4.3.5,<4.4.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/pyzmq?source=conda-forge-mapping
+  size: 388466
+  timestamp: 1715024604414
+- kind: conda
+  name: pyzmq
+  version: 26.0.3
+  build: py310he0bbd50_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.3-py310he0bbd50_0.conda
+  sha256: ddd28309169d61af6109c9d61392b4b035c1a2633a0bf1c58f1638c1a3870382
+  md5: b4481c0107ab67a37e8b7b218689d865
+  depends:
+  - __osx >=10.9
+  - libcxx >=16
+  - libsodium >=1.0.18,<1.0.19.0a0
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - zeromq >=4.3.5,<4.4.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/pyzmq?source=conda-forge-mapping
+  size: 366807
+  timestamp: 1715024677564
+- kind: conda
+  name: pyzmq
+  version: 26.0.3
+  build: py311h08a0b41_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.3-py311h08a0b41_0.conda
+  sha256: 1b488c4600682702e10c296d77f4497b1ef3fdf37847861e4e1269f2718b8842
+  md5: 8bef21c0a0160e7369fc2f494acf85d0
+  depends:
+  - libgcc-ng >=12
+  - libsodium >=1.0.18,<1.0.19.0a0
+  - libstdcxx-ng >=12
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - zeromq >=4.3.5,<4.4.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/pyzmq?source=conda-forge-mapping
+  size: 475189
+  timestamp: 1715024515323
+- kind: conda
+  name: pyzmq
+  version: 26.0.3
+  build: py311h484c95c_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.3-py311h484c95c_0.conda
+  sha256: 9c5c301d6bbb041d8728dfde015be7bc3ca5159b8193013581c5aa2de7bb9e89
+  md5: f32e37cabb3bc68396d2bc7939ac333c
+  depends:
+  - libsodium >=1.0.18,<1.0.19.0a0
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  - zeromq >=4.3.5,<4.3.6.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/pyzmq?source=conda-forge-mapping
+  size: 453691
+  timestamp: 1715025354726
+- kind: conda
+  name: pyzmq
+  version: 26.0.3
+  build: py311h89e2aaa_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.3-py311h89e2aaa_0.conda
+  sha256: 54e3e8a723ee2fff0e9317417684d5237453f935c0c971fb9808b9acb4fe15fa
+  md5: 91ec96c7ebdeb80c1d0d32777bfe76fa
+  depends:
+  - __osx >=10.9
+  - libcxx >=16
+  - libsodium >=1.0.18,<1.0.19.0a0
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - zeromq >=4.3.5,<4.4.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/pyzmq?source=conda-forge-mapping
+  size: 453164
+  timestamp: 1715024606404
+- kind: conda
+  name: pyzmq
+  version: 26.0.3
+  build: py311h9bed540_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.3-py311h9bed540_0.conda
+  sha256: 03b787e5d09ebd7c8e5a359d21ed264c4f0c473e7421be48d339fabddd43ffea
+  md5: 140d0704f24e0bad258d4e7ef567d797
+  depends:
+  - __osx >=11.0
+  - libcxx >=16
+  - libsodium >=1.0.18,<1.0.19.0a0
+  - python >=3.11,<3.12.0a0
+  - python >=3.11,<3.12.0a0 *_cpython
+  - python_abi 3.11.* *_cp311
+  - zeromq >=4.3.5,<4.4.0a0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/pyzmq?source=conda-forge-mapping
+  size: 451293
+  timestamp: 1715024663451
+- kind: conda
+  name: pyzmq
+  version: 26.0.3
   build: py312h8fd38d8_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.3-py312h8fd38d8_0.conda
   sha256: a3bf1e1af97a256a3a498cc7f2fedb478df18cf629cc9e9aa73a5b4cfc204d45
   md5: 27efa6d21e98bcab4585a6b913df7625
   depends:
   - libgcc-ng >=12
@@ -5188,14 +7444,160 @@
   purls:
   - pkg:pypi/tomlkit?source=conda-forge-mapping
   size: 37297
   timestamp: 1715185504185
 - kind: conda
   name: tornado
   version: '6.4'
+  build: py310h2372a71_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py310h2372a71_0.conda
+  sha256: bf3f211554444e03ed4663c0704fada38e0440fa723f1e32e12243ab026e3817
+  md5: 48f39c24349d9ae5c8e8873c42fb6170
+  depends:
+  - libgcc-ng >=12
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/tornado?source=conda-forge-mapping
+  size: 650910
+  timestamp: 1708363310348
+- kind: conda
+  name: tornado
+  version: '6.4'
+  build: py310h8d17308_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py310h8d17308_0.conda
+  sha256: ec383c3e3927634305d1e0b97d958c426f353156317f1c0210e6ce43c45eee80
+  md5: 0fcef3625a9081c94da6ca74af3fc293
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/tornado?source=conda-forge-mapping
+  size: 652769
+  timestamp: 1708363845639
+- kind: conda
+  name: tornado
+  version: '6.4'
+  build: py310hb372a2b_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py310hb372a2b_0.conda
+  sha256: ae6792e3cb7ebddef4884554c1566ed23d3891bb46b5357884154e93eb0dcc60
+  md5: 9665892738f34481a7450d6c16d4038a
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python_abi 3.10.* *_cp310
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/tornado?source=conda-forge-mapping
+  size: 651434
+  timestamp: 1708363551700
+- kind: conda
+  name: tornado
+  version: '6.4'
+  build: py310hd125d64_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py310hd125d64_0.conda
+  sha256: 8ee446ec68401a54540e3d848ffe7e4eb5633b7462c2a990efe0fb2621ebb50a
+  md5: 918e4a0c909366d09cf9530bdf3dc398
+  depends:
+  - python >=3.10,<3.11.0a0
+  - python >=3.10,<3.11.0a0 *_cpython
+  - python_abi 3.10.* *_cp310
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/tornado?source=conda-forge-mapping
+  size: 652190
+  timestamp: 1708363567796
+- kind: conda
+  name: tornado
+  version: '6.4'
+  build: py311h05b510d_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py311h05b510d_0.conda
+  sha256: 29c07a81b52310f9679ca05a6f1d3d3ee8c1830f183f91ad8d46f99cc2fb6720
+  md5: 241cd427ab1f38b72d6ddda3994c80a7
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python >=3.11,<3.12.0a0 *_cpython
+  - python_abi 3.11.* *_cp311
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/tornado?source=conda-forge-mapping
+  size: 856729
+  timestamp: 1708363632330
+- kind: conda
+  name: tornado
+  version: '6.4'
+  build: py311h459d7ec_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py311h459d7ec_0.conda
+  sha256: 5bb1e24d1767e403183e4cc842d184b2da497e778f0311c5b1d023fb3af9e6b6
+  md5: cc7727006191b8f3630936b339a76cd0
+  depends:
+  - libgcc-ng >=12
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/tornado?source=conda-forge-mapping
+  size: 853245
+  timestamp: 1708363316040
+- kind: conda
+  name: tornado
+  version: '6.4'
+  build: py311ha68e1ae_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py311ha68e1ae_0.conda
+  sha256: ce73a6cede35941e1d82098e37ab483e0f322503a87c48ea39e8ac05798f9e39
+  md5: 7bbff4fa9c26e56821e2eb89466436b1
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/tornado?source=conda-forge-mapping
+  size: 856957
+  timestamp: 1708363616871
+- kind: conda
+  name: tornado
+  version: '6.4'
+  build: py311he705e18_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py311he705e18_0.conda
+  sha256: 0b994ce7984953d1d528b7e19a97db0b34da09398feaf592500df637719d5623
+  md5: 40845aadca8df7ccc21c393ba3aa9eac
+  depends:
+  - python >=3.11,<3.12.0a0
+  - python_abi 3.11.* *_cp311
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/tornado?source=conda-forge-mapping
+  size: 857610
+  timestamp: 1708363541170
+- kind: conda
+  name: tornado
+  version: '6.4'
   build: py312h41838bb_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
   sha256: 558f50290a25d8da6071a8e951b2b0c2ef77f457254438fa7c19cb9ee9f5d952
   md5: 2d2d1fde5800d45cb56218583156d23d
   depends:
   - python >=3.12,<3.13.0a0
```

### Comparing `pydicomsorter-0.9.1/.github/workflows/main.yaml` & `pydicomsorter-0.9.2/.github/workflows/main.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 jobs:
   ################################################################################################
   # Unit-Tests: Run unit tests using pytest
   ################################################################################################
   Unit-Tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 15 # Consider increasing timeout
-    env:
-      PIXI_ENV: "dev"
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, macos-14, windows-latest]
+        env: ["py310", "py311", "py312"]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
-          environments: ${{ env.PIXI_ENV }}
+          environments: ${{ matrix.env }}
           pixi-version: v0.22.0
           cache: false
 
       - name: Run pytest
         run: |
-          pixi run test
+          pixi run -e ${{ matrix.env }} test
 
       - name: Upload coverage report artifact to be used by Codecov
         # only upload if matrix.os is ubuntu-latest and matrix.python-version is 3.12
         if: matrix.os == 'ubuntu-latest'
         uses: actions/upload-artifact@v2
         with:
           name: coverage-report
```

### Comparing `pydicomsorter-0.9.1/config/mkdocs.yaml` & `pydicomsorter-0.9.2/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/config/releaserc.toml` & `pydicomsorter-0.9.2/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/config/ruff.toml` & `pydicomsorter-0.9.2/config/ruff.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,14 @@
   "F",
   "W",   # flake8
   "C",   # mccabe
   "I",   # isort
   "N",   # pep8-naming
   "D",   # flake8-docstrings
   "ANN", # flake8-annotations
-  "S",   # flake8-bandit
   "BLE", # flake8-blind-except
   "B",   # flake8-bugbear
   "A",   # flake8-builtins
   "G",   # flake8-logging-format
   "ERA", # eradicate
   "RUF", # Ruff-specific rules
   "TCH", # flake8-type-checking
```

### Comparing `pydicomsorter-0.9.1/docs/CHANGELOG.md` & `pydicomsorter-0.9.2/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # CHANGELOG
 
 
 
+## v0.9.2 (2024-05-23)
+
+### Chore
+
+* chore: Update .gitignore and .github/workflows/main.yaml ([`431fe1a`](https://github.com/jjjermiah/PyDicomSorter/commit/431fe1ac2f4e7fab7d238625a82d4ef3c9a3a691))
+
+### Fix
+
+* fix: typo ([`b94f9f1`](https://github.com/jjjermiah/PyDicomSorter/commit/b94f9f1266ca840cb832640328de8f5e2d780896))
+
+* fix: force use the matrix env ([`1e63f36`](https://github.com/jjjermiah/PyDicomSorter/commit/1e63f36fd1fe2f65e8b7c78dea583156d6490cdc))
+
+
 ## v0.9.1 (2024-05-22)
 
 ### Fix
 
 * fix: version variable ([`23843a5`](https://github.com/jjjermiah/PyDicomSorter/commit/23843a5902fc7f88e1b69d3ada3ca4b2a2705c45))
```

### Comparing `pydicomsorter-0.9.1/docs/about.md` & `pydicomsorter-0.9.2/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/src/pydicomsorter/dicomsort.py` & `pydicomsorter-0.9.2/src/pydicomsorter/dicomsort.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,27 +15,29 @@
     """Dicomsort class."""
 
     def __init__(self, destination_dir: str) -> None:
         """Initialize the DICOMSorter."""
         self.format, self.keys = PatternParser().parse(destination_dir)
         self.console = Console()
 
-    def validate_keys(self) -> "DICOMSorter":
+    def validate_keys(self) -> 'DICOMSorter':
         """Validate the keys."""
         invalid_keys: list[str] = self.invalid_keys()
+        if not invalid_keys:
+            self.console.print('All keys are valid.')
+            return self
         for key in invalid_keys:
-            self.console.print(f"Invalid key:{key}")
+            self.console.print(f'Invalid key:{key}')
             closest_match = difflib.get_close_matches(key, all_dicom_tags, 3, 0.4)
             if closest_match:
-                self.console.print("Closest matches:")
+                self.console.print('Closest matches:')
                 [
-                    self.console.print(f"\t[bold cyan]{match}[/bold cyan]")
+                    self.console.print(f'\t[bold cyan]{match}[/bold cyan]')
                     for match in closest_match
                 ]
             else:
-                self.console.print("No close match found.")
-
-        return self
+                self.console.print('No close match found.')
+        raise ValueError('Invalid keys found.')
 
     def invalid_keys(self) -> list[str]:
         """Validate the keys."""
         return [key for key in self.keys if not tag_exists(keyword=key)]
```

### Comparing `pydicomsorter-0.9.1/src/pydicomsorter/options.py` & `pydicomsorter-0.9.2/src/pydicomsorter/options.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/src/pydicomsorter/parser.py` & `pydicomsorter-0.9.2/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.9.2/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/src/pydicomsorter/sandbox/dicomsort.py` & `pydicomsorter-0.9.2/src/pydicomsorter/sandbox/dicomsort.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.9.2/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/tests/test_parser.py` & `pydicomsorter-0.9.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/.gitignore` & `pydicomsorter-0.9.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -166,10 +166,11 @@
 .ruff_cache
 src/testmypixipkg/__pycache__/__init__.cpython-312.pyc
 **/__pycache__/*
 *./**/.pyc
 **.pyc
 
 data
+nbia-data
 
 
 **/.vscode/
```

### Comparing `pydicomsorter-0.9.1/LICENSE` & `pydicomsorter-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.1/README.md` & `pydicomsorter-0.9.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
 [![PyPI - Format](https://img.shields.io/pypi/format/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
 [![pixi-badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json&style=flat-square)](https://github.com/prefix-dev/pixi)
 
 Testing the pydicom library to sort dicom files by patient name and study date.
 
-Designing:
+> WARNING: This is a work in progress and is not implemented.
+
+Designing should look like:
 
 ``` bash
 Usage: dicomsort [OPTIONS] SOURCEDIR DESTINATION_DIR
 
 ╭─ Advanced options ───────────────────────────────────────────────────────────────╮
 │ --delete_source  -d    Delete the source files after sorting.                    │
 │ --keep_going     -k    Keep going when an error occurs.                          │
@@ -26,12 +28,24 @@
 ╭─ Basic options ──────────────────────────────────────────────────────────────────╮
 │ --verbose        Print verbose output.                                           │
 │ --debug          Print debug output.                                             │
 │ --help     -h    Show this message and exit.                                     │
 ╰──────────────────────────────────────────────────────────────────────────────────╯
 ```
 
+# DICOM data model
+
+A Patient has one or more Studies, a Study has one or more Series, and a Series has one or more Instances.
+
+```mermaid
+graph TD
+    A[Patient] --> B(Study)
+    B --> C(Series)
+    C --> D(Instance)
+
+```
+
 <!-- [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
 
 [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=jjjermiah)](https://github.com/jjjermiah/github-readme-stats) -->
 
 <!-- [![GitHub Trends SVG](https://api.githubtrends.io/user/svg/jjjermiah/langs)](https://githubtrends.io) -->
```

### Comparing `pydicomsorter-0.9.1/pyproject.toml` & `pydicomsorter-0.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.9.1"
+version = "0.9.2"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 
-requires-python = ">= 3.12"
+requires-python = ">= 3.10"
 dependencies = ["rich", "rich-click", "pydicom", "pydantic"]
 
 [project.urls]
 homepage = "https://github.com/jjjermiah/pydicomsorter"
 repository = "https://github.com/jjjermiah/pydicomsorter"
 documentation = "https://jjjermiah.github.io/pydicomsorter/"
 changelog = "https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md"
 issues = "https://github.com/jjjermiah/pydicomsorter/issues"
 
 [project.scripts]
 dicomsort = "pydicomsorter.cli:main"
 
-
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 #--------------------------------------------------------------------------------------------------#
 ############################################## PIXI ################################################
 #__________________________________________________________________________________________________#
@@ -39,16 +38,29 @@
 
 [tool.pixi.dependencies]
 
 [tool.pixi.pypi-dependencies]
 pydicomsorter = { path = ".", editable = true }
 
 [tool.pixi.environments]
+
 dev = { features = ["test", "style", "docs"], solve-group = "default" }
 publish = { features = ["build", "release"], solve-group = "default" }
+py310 = ["py310", "test"]
+py311 = ["py311", "test"]
+py312 = ["py312", "test"]
+
+############################################## python ###############################################
+
+[tool.pixi.feature.py310.dependencies]
+python = "3.10.*"
+[tool.pixi.feature.py311.dependencies]
+python = "3.11.*"
+[tool.pixi.feature.py312.dependencies]
+python = "3.12.*"
 
 ############################################## TEST ################################################
 [tool.pixi.feature.test.dependencies]
 pytest = "*"
 pytest-cov = "*"
 pytest-xdist = "*"
 ipykernel = ">=6.29.3,<6.30"
```

### Comparing `pydicomsorter-0.9.1/PKG-INFO` & `pydicomsorter-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
 Maintainer-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: package,pixi,pydicomsorter,python
-Requires-Python: >=3.12
+Requires-Python: >=3.10
 Requires-Dist: pydantic
 Requires-Dist: pydicom
 Requires-Dist: rich
 Requires-Dist: rich-click
 Description-Content-Type: text/markdown
 
 # pydicomsorter
@@ -29,15 +29,17 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
 [![PyPI - Format](https://img.shields.io/pypi/format/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
 [![pixi-badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json&style=flat-square)](https://github.com/prefix-dev/pixi)
 
 Testing the pydicom library to sort dicom files by patient name and study date.
 
-Designing:
+> WARNING: This is a work in progress and is not implemented.
+
+Designing should look like:
 
 ``` bash
 Usage: dicomsort [OPTIONS] SOURCEDIR DESTINATION_DIR
 
 ╭─ Advanced options ───────────────────────────────────────────────────────────────╮
 │ --delete_source  -d    Delete the source files after sorting.                    │
 │ --keep_going     -k    Keep going when an error occurs.                          │
@@ -47,12 +49,24 @@
 ╭─ Basic options ──────────────────────────────────────────────────────────────────╮
 │ --verbose        Print verbose output.                                           │
 │ --debug          Print debug output.                                             │
 │ --help     -h    Show this message and exit.                                     │
 ╰──────────────────────────────────────────────────────────────────────────────────╯
 ```
 
+# DICOM data model
+
+A Patient has one or more Studies, a Study has one or more Series, and a Series has one or more Instances.
+
+```mermaid
+graph TD
+    A[Patient] --> B(Study)
+    B --> C(Series)
+    C --> D(Instance)
+
+```
+
 <!-- [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
 
 [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=jjjermiah)](https://github.com/jjjermiah/github-readme-stats) -->
 
 <!-- [![GitHub Trends SVG](https://api.githubtrends.io/user/svg/jjjermiah/langs)](https://githubtrends.io) -->
```

