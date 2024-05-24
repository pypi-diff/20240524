# Comparing `tmp/compendium-0.1.3.post8.tar.gz` & `tmp/compendium-0.1.3.post9.tar.gz`

## Comparing `compendium-0.1.3.post8.tar` & `compendium-0.1.3.post9.tar`

### file list

```diff
@@ -1,123 +1,124 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/.flake8
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/mkdocs.yml
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/versioning.tar.gz
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/.github/workflows/docs.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/configuration.md
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/index.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/schema.md
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/settings.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/config_manager.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/filetypes.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/loader.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/paths.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/settings.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/filetypes/json.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/filetypes/toml.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/filetypes/xml.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/docs/development/filetypes/yaml.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config.toml
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested_env.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/settings.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/settings.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/check.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/config_file.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/example-out.yaml
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/example.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/in.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/in.toml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/in.yaml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/out.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/out.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_file/out.yaml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/config1.toml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/config2.toml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/config_manager.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/prototyping/config1.toml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/prototyping/config2.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/prototyping/example.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/prototyping/multiconfig.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/prototyping/prototype.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/prototyping/read_write.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/config_manager/prototyping/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/dataclass/hierarchial/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/dataclass/hierarchial/config.toml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/dataclass/hierarchial/config_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/dataclass/marshmallow/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/dataclass/pydantic/.keep
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/dataclass/simple/example-out.yaml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/dataclass/simple/example.yaml
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/dataclass/simple/example_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/hidden/.example
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/hidden/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/hidden/config.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/__init__.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman.py
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/proman-lock.json
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/pyproject.toml
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/module1/proman-lock.json
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/module1/pyproject.toml
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/module1/submodule1/proman-lock.json
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/module1/submodule1/pyproject.toml
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/module1/submodule2/proman-lock.json
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/module1/submodule2/pyproject.toml
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/module2/proman-lock.json
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/nested/proman/module2/pyproject.toml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/node.toml
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/tree.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/dry/node.toml
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/dry/dehiscent/node.toml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/dry/indehiscent/node.toml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/succulant/node.toml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/succulant/berry/node.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/succulant/berry/hesperidium/node.toml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/succulant/drupe/node.toml
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/examples/tree/succulant/pome/node.toml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/__init__.py
--rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/config_manager.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/exceptions.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/filepaths.py
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/py.typed
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/settings.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/filetypes/__init__.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/filetypes/ini.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/filetypes/json.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/filetypes/toml.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/filetypes/xml.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/src/compendium/filetypes/yaml.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tasks/__init__.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tasks/build.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tasks/doc.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tasks/qa.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/__init__.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/config.toml
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/test_config_manager.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/test_settings.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/test_version.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/test_filepaths.py.bak
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/hierarchy/settings1.toml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/hierarchy/settings2.toml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/hierarchy/settings3.toml
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/hierarchy/test_hierarchy.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/tree/fruit.toml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/tree/fruit1.toml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/tree/fruit2.toml
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/filepaths/tree/test_tree.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/ini/config.ini
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/ini/test_ini.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/json/config.json
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/json/test_json.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/module/config.toml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/toml/config.toml
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/toml/test_toml.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/xml/config.xml
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/xml/test_xml.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/yaml/config.yaml
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/tests/yaml/test_yaml.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/LICENSE
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/README.md
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/pyproject.toml
--rw-r--r--   0        0        0    19599 2020-02-02 00:00:00.000000 compendium-0.1.3.post8/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/.flake8
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/CODEOWNERS
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/mkdocs.yml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/versioning.tar.gz
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/configuration.md
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/index.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/schema.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/settings.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/config_manager.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/filetypes.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/loader.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/paths.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/settings.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/filetypes/json.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/filetypes/toml.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/filetypes/xml.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/docs/development/filetypes/yaml.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config.toml
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested_env.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/settings.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/settings.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/check.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/config_file.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/example-out.yaml
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/example.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/in.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/in.toml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/in.yaml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/out.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/out.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_file/out.yaml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/config1.toml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/config2.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/config_manager.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/prototyping/config1.toml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/prototyping/config2.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/prototyping/example.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/prototyping/multiconfig.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/prototyping/prototype.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/prototyping/read_write.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/config_manager/prototyping/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/dataclass/hierarchial/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/dataclass/hierarchial/config.toml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/dataclass/hierarchial/config_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/dataclass/marshmallow/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/dataclass/pydantic/.keep
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/dataclass/simple/example-out.yaml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/dataclass/simple/example.yaml
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/dataclass/simple/example_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/hidden/.example
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/hidden/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/hidden/config.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/__init__.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman.py
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/proman-lock.json
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/module1/proman-lock.json
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/module1/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/module1/submodule1/proman-lock.json
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/module1/submodule1/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/module1/submodule2/proman-lock.json
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/module1/submodule2/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/module2/proman-lock.json
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/nested/proman/module2/pyproject.toml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/node.toml
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/tree.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/dry/node.toml
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/dry/dehiscent/node.toml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/dry/indehiscent/node.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/succulant/node.toml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/succulant/berry/node.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/succulant/berry/hesperidium/node.toml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/succulant/drupe/node.toml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/examples/tree/succulant/pome/node.toml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/__init__.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/config_manager.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/exceptions.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/filepaths.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/py.typed
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/settings.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/filetypes/__init__.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/filetypes/ini.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/filetypes/json.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/filetypes/toml.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/filetypes/xml.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/src/compendium/filetypes/yaml.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tasks/__init__.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tasks/build.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tasks/doc.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tasks/qa.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/config.toml
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/test_config_manager.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/test_settings.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/test_version.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/test_filepaths.py.bak
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/hierarchy/settings1.toml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/hierarchy/settings2.toml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/hierarchy/settings3.toml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/hierarchy/test_hierarchy.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/tree/fruit.toml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/tree/fruit1.toml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/tree/fruit2.toml
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/filepaths/tree/test_tree.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/ini/config.ini
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/ini/test_ini.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/json/config.json
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/json/test_json.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/module/config.toml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/toml/config.toml
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/toml/test_toml.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/xml/config.xml
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/xml/test_xml.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/yaml/config.yaml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/tests/yaml/test_yaml.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/LICENSE
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/README.md
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/pyproject.toml
+-rw-r--r--   0        0        0    19599 2020-02-02 00:00:00.000000 compendium-0.1.3.post9/PKG-INFO
```

### Comparing `compendium-0.1.3.post8/mkdocs.yml` & `compendium-0.1.3.post9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/.github/workflows/ci.yml` & `compendium-0.1.3.post9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/.github/workflows/docs.yml` & `compendium-0.1.3.post9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/docs/configuration.md` & `compendium-0.1.3.post9/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/docs/settings.md` & `compendium-0.1.3.post9/docs/settings.md`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/config.toml` & `compendium-0.1.3.post9/examples/config.toml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/nested_env.py` & `compendium-0.1.3.post9/examples/nested_env.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/settings.md` & `compendium-0.1.3.post9/examples/settings.md`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/settings.py` & `compendium-0.1.3.post9/examples/settings.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/config_file/config_file.py` & `compendium-0.1.3.post9/examples/config_file/config_file.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/config_manager/config_manager.py` & `compendium-0.1.3.post9/examples/config_manager/config_manager.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/config_manager/prototyping/multiconfig.py` & `compendium-0.1.3.post9/examples/config_manager/prototyping/multiconfig.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/config_manager/prototyping/prototype.py` & `compendium-0.1.3.post9/examples/config_manager/prototyping/prototype.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/config_manager/prototyping/read_write.py` & `compendium-0.1.3.post9/examples/config_manager/prototyping/read_write.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/config_manager/prototyping/simple.py` & `compendium-0.1.3.post9/examples/config_manager/prototyping/simple.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/dataclass/hierarchial/config_file.py` & `compendium-0.1.3.post9/examples/dataclass/hierarchial/config_file.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/dataclass/simple/example_config.py` & `compendium-0.1.3.post9/examples/dataclass/simple/example_config.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/hidden/config.py` & `compendium-0.1.3.post9/examples/hidden/config.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/nested/proman.py` & `compendium-0.1.3.post9/examples/nested/proman.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/examples/tree/tree.py` & `compendium-0.1.3.post9/examples/tree/tree.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/__init__.py` & `compendium-0.1.3.post9/src/compendium/__init__.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/config_manager.py` & `compendium-0.1.3.post9/src/compendium/config_manager.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/exceptions.py` & `compendium-0.1.3.post9/src/compendium/exceptions.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/filepaths.py` & `compendium-0.1.3.post9/src/compendium/filepaths.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/loader.py` & `compendium-0.1.3.post9/src/compendium/loader.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/settings.py` & `compendium-0.1.3.post9/src/compendium/settings.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/filetypes/__init__.py` & `compendium-0.1.3.post9/src/compendium/filetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/filetypes/ini.py` & `compendium-0.1.3.post9/src/compendium/filetypes/ini.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/filetypes/json.py` & `compendium-0.1.3.post9/src/compendium/filetypes/json.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/filetypes/toml.py` & `compendium-0.1.3.post9/src/compendium/filetypes/toml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/filetypes/xml.py` & `compendium-0.1.3.post9/src/compendium/filetypes/xml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/src/compendium/filetypes/yaml.py` & `compendium-0.1.3.post9/src/compendium/filetypes/yaml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tasks/build.py` & `compendium-0.1.3.post9/tasks/build.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tasks/doc.py` & `compendium-0.1.3.post9/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tasks/qa.py` & `compendium-0.1.3.post9/tasks/qa.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/config.toml` & `compendium-0.1.3.post9/tests/config.toml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/test_config_manager.py` & `compendium-0.1.3.post9/tests/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/test_settings.py` & `compendium-0.1.3.post9/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/filepaths/test_filepaths.py.bak` & `compendium-0.1.3.post9/tests/filepaths/test_filepaths.py.bak`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/filepaths/hierarchy/test_hierarchy.py` & `compendium-0.1.3.post9/tests/filepaths/hierarchy/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/filepaths/tree/test_tree.py` & `compendium-0.1.3.post9/tests/filepaths/tree/test_tree.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/ini/test_ini.py` & `compendium-0.1.3.post9/tests/ini/test_ini.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/json/test_json.py` & `compendium-0.1.3.post9/tests/json/test_json.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/module/config.toml` & `compendium-0.1.3.post9/tests/module/config.toml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/toml/test_toml.py` & `compendium-0.1.3.post9/tests/toml/test_toml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/xml/test_xml.py` & `compendium-0.1.3.post9/tests/xml/test_xml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/tests/yaml/test_yaml.py` & `compendium-0.1.3.post9/tests/yaml/test_yaml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/.gitignore` & `compendium-0.1.3.post9/.gitignore`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/LICENSE` & `compendium-0.1.3.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/README.md` & `compendium-0.1.3.post9/README.md`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post8/pyproject.toml` & `compendium-0.1.3.post9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.11.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "compendium"
-version = "0.1.3.post8"
+version = "0.1.3.post9"
 description = "Simple layered configuraion tool"
 authors = [{name="Jesse P. Johnson", email="jpj6652@gmail.com"}]
 maintainers = [{name="Jesse P. Johnson", email="jpj6652@gmail.com"}]
 requires-python = ">=3.6.2"
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = ["configuration", "configuration management"]
```

### Comparing `compendium-0.1.3.post8/PKG-INFO` & `compendium-0.1.3.post9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: compendium
-Version: 0.1.3.post8
+Version: 0.1.3.post9
 Summary: Simple layered configuraion tool
 Project-URL: homepage, https://github.com/kuwv/python-compendium
 Project-URL: documentation, https://kuwv.github.io/python-compendium
 Author-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 Maintainer-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
```

