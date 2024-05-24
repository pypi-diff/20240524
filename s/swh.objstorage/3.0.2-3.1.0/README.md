# Comparing `tmp/swh_objstorage-3.0.2.tar.gz` & `tmp/swh_objstorage-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_objstorage-3.0.2.tar", last modified: Sun May  5 11:07:06 2024, max compression
+gzip compressed data, was "swh_objstorage-3.1.0.tar", last modified: Fri May 24 11:59:46 2024, max compression
```

## Comparing `swh_objstorage-3.0.2.tar` & `swh_objstorage-3.1.0.tar`

### file list

```diff
@@ -1,145 +1,141 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.239795 swh_objstorage-3.0.2/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-05-05 11:07:06.235795 swh_objstorage-3.0.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.203795 swh_objstorage-3.0.2/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/bin/swh-objstorage-azure
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.203795 swh_objstorage-3.0.2/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.203795 swh_objstorage-3.0.2/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.203795 swh_objstorage-3.0.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/docs/winery.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/requirements-libcloud.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/requirements-winery.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      297 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-05 11:07:06.239795 swh_objstorage-3.0.2/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.191795 swh_objstorage-3.0.2/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.207795 swh_objstorage-3.0.2/swh/objstorage/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.211795 swh_objstorage-3.0.2/swh/objstorage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1974 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5013 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/api/server.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.211795 swh_objstorage-3.0.2/swh/objstorage/backends/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17381 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5150 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1780 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8283 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/libcloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11964 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/pathslicing.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.211795 swh_objstorage-3.0.2/swh/objstorage/backends/seaweedfs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/seaweedfs/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/seaweedfs/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4925 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/seaweedfs/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.215795 swh_objstorage-3.0.2/swh/objstorage/backends/winery/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      191 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2076 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/database.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2857 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/gunicorn.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15419 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16100 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/roshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6856 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/rwshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17191 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/sharedbase.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/sleep.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.215795 swh_objstorage-3.0.2/swh/objstorage/backends/winery/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/sql/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6455 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/backends/winery/throttler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12642 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/constants.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1466 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2970 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/factory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8544 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/interface.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.219795 swh_objstorage-3.0.2/swh/objstorage/multiplexer/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      121 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/multiplexer/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.219795 swh_objstorage-3.0.2/swh/objstorage/multiplexer/filter/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2617 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/multiplexer/filter/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2721 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/multiplexer/filter/filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      785 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/multiplexer/filter/read_write_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11782 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/multiplexer/multiplexer_objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7416 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)      956 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.223795 swh_objstorage-3.0.2/swh/objstorage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13564 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/objstorage_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_api.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7083 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_cloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4694 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_instantiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3747 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_multiplexer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7192 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_pathslicing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_random_generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_seaweedfs.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45626 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_winery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_pathslicer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2952 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_readonly_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19921 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/winery_benchmark.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6882 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/tests/winery_testing_helpers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/swh/objstorage/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.231795 swh_objstorage-3.0.2/swh.objstorage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-05-05 11:07:06.000000 swh_objstorage-3.0.2/swh.objstorage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4236 2024-05-05 11:07:06.000000 swh_objstorage-3.0.2/swh.objstorage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-05 11:07:06.000000 swh_objstorage-3.0.2/swh.objstorage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-05 11:07:06.000000 swh_objstorage-3.0.2/swh.objstorage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      476 2024-05-05 11:07:06.000000 swh_objstorage-3.0.2/swh.objstorage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-05 11:07:06.000000 swh_objstorage-3.0.2/swh.objstorage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/tox.ini
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.231795 swh_objstorage-3.0.2/winery-test-environment/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/ansible.cfg
--rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/bootstrap.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/build-vms.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/ceph.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/fed4fire.rspec
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/fed4fire.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/grid5000.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.231795 swh_objstorage-3.0.2/winery-test-environment/inventory/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.195795 swh_objstorage-3.0.2/winery-test-environment/inventory/group_vars/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.231795 swh_objstorage-3.0.2/winery-test-environment/inventory/group_vars/all/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/inventory/group_vars/all/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/inventory/groups.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/inventory/hosts.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/inventory/osd.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/libvirt.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:06.231795 swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/README.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/mitogen.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/mitogen_free.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/mitogen_linear.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/osd.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/remote-tox.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/render-stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/rng.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-05 11:07:00.000000 swh_objstorage-3.0.2/winery-test-environment/tests.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.335599 swh_objstorage-3.1.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-24 11:59:46.335599 swh_objstorage-3.1.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.303599 swh_objstorage-3.1.0/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/bin/swh-objstorage-azure
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.307599 swh_objstorage-3.1.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.307599 swh_objstorage-3.1.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.307599 swh_objstorage-3.1.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/docs/winery.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-libcloud.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements-winery.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      308 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-24 11:59:46.335599 swh_objstorage-3.1.0/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.295599 swh_objstorage-3.1.0/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.311599 swh_objstorage-3.1.0/swh/objstorage/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.311599 swh_objstorage-3.1.0/swh/objstorage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2521 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5115 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/api/server.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.311599 swh_objstorage-3.1.0/swh/objstorage/backends/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17552 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5306 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3294 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1855 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8398 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/libcloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12102 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/pathslicing.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.315599 swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5043 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.315599 swh_objstorage-3.1.0/swh/objstorage/backends/winery/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      191 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2076 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/database.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2857 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/gunicorn.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15484 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16122 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/roshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6856 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/rwshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17191 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sharedbase.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sleep.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.315599 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/sql/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6455 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/backends/winery/throttler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12642 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/constants.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1971 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3472 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/factory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8960 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16465 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8303 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.319599 swh_objstorage-3.1.0/swh/objstorage/proxies/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/proxies/readonly.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1493 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.323599 swh_objstorage-3.1.0/swh/objstorage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15606 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/objstorage_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_api.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7640 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_cloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4729 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_instantiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13803 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7192 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_pathslicing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_random_generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_seaweedfs.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45626 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_winery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_pathslicer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3148 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_readonly_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19921 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/winery_benchmark.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6882 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/tests/winery_testing_helpers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/swh/objstorage/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.331599 swh_objstorage-3.1.0/swh.objstorage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4064 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      487 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-24 11:59:46.000000 swh_objstorage-3.1.0/swh.objstorage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.327599 swh_objstorage-3.1.0/winery-test-environment/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/ansible.cfg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/bootstrap.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/build-vms.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/ceph.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/fed4fire.rspec
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/fed4fire.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/grid5000.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.327599 swh_objstorage-3.1.0/winery-test-environment/inventory/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.299599 swh_objstorage-3.1.0/winery-test-environment/inventory/group_vars/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.327599 swh_objstorage-3.1.0/winery-test-environment/inventory/group_vars/all/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/inventory/group_vars/all/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/inventory/groups.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/inventory/hosts.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/inventory/osd.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/libvirt.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:46.327599 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/README.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_free.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_linear.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/osd.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/remote-tox.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/render-stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/rng.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-24 11:59:41.000000 swh_objstorage-3.1.0/winery-test-environment/tests.yml
```

### Comparing `swh_objstorage-3.0.2/.pre-commit-config.yaml` & `swh_objstorage-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/CODE_OF_CONDUCT.md` & `swh_objstorage-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/LICENSE` & `swh_objstorage-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/PKG-INFO` & `swh_objstorage-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 3.0.2
+Version: 3.1.0
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: click
+Requires-Dist: deprecated
 Requires-Dist: msgpack
 Requires-Dist: typing-extensions>=3.7.4
 Requires-Dist: requests
 Requires-Dist: swh.core[http]>=3.0.0
 Requires-Dist: swh.model>=0.0.27
 Requires-Dist: swh.perfecthash>=1.3.0
 Provides-Extra: azure
```

### Comparing `swh_objstorage-3.0.2/README.rst` & `swh_objstorage-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/bin/swh-objstorage-azure` & `swh_objstorage-3.1.0/bin/swh-objstorage-azure`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/conftest.py` & `swh_objstorage-3.1.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/docs/winery.rst` & `swh_objstorage-3.1.0/docs/winery.rst`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/mypy.ini` & `swh_objstorage-3.1.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/pyproject.toml` & `swh_objstorage-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/api/client.py` & `swh_objstorage-3.1.0/swh/objstorage/api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 import msgpack
 
 from swh.core.api import RPCClient
 from swh.objstorage.constants import DEFAULT_LIMIT
 from swh.objstorage.exc import (
     Error,
+    NoBackendsLeftError,
     ObjCorruptedError,
     ObjNotFoundError,
     ObjStorageAPIError,
 )
 from swh.objstorage.interface import CompositeObjId, ObjId, ObjStorageInterface
-from swh.objstorage.objstorage import objid_to_default_hex
+from swh.objstorage.objstorage import objid_to_default_hex, timed
 
 
 class RemoteObjStorage(RPCClient):
     """Proxy to a remote object storage.
 
     This class allows to connect to an object storage server via
     http protocol.
@@ -29,16 +30,22 @@
         url (string): The url of the server to connect. Must end
             with a '/'
         session: The session to send requests.
 
     """
 
     api_exception = ObjStorageAPIError
-    reraise_exceptions = [ObjNotFoundError, Error, ObjCorruptedError]
+    reraise_exceptions = [
+        ObjNotFoundError,
+        Error,
+        ObjCorruptedError,
+        NoBackendsLeftError,
+    ]
     backend_class = ObjStorageInterface
+    name: str = "remote"
 
     def restore(self: ObjStorageInterface, content: bytes, obj_id: ObjId) -> None:
         return self.add(content, obj_id, check_presence=False)
 
     def __iter__(self) -> Iterator[CompositeObjId]:
         yield from self.list_content()
 
@@ -56,7 +63,15 @@
             "get",
             "content",
             headers={"accept": "application/x-msgpack"},
             params=params,
             stream=True,
         )
         yield from msgpack.Unpacker(response.raw, raw=False)
+
+
+# XXX Maybe there is a better way of doing this, but according the automagic
+# way this class is built (via the MetaRPCClient metaclass), one cannot easily
+# just overload the methods in the class definition.
+RemoteObjStorage.get = timed(RemoteObjStorage.get)  # type: ignore
+RemoteObjStorage.add = timed(RemoteObjStorage.add)  # type: ignore
+RemoteObjStorage.__contains__ = timed(RemoteObjStorage.__contains__)  # type: ignore
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/api/server.py` & `swh_objstorage-3.1.0/swh/objstorage/api/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 import msgpack
 
 from swh.core.api import RPCServerApp
 from swh.core.api import encode_data_server as encode_data
 from swh.core.api import error_handler
 from swh.core.config import read as config_read
 from swh.core.statsd import statsd
-from swh.objstorage.exc import Error, ObjCorruptedError, ObjNotFoundError
+from swh.objstorage.exc import (
+    Error,
+    NoBackendsLeftError,
+    ObjCorruptedError,
+    ObjNotFoundError,
+)
 from swh.objstorage.factory import get_objstorage as get_swhobjstorage
 from swh.objstorage.interface import ObjStorageInterface
 
 
 def timed(f):
     @functools.wraps(f)
     def w(*a, **kw):
@@ -46,15 +51,20 @@
     if objstorage is None:
         objstorage = get_swhobjstorage(**app.config["objstorage"])
 
     return objstorage
 
 
 class ObjStorageServerApp(RPCServerApp):
-    client_exception_classes = (ObjNotFoundError, ObjCorruptedError, Error)
+    client_exception_classes = (
+        Error,
+        NoBackendsLeftError,
+        ObjCorruptedError,
+        ObjNotFoundError,
+    )
     method_decorators = [timed]
 
     def pre_add(self, kw):
         """Called before the 'add' method."""
         statsd.increment(
             "swh_objstorage_in_bytes_total",
             len(kw["content"]),
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/azure.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     generate_container_sas,
 )
 from azure.storage.blob.aio import ContainerClient as AsyncContainerClient
 
 from swh.model import hashutil
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
-from swh.objstorage.objstorage import CompressionFormat, ObjStorage
+from swh.objstorage.objstorage import CompressionFormat, ObjStorage, timed
 from swh.objstorage.utils import call_async
 
 
 def get_container_url(
     account_name: str,
     account_key: str,
     container_name: str,
@@ -102,17 +102,19 @@
       Signature". The :func:`get_container_url` helper can be used to generate
       such a URL from the account's access keys. The ``account_name``,
       ``api_secret_key`` and ``container_name`` arguments are deprecated.
 
     """
 
     PRIMARY_HASH = "sha1"
+    name: str = "azure"
 
     def __init__(
         self,
+        *,
         container_url: Optional[str] = None,
         account_name: Optional[str] = None,
         api_secret_key: Optional[str] = None,
         container_name: Optional[str] = None,
         connection_string: Optional[str] = None,
         compression: CompressionFormat = "gzip",
         use_secondary_endpoint_for_downloads=False,
@@ -208,14 +210,15 @@
 
             # FIXME: check_write is ignored here
             if not props:
                 return False
 
         return True
 
+    @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         """Does the storage contains the obj_id."""
         hex_obj_id = self._internal_id(obj_id)
         client = self.get_blob_client(hex_obj_id)
         try:
             client.get_blob_properties()
         except ResourceNotFoundError:
@@ -234,14 +237,15 @@
 
         Returns:
             number of objects contained in the storage.
 
         """
         return sum(1 for i in self)
 
+    @timed
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
         """Add an obj in storage if it's not there already."""
         if check_presence and obj_id in self:
             return
 
         hex_obj_id = self._internal_id(obj_id)
 
@@ -261,14 +265,15 @@
     def restore(self, content: bytes, obj_id: ObjId) -> None:
         """Restore a content."""
         if obj_id in self:
             self.delete(obj_id)
 
         return self.add(content, obj_id, check_presence=False)
 
+    @timed
     def get(self, obj_id: ObjId) -> bytes:
         """retrieve blob's content if found."""
         return call_async(self._get_async, obj_id)
 
     async def _get_async(self, obj_id, container_clients=None):
         """Coroutine implementing ``get(obj_id)`` using azure-storage-blob's
         asynchronous implementation.
@@ -361,19 +366,24 @@
     accounts is a dict containing entries of the form:
         <prefix>: <container_url_for_prefix>
     """
 
     def __init__(
         self,
         accounts: Mapping[str, Union[str, Mapping[str, str]]],
+        name: str = "azure-prefixed",
         compression: CompressionFormat = "gzip",
         **kwargs,
     ):
         # shortcut AzureCloudObjStorage __init__
-        ObjStorage.__init__(self, **kwargs)
+        ObjStorage.__init__(
+            self,
+            name=name,
+            **kwargs,
+        )
 
         self.compression = compression
 
         # Definition sanity check
         prefix_lengths = set(len(prefix) for prefix in accounts)
         if not len(prefix_lengths) == 1:
             raise ValueError(
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/generator.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from itertools import count, islice, repeat
 import logging
 import random
 from typing import Generator, Iterator, Optional, cast
 
 from swh.objstorage.constants import ID_HASH_ALGO
 from swh.objstorage.interface import CompositeObjId, ObjId
-from swh.objstorage.objstorage import DEFAULT_LIMIT, ObjStorage
+from swh.objstorage.objstorage import DEFAULT_LIMIT, ObjStorage, timed
+
+# we decorate methods with timed here to make tests pass without special care
 
 logger = logging.getLogger(__name__)
 
 
 class Randomizer:
     def __init__(self):
         self.size = 0
@@ -164,16 +166,18 @@
     for objsize in gen:
         yield randomizer.read(objsize)
 
 
 class RandomGeneratorObjStorage(ObjStorage):
     """A stupid read-only storage that generates blobs for testing purpose."""
 
+    name: str = "generator"
+
     def __init__(self, filesize=None, total=None, **kwargs):
-        super().__init__()
+        super().__init__(**kwargs)
         if filesize:
             filesize = int(filesize)
         self.filesize = filesize
         if total:
             total = int(total)
         self.total = total
         self._content_generator = None
@@ -183,14 +187,15 @@
         if self._content_generator is None:
             self._content_generator = gen_random_content(self.total, self.filesize)
         return self._content_generator
 
     def check_config(self, *, check_write):
         return True
 
+    @timed
     def __contains__(self, obj_id, *args, **kwargs):
         return False
 
     def __iter__(self) -> Iterator[CompositeObjId]:
         i = 1
         while True:
             j = yield {ID_HASH_ALGO: b"%d" % i}
@@ -198,17 +203,19 @@
                 logger.debug("DONE")
                 break
             if j is not None:
                 i = j
             else:
                 i += 1
 
+    @timed
     def get(self, obj_id, *args, **kwargs):
         return next(self.content_generator)
 
+    @timed
     def add(self, content, obj_id, check_presence=True, *args, **kwargs):
         pass
 
     def check(self, obj_id, *args, **kwargs):
         return True
 
     def delete(self, obj_id, *args, **kwargs):
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/http.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/http.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 from urllib.parse import urljoin
 
 import requests
 
 from swh.model import hashutil
 from swh.objstorage.constants import ID_HASH_ALGO
 from swh.objstorage.exc import (
-    NonIterableObjStorage,
+    NonIterableObjStorageError,
     ObjNotFoundError,
-    ReadOnlyObjStorage,
+    ReadOnlyObjStorageError,
 )
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
     DEFAULT_LIMIT,
     CompressionFormat,
     ObjStorage,
     objid_to_default_hex,
+    timed,
 )
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.ERROR)
 
 
 class HTTPReadOnlyObjStorage(ObjStorage):
@@ -35,52 +36,57 @@
     For example, can be used to retrieve objects from S3:
 
     objstorage:
       cls: http
       url: https://softwareheritage.s3.amazonaws.com/content/
     """
 
+    name: str = "http"
+
     def __init__(self, url=None, compression: CompressionFormat = "none", **kwargs):
         super().__init__(**kwargs)
         self.session = requests.sessions.Session()
         self.root_path = url
         if not self.root_path.endswith("/"):
             self.root_path += "/"
         self.compression = compression
 
     def check_config(self, *, check_write):
         """Check the configuration for this object storage"""
-        return True
+        return check_write is False
 
+    @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         resp = self.session.head(self._path(obj_id))
         return resp.status_code == 200
 
     def __iter__(self) -> Iterator[CompositeObjId]:
-        raise NonIterableObjStorage("__iter__")
+        raise NonIterableObjStorageError("__iter__")
 
     def __len__(self):
-        raise NonIterableObjStorage("__len__")
+        raise NonIterableObjStorageError("__len__")
 
+    @timed
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
-        raise ReadOnlyObjStorage("add")
+        raise ReadOnlyObjStorageError("add")
 
     def delete(self, obj_id: ObjId):
-        raise ReadOnlyObjStorage("delete")
+        raise ReadOnlyObjStorageError("delete")
 
     def restore(self, content: bytes, obj_id: ObjId) -> None:
-        raise ReadOnlyObjStorage("restore")
+        raise ReadOnlyObjStorageError("restore")
 
     def list_content(
         self,
         last_obj_id: Optional[ObjId] = None,
         limit: Optional[int] = DEFAULT_LIMIT,
     ) -> Iterator[CompositeObjId]:
-        raise NonIterableObjStorage("__len__")
+        raise NonIterableObjStorageError("__len__")
 
+    @timed
     def get(self, obj_id: ObjId) -> bytes:
         try:
             resp = self.session.get(self._path(obj_id))
             resp.raise_for_status()
         except Exception:
             raise ObjNotFoundError(obj_id)
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/in_memory.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/in_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,52 +3,56 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from typing import Dict, Iterator
 
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
-from swh.objstorage.objstorage import ObjStorage
+from swh.objstorage.objstorage import ObjStorage, timed
 
 
 class InMemoryObjStorage(ObjStorage):
     """In-Memory objstorage.
 
     Intended for test purposes.
 
     """
 
     PRIMARY_HASH = "sha1"
+    name: str = "memory"
 
-    def __init__(self, **args):
-        super().__init__()
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         self.state: Dict[bytes, bytes] = {}
 
     def check_config(self, *, check_write):
         return True
 
     def _state_key(self, obj_id: ObjId) -> bytes:
         if isinstance(obj_id, dict):
             return obj_id[self.PRIMARY_HASH]
         else:
             return obj_id
 
+    @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         return self._state_key(obj_id) in self.state
 
     def __iter__(self) -> Iterator[CompositeObjId]:
         for id_ in sorted(self.state):
             yield {self.PRIMARY_HASH: id_}
 
+    @timed
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
         if check_presence and obj_id in self:
             return
 
         self.state[self._state_key(obj_id)] = content
 
+    @timed
     def get(self, obj_id: ObjId) -> bytes:
         if obj_id not in self:
             raise ObjNotFoundError(obj_id)
 
         return self.state[self._state_key(obj_id)]
 
     def delete(self, obj_id: ObjId):
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/libcloud.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/libcloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from swh.model import hashutil
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
     CompressionFormat,
     ObjStorage,
     objid_to_default_hex,
+    timed,
 )
 
 
 def patch_libcloud_s3_urlencode():
     """Patches libcloud's S3 backend to properly sign queries.
 
     Recent versions of libcloud are not affected (they use signature V4),
@@ -56,14 +57,15 @@
       path_prefix: prefix to prepend to object paths in the container,
                    separated with a slash
       compression: compression algorithm to use for objects
       kwargs: extra arguments are passed through to the LibCloud driver
     """
 
     PRIMARY_HASH = "sha1"
+    name: str = "cloud"
 
     def __init__(
         self,
         container_name: str,
         compression: CompressionFormat = "gzip",
         path_prefix: Optional[str] = None,
         **kwargs,
@@ -114,14 +116,15 @@
         )
 
     def check_config(self, *, check_write):
         """Check the configuration for this object storage"""
         # FIXME: hopefully this blew up during instantiation
         return True
 
+    @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         try:
             self._get_object(obj_id)
         except ObjNotFoundError:
             return False
         else:
             return True
@@ -155,23 +158,25 @@
 
         Returns:
             number of objects contained in the storage.
 
         """
         return sum(1 for i in self)
 
+    @timed
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
         if check_presence and obj_id in self:
             return
 
         self._put_object(content, obj_id)
 
     def restore(self, content: bytes, obj_id: ObjId) -> None:
         return self.add(content, obj_id, check_presence=False)
 
+    @timed
     def get(self, obj_id: ObjId) -> bytes:
         obj = b"".join(self._get_object(obj_id).as_stream())
         return self.decompress(obj, objid_to_default_hex(obj_id))
 
     def download_url(
         self,
         obj_id: ObjId,
@@ -224,14 +229,16 @@
             object_path,
         )
 
 
 class AwsCloudObjStorage(CloudObjStorage):
     """Amazon's S3 Cloud-based object storage"""
 
+    name: str = "s3"
+
     def _get_provider(self):
         return Provider.S3
 
     def download_url(
         self,
         obj_id: ObjId,
         content_disposition: Optional[str] = None,
@@ -242,9 +249,11 @@
             ex_expiry=(expiry.total_seconds() / 3600) if expiry is not None else 24,
         )
 
 
 class OpenStackCloudObjStorage(CloudObjStorage):
     """OpenStack Swift Cloud based object storage"""
 
+    name: str = "swift"
+
     def _get_provider(self):
         return Provider.OPENSTACK_SWIFT
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/noop.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/noop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # Copyright (C) 2021  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from swh.objstorage.objstorage import ObjStorage
+from swh.objstorage.objstorage import ObjStorage, timed
+
+# we decorate methods with timed here to make tests pass without special care
 
 
 class NoopObjStorage(ObjStorage):
     """Noop objstorage. Basic implementation which does no operations at all.
 
     Only intended for test purposes to avoid either memory or i/o operations. This
     allows swh clients to use the swh stack without having to deal with objstorage
     configuration. So users can concentrate on testing the remaining part of the stack
     without the objstorage.
 
     """
 
+    name: str = "noop"
+
     def check_config(self, *, check_write):
         return True
 
+    @timed
     def __contains__(self, obj_id, *args, **kwargs):
         return False
 
+    @timed
     def add(self, content, obj_id, check_presence=True, *args, **kwargs):
         pass
 
+    @timed
     def get(self, obj_id, *args, **kwargs):
         return None
 
     def check(self, obj_id, *args, **kwargs):
         pass
 
     def delete(self, obj_id, *args, **kwargs):
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/pathslicing.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/pathslicing.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
     CompressionFormat,
     ObjStorage,
     compressors,
     objid_to_default_hex,
+    timed,
 )
 
 BUFSIZ = 1048576
 
 DIR_MODE = 0o755
 FILE_MODE = 0o644
 
@@ -163,17 +164,23 @@
         slicing (str): string that indicates the slicing to perform
             on the hash of the content to know the path where it should
             be stored (see the documentation of the PathSlicer class).
 
     """
 
     PRIMARY_HASH: Literal["sha1"] = "sha1"
+    name: str = "pathslicing"
 
     def __init__(
-        self, root, slicing, compression: CompressionFormat = "gzip", **kwargs
+        self,
+        *,
+        root: str = "",
+        compression: CompressionFormat = "gzip",
+        slicing: str = "",
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.root = root
         self.slicer = PathSlicer(root, slicing)
 
         self.use_fdatasync = hasattr(os, "fdatasync")
         self.compression = compression
@@ -200,14 +207,15 @@
             raise ValueError(
                 'Unknown compression algorithm "%s" for '
                 "PathSlicingObjStorage" % self.compression
             )
 
         return True
 
+    @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         hex_obj_id = objid_to_default_hex(obj_id)
         return os.path.isfile(self.slicer.get_path(hex_obj_id))
 
     def __iter__(self) -> Iterator[CompositeObjId]:
         """Iterate over the object identifiers currently available in the
         storage.
@@ -240,28 +248,30 @@
         performances applies
 
         Return:
             number of objects contained in the storage
         """
         return sum(1 for i in self)
 
+    @timed
     def add(
         self,
         content: bytes,
         obj_id: ObjId,
         check_presence: bool = True,
     ) -> None:
         if check_presence and obj_id in self:
             # If the object is already present, return immediately.
             return
 
         hex_obj_id = objid_to_default_hex(obj_id)
         with self._write_obj_file(hex_obj_id) as f:
             f.write(self.compress(content))
 
+    @timed
     def get(self, obj_id: ObjId) -> bytes:
         if obj_id not in self:
             raise ObjNotFoundError(obj_id)
 
         # Open the file and return its content as bytes
         hex_obj_id = objid_to_default_hex(obj_id)
         with open(self.slicer.get_path(hex_obj_id), "rb") as f:
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/seaweedfs/http.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/seaweedfs/objstorage.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/seaweedfs/objstorage.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,50 +15,54 @@
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
     DEFAULT_LIMIT,
     CompressionFormat,
     ObjStorage,
     objid_to_default_hex,
+    timed,
 )
 
 from .http import HttpFiler
 
 LOGGER = logging.getLogger(__name__)
 
 
 class SeaweedFilerObjStorage(ObjStorage):
     """ObjStorage with seaweedfs abilities, using the Filer API.
 
     https://github.com/chrislusf/seaweedfs/wiki/Filer-Server-API
     """
 
     PRIMARY_HASH = "sha1"
+    name: str = "seaweedfs"
 
     def __init__(
         self,
-        url,
+        *,
+        url: str = "",
         compression: CompressionFormat = "none",
-        slicing="",
-        pool_maxsize=100,
+        slicing: str = "",
+        pool_maxsize: int = 100,
         **kwargs,
     ):
         super().__init__(**kwargs)
+        self.compression = compression
         self.wf = HttpFiler(url, pool_maxsize=pool_maxsize)
         self.root_path = urlparse(url).path
         if not self.root_path.endswith("/"):
             self.root_path += "/"
         self.slicer = PathSlicer(self.root_path, slicing)
-        self.compression = compression
 
     def check_config(self, *, check_write):
         """Check the configuration for this object storage"""
         # FIXME: hopefully this blew up during instantiation
         return True
 
+    @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         return self.wf.exists(self._path(obj_id))
 
     def __iter__(self) -> Iterator[CompositeObjId]:
         """Iterate over the objects present in the storage
 
         Warning: Iteration over the contents of a cloud-based object storage
@@ -80,23 +84,26 @@
 
         Returns:
             number of objects contained in the storage.
 
         """
         return sum(1 for i in self)
 
+    @timed
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
         if check_presence and obj_id in self:
             return
 
         self.wf.put(io.BytesIO(self.compress(content)), self._path(obj_id))
 
+    @timed
     def restore(self, content: bytes, obj_id: ObjId) -> None:
         return self.add(content, obj_id, check_presence=False)
 
+    @timed
     def get(self, obj_id: ObjId) -> bytes:
         try:
             obj = self.wf.get(self._path(obj_id))
         except Exception as exc:
             LOGGER.info("Failed to get object %s: %r", self._path(obj_id), exc)
             raise ObjNotFoundError(obj_id)
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/database.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/database.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/gunicorn.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/gunicorn.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/objstorage.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/objstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import partial
 import logging
 from multiprocessing import Process
 from typing import Callable, List, Optional, Tuple
 
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import ObjId
-from swh.objstorage.objstorage import ObjStorage
+from swh.objstorage.objstorage import ObjStorage, timed
 
 from .roshard import (
     DEFAULT_IMAGE_FEATURES_UNSUPPORTED,
     Pool,
     ROShard,
     ROShardCreator,
     ShardNotMapped,
@@ -25,31 +25,35 @@
 from .stats import Stats
 
 logger = logging.getLogger(__name__)
 
 
 class WineryObjStorage(ObjStorage):
     PRIMARY_HASH = "sha256"
+    name: str = "winery"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         if kwargs.get("readonly"):
             self.winery = WineryReader(**kwargs)
         else:
             self.winery = WineryWriter(**kwargs)
 
+    @timed
     def get(self, obj_id: ObjId) -> bytes:
         return self.winery.get(self._hash(obj_id))
 
     def check_config(self, *, check_write: bool) -> bool:
         return True
 
+    @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         return self._hash(obj_id) in self.winery
 
+    @timed
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
         self.winery.add(content, self._hash(obj_id), check_presence)
 
     def delete(self, obj_id: ObjId):
         if not self.allow_delete:
             raise PermissionError("Delete is not allowed.")
         return self.winery.delete(obj_id)
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/roshard.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/roshard.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,16 +328,16 @@
     def get(self, key):
         if not self.shard:
             self.open()
 
         return self.throttler.throttle_get(self.shard.lookup, key)
 
     def close(self):
-        if self.shard:
-            self.shard.close()
+        if shard := getattr(self, "shard", None):
+            shard.close()
         self.shard = None
 
     def __del__(self):
         self.close()
 
     @staticmethod
     def delete(pool, shard_name, obj_id):
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/rwshard.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/rwshard.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/sharedbase.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/sharedbase.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/sleep.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/sleep.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/sql/30-schema.sql` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/stats.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/stats.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/backends/winery/throttler.py` & `swh_objstorage-3.1.0/swh/objstorage/backends/winery/throttler.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/cli.py` & `swh_objstorage-3.1.0/swh/objstorage/cli.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/constants.py` & `swh_objstorage-3.1.0/swh/objstorage/constants.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/factory.py` & `swh_objstorage-3.1.0/swh/objstorage/factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-# Copyright (C) 2016-2022  The Software Heritage developers
+# Copyright (C) 2016-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import importlib
+import warnings
 
 from swh.objstorage.interface import ObjStorageInterface
-from swh.objstorage.multiplexer import MultiplexerObjStorage
-from swh.objstorage.multiplexer.filter import add_filters
 from swh.objstorage.objstorage import ObjStorage
 
 __all__ = ["get_objstorage", "ObjStorage"]
 
 
 OBJSTORAGE_IMPLEMENTATIONS = {
-    "pathslicing": ".backends.pathslicing.PathSlicingObjStorage",
-    "remote": ".api.client.RemoteObjStorage",
-    "memory": ".backends.in_memory.InMemoryObjStorage",
-    "seaweedfs": ".backends.seaweedfs.SeaweedFilerObjStorage",
-    "random": ".backends.generator.RandomGeneratorObjStorage",
-    "http": ".backends.http.HTTPReadOnlyObjStorage",
-    "noop": ".backends.noop.NoopObjStorage",
-    "azure": ".backends.azure.AzureCloudObjStorage",
-    "azure-prefixed": ".backends.azure.PrefixedAzureCloudObjStorage",
-    "s3": ".backends.libcloud.AwsCloudObjStorage",
-    "swift": ".backends.libcloud.OpenStackCloudObjStorage",
-    "winery": ".backends.winery.WineryObjStorage",
+    "pathslicing": "swh.objstorage.backends.pathslicing.PathSlicingObjStorage",
+    "remote": "swh.objstorage.api.client.RemoteObjStorage",
+    "memory": "swh.objstorage.backends.in_memory.InMemoryObjStorage",
+    "seaweedfs": "swh.objstorage.backends.seaweedfs.objstorage.SeaweedFilerObjStorage",
+    "random": "swh.objstorage.backends.generator.RandomGeneratorObjStorage",
+    "http": "swh.objstorage.backends.http.HTTPReadOnlyObjStorage",
+    "noop": "swh.objstorage.backends.noop.NoopObjStorage",
+    "azure": "swh.objstorage.backends.azure.AzureCloudObjStorage",
+    "azure-prefixed": "swh.objstorage.backends.azure.PrefixedAzureCloudObjStorage",
+    "s3": "swh.objstorage.backends.libcloud.AwsCloudObjStorage",
+    "swift": "swh.objstorage.backends.libcloud.OpenStackCloudObjStorage",
+    "winery": "swh.objstorage.backends.winery.WineryObjStorage",
+    # filters and proxies
+    "multiplexer": "swh.objstorage.multiplexer.MultiplexerObjStorage",
+    "read-only": "swh.objstorage.proxies.readonly.ReadOnlyProxyObjStorage",
+    # deprecated factories
+    "filtered": "_construct_filtered_objstorage",
 }
 
 
 def get_objstorage(cls: str, **kwargs) -> ObjStorageInterface:
     """Create an ObjStorage using the given implementation class.
 
     Args:
         cls: objstorage class unique key contained in the
-            _STORAGE_CLASSES dict.
+            OBJSTORAGE_IMPLEMENTATIONS dict.
         kwargs: arguments for the required class of objstorage
                 that must match exactly the one in the `__init__` method of the
                 class.
     Returns:
         subclass of ObjStorage that match the given `storage_class` argument.
     Raises:
         ValueError: if the given storage class is not a valid objstorage
@@ -55,25 +59,23 @@
         (module_path, class_name) = class_path.rsplit(".", 1)
         try:
             module = importlib.import_module(module_path, package=__package__)
         except ImportError as e:
             raise ValueError(f"Storage class {cls} is not available: {e.args[0]}")
         ObjStorage = getattr(module, class_name)
     else:
+        # used by (deprecated) filtered for which the value is a factory
+        # function rather than a class
         ObjStorage = globals()[class_path]
-
     return ObjStorage(**kwargs)
 
 
-def _construct_filtered_objstorage(storage_conf, filters_conf):
-    return add_filters(get_objstorage(**storage_conf), filters_conf)
-
-
-OBJSTORAGE_IMPLEMENTATIONS["filtered"] = "_construct_filtered_objstorage"
-
-
-def _construct_multiplexer_objstorage(objstorages):
-    storages = [get_objstorage(**conf) for conf in objstorages]
-    return MultiplexerObjStorage(storages)
-
+def _construct_filtered_objstorage(storage_conf, filters_conf, **kwargs):
+    if len(filters_conf) != 1 or filters_conf[0]["type"] != "readonly":
+        raise ValueError("This legacy function only supports a single readonly filter")
+    warnings.warn(
+        "The 'filtered[type:readonly]' objstorage class has been deprecated, "
+        "please use a 'read-only' proxy class instead.",
+        DeprecationWarning,
+    )
 
-OBJSTORAGE_IMPLEMENTATIONS["multiplexer"] = "_construct_multiplexer_objstorage"
+    return get_objstorage(cls="read-only", storage=get_objstorage(**storage_conf))
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/interface.py` & `swh_objstorage-3.1.0/swh/objstorage/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2015-2023 The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 
 from datetime import timedelta
 from typing import (
@@ -71,28 +71,46 @@
     - __contains__()  check if an object is present, by object id
     - add()           add a new object, returning an object id
     - restore()       same as add() but erase an already existed content
     - get()           retrieve the content of an object, by object id
     - check()         check the integrity of an object, by object id
     - delete()        remove an object
 
+    and the following attributes:
+
+    - name            name given to the object storage; useful e.g. for logging in
+                      composite object storagges (multiplexer)
+
     Each implementation of this interface can have a different behavior and
     its own way to store the contents.
     """
 
+    name: str
+
+    def __init__(
+        self,
+        *,
+        name: str = "",
+        **kwargs,
+    ):
+        ...
+
     @remote_api_endpoint("check_config")
     def check_config(self, *, check_write):
         """Check whether the object storage is properly configured.
 
         Args:
             check_write (bool): if True, check if writes to the object storage
             can succeed.
 
         Returns:
-            True if the configuration check worked, an exception if it didn't.
+            True if the configuration check worked, False if 'check_write' is
+            True and the object storage is actually read only, and an exception
+            if the check failed.
+
         """
         ...
 
     @remote_api_endpoint("content/contains")
     def __contains__(self, obj_id: ObjId) -> bool:
         """Indicate if the given object is present in the storage.
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/multiplexer/filter/filter.py` & `swh_objstorage-3.1.0/swh/objstorage/proxies/readonly.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,33 @@
-# Copyright (C) 2015-2016  The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from typing import Iterator
+from typing import Dict, Iterator, Union
 
-from swh.objstorage.interface import CompositeObjId
+from swh.objstorage.exc import ReadOnlyObjStorageError
+from swh.objstorage.factory import get_objstorage
+from swh.objstorage.interface import CompositeObjId, ObjStorageInterface
 from swh.objstorage.objstorage import ObjStorage
 
 
-class ObjStorageFilter(ObjStorage):
-    """Base implementation of a filter that allow inputs on ObjStorage or
-    not.
-
-    This class copy the API of ...objstorage in order to filter the
-    inputs of this class.
-
-    If the operation is allowed, return the result of this operation
-    applied to the destination implementation. Otherwise, just return
-    without any operation.
-
-    This class is an abstract base class for a classic read/write
-    storage.  Filters can inherit from it and only redefine some
-    methods in order to change behavior.
+class ReadOnlyProxyObjStorage(ObjStorage):
+    """Filter that disable write operation of the storage.
 
+    Writes will always succeed without doing any actual write operations.
     """
 
-    def __init__(self, storage):
-        self.storage = storage
+    name: str = "read-only"
 
-    def check_config(self, *, check_write):
-        """Check the object storage for proper configuration.
-
-        Args:
-            check_write: check whether writes to the objstorage will succeed
-        Returns:
-            True if the storage is properly configured
-        """
-        return self.storage.check_config(check_write=check_write)
+    def __init__(self, storage: Union[ObjStorageInterface, Dict], **kwargs):
+        super().__init__(**kwargs)
+        self.storage: ObjStorageInterface = (
+            get_objstorage(**storage) if isinstance(storage, dict) else storage
+        )
 
     def __contains__(self, *args, **kwargs):
         return self.storage.__contains__(*args, **kwargs)
 
     def __iter__(self) -> Iterator[CompositeObjId]:
         """Iterates over the content of each storages
 
@@ -57,21 +43,26 @@
         Warning: performance issue in `__iter__` also applies here.
 
         Returns:
             number of objects contained in the storage.
         """
         return self.storage.__len__()
 
-    def add(self, content, obj_id, check_presence=True, *args, **kwargs):
-        return self.storage.add(content, obj_id, check_presence, *args, **kwargs)
-
-    def restore(self, content, obj_id, *args, **kwargs):
-        return self.storage.restore(content, obj_id, *args, **kwargs)
-
     def get(self, obj_id, *args, **kwargs):
         return self.storage.get(obj_id, *args, **kwargs)
 
     def check(self, obj_id, *args, **kwargs):
         return self.storage.check(obj_id, *args, **kwargs)
 
-    def delete(self, obj_id, *args, **kwargs):
-        return self.storage.delete(obj_id, *args, **kwargs)
+    def check_config(self, *, check_write):
+        if check_write:
+            return False
+        return self.storage.check_config(check_write=False)
+
+    def add(self, *args, **kwargs):
+        raise ReadOnlyObjStorageError("add")
+
+    def restore(self, *args, **kwargs):
+        raise ReadOnlyObjStorageError("restore")
+
+    def delete(self, *args, **kwargs):
+        raise ReadOnlyObjStorageError("dalete")
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/multiplexer/multiplexer_objstorage.py` & `swh_objstorage-3.1.0/swh/objstorage/multiplexer.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,24 +2,46 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import logging
 import queue
 import threading
-from typing import Dict, Iterable, Iterator, Mapping, Optional, Tuple, Union
+from typing import Dict, Iterable, Iterator, List, Mapping, Optional, Set, Tuple, Union
 
+# note: it's required to access the statsd object form the statsd module to
+# help mocking it in tests...
+from swh.core import statsd
 from swh.model.model import Sha1
-from swh.objstorage.exc import ObjCorruptedError, ObjNotFoundError
-from swh.objstorage.interface import CompositeObjId, ObjId
-from swh.objstorage.objstorage import ObjStorage
+from swh.objstorage.exc import (
+    NoBackendsLeftError,
+    ObjCorruptedError,
+    ObjNotFoundError,
+    ObjStorageAPIError,
+)
+from swh.objstorage.factory import get_objstorage
+from swh.objstorage.interface import CompositeObjId, ObjId, ObjStorageInterface
+from swh.objstorage.objstorage import ObjStorage, timed
 from swh.objstorage.utils import format_obj_id
 
+MP_COUNTER_METRICS = "swh_objstorage_multiplexer_backend_total"
+MP_BACKEND_DISABLED_METRICS = "swh_objstorage_multiplexer_backend_disabled_total"
+MP_BACKEND_ENABLED_METRICS = "swh_objstorage_multiplexer_backend_enabled_total"
+
 logger = logging.getLogger(__name__)
 
+DEFAULT_TRANSIENT_READ_EXCEPTIONS = (
+    "requests.exceptions.ConnectTimeout",
+    "requests.exceptions.ReadTimeout",
+    "requests.exceptions.SSLError",
+    "requests.exceptions.ConnectionError",
+    "builtins.TimeoutError",
+    "builtins.IOError",
+)
+
 
 class ObjStorageThread(threading.Thread):
     def __init__(self, storage):
         super().__init__(daemon=True)
         self.storage = storage
         self.commands = queue.Queue()
 
@@ -125,89 +147,167 @@
 
 class MultiplexerObjStorage(ObjStorage):
     """Implementation of ObjStorage that distributes between multiple
     storages.
 
     The multiplexer object storage allows an input to be demultiplexed
     among multiple storages that will or will not accept it by
-    themselves (see .filter package).
+    themselves.
 
     As the ids can be different, no pre-computed ids should be
     submitted.  Also, there are no guarantees that the returned ids
     can be used directly into the storages that the multiplexer
     manage.
 
     Use case examples follow.
 
-    Example 1::
+    Example::
 
-        storage_v1 = filter.read_only(PathSlicingObjStorage('/dir1',
-                                                            '0:2/2:4/4:6'))
+        storage_v1 = ReadOnlyProxyObjStorage(
+                        PathSlicingObjStorage('/dir1', '0:2/2:4/4:6')
+        )
         storage_v2 = PathSlicingObjStorage('/dir2', '0:1/0:5')
         storage = MultiplexerObjStorage([storage_v1, storage_v2])
 
     When using 'storage', all the new contents will only be added to the v2
     storage, while it will be retrievable from both.
 
-    Example 2::
+    """
+
+    name: str = "multiplexer"
 
-        storage_v1 = filter.id_regex(
-            PathSlicingObjStorage('/dir1', '0:2/2:4/4:6'),
-            r'[^012].*'
+    def __init__(
+        self,
+        *,
+        objstorages: Iterable[Union[ObjStorageInterface, Dict]],
+        read_exception_cooldown: float = 5,
+        transient_read_exceptions: Optional[List[str]] = None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.storages = [
+            get_objstorage(**sto) if isinstance(sto, dict) else sto
+            for sto in objstorages
+        ]
+        self.storage_threads = [ObjStorageThread(storage) for storage in self.storages]
+        for thread in self.storage_threads:
+            thread.start()
+        self.write_storage_threads = [
+            thread
+            for thread, storage in zip(self.storage_threads, self.storages)
+            if storage.check_config(check_write=True)
+        ]
+
+        self.read_exception_cooldown = read_exception_cooldown
+        self.transient_read_exceptions = set(
+            transient_read_exceptions or DEFAULT_TRANSIENT_READ_EXCEPTIONS
         )
-        storage_v2 = filter.if_regex(
-            PathSlicingObjStorage('/dir2', '0:1/0:5'),
-            r'[012]/*'
+
+        self.active_readers: Set[int] = set()
+        self.reset_timers: Dict[int, threading.Timer] = {}
+        self.reset_active_readers()
+
+    def reset_active_readers(self):
+        """Reset the active readers set to all storages, and cancel all reset_failed_threads"""
+        for t in self.reset_timers.values():
+            if t.is_alive():
+                t.cancel()
+
+        self.reset_timers = {}
+        self.active_readers = set(range(len(self.storages)))
+
+    def disable_backend(self, endpoint: str, name: str, i: int) -> None:
+        """Mark read backend `name` at index `i` as failed, from endpoint `endpoint`."""
+        if i not in self.active_readers:
+            return
+
+        statsd.statsd.increment(
+            MP_BACKEND_DISABLED_METRICS,
+            1,
+            tags={
+                "endpoint": endpoint,
+                "name": self.name,
+                "backend": name,
+                "backend_number": i,
+            },
         )
-        storage = MultiplexerObjStorage([storage_v1, storage_v2])
 
-    When using this storage, the contents with a sha1 starting with 0, 1 or 2
-    will be redirected (read AND write) to the storage_v2, while the others
-    will be redirected to the storage_v1.  If a content starting with 0, 1 or 2
-    is present in the storage_v1, it would be ignored anyway.
+        self.active_readers.remove(i)
+        if i not in self.reset_timers:
+            reset_failed_timer = threading.Timer(
+                self.read_exception_cooldown,
+                self.enable_backend,
+                kwargs={"name": name, "i": i},
+            )
+            reset_failed_timer.start()
+            self.reset_timers[i] = reset_failed_timer
 
-    """
+        if not self.active_readers:
+            raise NoBackendsLeftError(
+                "All backends disabled due to transient failures!"
+            )
 
-    def __init__(self, storages, **kwargs):
-        super().__init__(**kwargs)
-        self.storages = storages
-        self.storage_threads = [ObjStorageThread(storage) for storage in storages]
-        for thread in self.storage_threads:
-            thread.start()
+    def enable_backend(self, name: str, i: int):
+        """Mark a reader as available again"""
+        statsd.statsd.increment(
+            MP_BACKEND_ENABLED_METRICS,
+            1,
+            tags={
+                "name": self.name,
+                "backend": name,
+                "backend_number": i,
+            },
+        )
+
+        self.active_readers.add(i)
+        if i in self.reset_timers:
+            del self.reset_timers[i]
 
     def wrap_call(self, threads, call, *args, **kwargs):
         threads = list(threads)
         mailbox = queue.Queue()
         for thread in threads:
             thread.queue_command(call, *args, mailbox=mailbox, **kwargs)
 
         return ObjStorageThread.collect_results(mailbox, len(threads))
 
     def get_read_threads(self, obj_id=None):
         yield from self.storage_threads
 
     def get_write_threads(self, obj_id=None):
-        yield from self.storage_threads
+        yield from self.write_storage_threads
 
     def check_config(self, *, check_write):
         """Check whether the object storage is properly configured.
 
+        If check_write is True, return True if at least one object storage
+        returned True.
+
         Args:
             check_write (bool): if True, check if writes to the object storage
             can succeed.
 
         Returns:
             True if the configuration check worked, an exception if it didn't.
+
         """
-        return all(
-            self.wrap_call(
-                self.storage_threads, "check_config", check_write=check_write
+        if not check_write:
+            return all(
+                self.wrap_call(
+                    self.storage_threads, "check_config", check_write=check_write
+                )
+            )
+        else:
+            return any(
+                self.wrap_call(
+                    self.storage_threads, "check_config", check_write=check_write
+                )
             )
-        )
 
+    @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         """Indicate if the given object is present in the storage.
 
         Args:
             obj_id (bytes): object identifier.
 
         Returns:
@@ -218,19 +318,21 @@
         for storage in self.get_read_threads(obj_id):
             if obj_id in storage:
                 return True
         return False
 
     def __iter__(self) -> Iterator[CompositeObjId]:
         def obj_iterator():
-            for storage in self.storages:
-                yield from storage
+            for i, storage in enumerate(self.storages):
+                if i in self.active_readers:
+                    yield from storage
 
         return obj_iterator()
 
+    @timed
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
         """Add a new object to the object storage.
 
         If the adding step works in all the storages that accept this content,
         this is a success. Otherwise, the full adding step is an error even if
         it succeed in some of the storages.
 
@@ -243,14 +345,18 @@
                 verified before adding the file.
 
         Returns:
             an id of the object into the storage. As the write-storages are
             always readable as well, any id will be valid to retrieve a
             content.
         """
+        # note: we do not have per-backend statsd metrics here because the
+        # threading scaffolding to manage IO with backends makes it a bit
+        # harder to do in a nice manner; plus metrics should be available in
+        # the backend objstorages themselves.
         self.wrap_call(
             self.get_write_threads(obj_id),
             "add",
             content,
             obj_id=obj_id,
             check_presence=check_presence,
         )
@@ -283,33 +389,62 @@
         return self.wrap_call(
             self.get_write_threads(obj_id),
             "restore",
             content,
             obj_id=obj_id,
         ).pop()
 
+    @timed
     def get(self, obj_id: ObjId) -> bytes:
         corrupted_exc: Optional[ObjCorruptedError] = None
-        for storage in self.get_read_threads(obj_id):
+        for i, storage in enumerate(self.get_read_threads(obj_id)):
+            if i not in self.active_readers:
+                continue
             try:
-                return storage.get(obj_id)
+                obj = storage.get(obj_id)
+                statsd.statsd.increment(
+                    MP_COUNTER_METRICS,
+                    1,
+                    tags={
+                        "endpoint": "get",
+                        "name": self.name,
+                        "backend": storage.storage.name,
+                        "backend_number": i,
+                    },
+                )
+                return obj
             except ObjNotFoundError:
                 continue
             except ObjCorruptedError as exc:
                 logger.warning(
-                    "Object %s was reported as corrupted by %s: %s",
+                    "Object %s was reported as corrupted by backend '%s': %s",
                     format_obj_id(obj_id),
-                    storage.storage.__class__.__name__,
+                    storage.storage.name,
                     str(exc),
                 )
                 # Hoist exception, mypy doesn't like when we directly use
                 # `except ObjCorruptedError as corrupted_exc`
                 corrupted_exc = exc
                 # Try reading from another storage
                 continue
+            except Exception as exc:
+                if isinstance(exc, ObjStorageAPIError):
+                    exc = exc.args[0]
+                exc_class = f"{exc.__class__.__module__}.{exc.__class__.__name__}"
+                if exc_class in self.transient_read_exceptions:
+                    logger.warning(
+                        "While reading object %s, received transient read "
+                        "exception on backend %s, marking backend as failed",
+                        format_obj_id(obj_id),
+                        storage.storage.name,
+                        exc_info=True,
+                    )
+                    self.disable_backend(endpoint="get", name=storage.storage.name, i=i)
+                    continue
+                raise
 
         if corrupted_exc:
             # The only objects we've found were corrupted, raise that exception
             raise corrupted_exc
         else:
             # No storage contains this content, raise the error
             raise ObjNotFoundError(obj_id)
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/objstorage.py` & `swh_objstorage-3.1.0/swh/objstorage/objstorage.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import abc
 import bz2
 import collections
 from datetime import timedelta
+import functools
 from itertools import dropwhile, islice
 import lzma
 from typing import (
     Callable,
     Dict,
     Iterable,
     Iterator,
@@ -20,20 +21,41 @@
     Tuple,
     Union,
 )
 import zlib
 
 from typing_extensions import Protocol
 
+from swh.core import statsd
 from swh.model import hashutil
 from swh.model.model import Sha1
 from swh.objstorage.constants import DEFAULT_LIMIT, ID_HASH_ALGO
 from swh.objstorage.exc import ObjCorruptedError, ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId, ObjStorageInterface
 
+DURATION_METRICS = "swh_objstorage_request_duration_seconds"
+
+
+def timed(f):
+    """A simple decorator used to add statsd probes on main ObjStorage methods
+    (add, get and __contains__)
+    """
+
+    @functools.wraps(f)
+    def w(self, *a, **kw):
+        with statsd.statsd.timed(
+            DURATION_METRICS,
+            tags={"endpoint": f.__name__, "name": self.name},
+        ):
+            return f(self, *a, **kw)
+
+    w._timed = True
+    w._f = f
+    return w
+
 
 def objid_to_default_hex(
     obj_id: ObjId, algo: Literal["sha1", "sha256"] = ID_HASH_ALGO
 ) -> str:
     """Converts SHA1 hashes and multi-hashes to the hexadecimal representation
     of the SHA1."""
     if isinstance(obj_id, bytes):
@@ -128,19 +150,30 @@
 
 CompressionFormat = Literal["bz2", "lzma", "gzip", "zlib", "none"]
 
 
 class ObjStorage(metaclass=abc.ABCMeta):
     PRIMARY_HASH: Literal["sha1", "sha256"] = "sha1"
     compression: CompressionFormat = "none"
+    name: str = "objstorage"
+    """Default objstorage name; can be overloaded at instantiation time giving a
+    'name' argument to the constructor"""
 
-    def __init__(self, *, allow_delete=False, **kwargs):
+    def __init__(
+        self: ObjStorageInterface,
+        *,
+        allow_delete: bool = False,
+        **kwargs,
+    ):
         # A more complete permission system could be used in place of that if
         # it becomes needed
         self.allow_delete = allow_delete
+        # if no name is given in kwargs, default to name defined as class attribute
+        if "name" in kwargs:
+            self.name = kwargs["name"]
 
     def add_batch(
         self: ObjStorageInterface,
         contents: Union[Mapping[Sha1, bytes], Iterable[Tuple[ObjId, bytes]]],
         check_presence: bool = True,
     ) -> Dict:
         summary = {"object:add": 0, "object:add:bytes": 0}
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/objstorage_testing.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/objstorage_testing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 # Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import inspect
-from typing import Tuple
+from typing import Optional, Tuple
 
 import pytest
 import requests
 
 from swh.objstorage.exc import ObjCorruptedError, ObjNotFoundError
+from swh.objstorage.factory import OBJSTORAGE_IMPLEMENTATIONS
 from swh.objstorage.interface import CompositeObjId, ObjStorageInterface
 from swh.objstorage.objstorage import compute_hash, decompressors
 
 
+def get_cls(sto: ObjStorageInterface) -> Optional[str]:
+    """Helper function to find the 'cls' name associated with a given
+    ObjStorage object (mostly a reverse of the OBJSTORAGE_IMPLEMENTATIONS dict
+    defined in factory.py)
+    """
+    for cls, v in OBJSTORAGE_IMPLEMENTATIONS.items():
+        if f"{sto.__class__.__module__}.{sto.__class__.__name__}" == v:
+            return cls
+    return None
+
+
 class ObjStorageTestFixture:
     num_objects = 1200
 
     @pytest.fixture(autouse=True)
     def objstorage(self, swh_objstorage):
         self.storage = swh_objstorage
 
@@ -60,14 +72,17 @@
 
         # If all the assertions above succeed, then this one should too.
         # But there's no harm in double-checking.
         # And we could replace the assertions above by this one, but unlike
         # the assertions above, it doesn't explain what is missing.
         assert isinstance(self.storage, ObjStorageInterface)
 
+    def test_name(self):
+        assert self.storage.name == get_cls(self.storage)
+
     def hash_content(self, content):
         obj_id = compute_hash(content)
         return content, obj_id
 
     def compositehash_content(self, content) -> Tuple[bytes, CompositeObjId]:
         obj_id = compute_hash(content)
         return content, {"sha1": obj_id}
@@ -112,14 +127,19 @@
         self.assertContentMatch(obj_id, content)
 
     def test_add_big(self):
         content, obj_id = self.hash_content(b"add_big" * 1024 * 1024)
         self.storage.add(content, obj_id=obj_id)
         self.assertContentMatch(obj_id, content)
 
+    def test_add_statsd(self, statsd):
+        content, obj_id = self.hash_content(b"add_get_w_id")
+        self.storage.add(content, obj_id=obj_id)
+        self.check_statsd(statsd, "add")
+
     def test_add_get_batch(self):
         content1, obj_id1 = self.hash_content(b"add_get_batch_1")
         content2, obj_id2 = self.hash_content(b"add_get_batch_2")
         self.storage.add(content1, obj_id1)
         self.storage.add(content2, obj_id2)
         cr1, cr2 = self.storage.get_batch([obj_id1, obj_id2])
         assert cr1 == content1
@@ -136,14 +156,47 @@
 
     def test_get_batch_unexisting_content(self):
         content, obj_id = self.hash_content(b"get_batch_unexisting_content")
         result = list(self.storage.get_batch([obj_id]))
         assert len(result) == 1
         assert result[0] is None
 
+    def check_statsd(self, statsd, endpoint):
+        while True:
+            stats = statsd.socket.recv()
+            assert stats
+            value, unit, tags = stats.split("|")
+            if (
+                f"name:{self.storage.name}" in tags
+                and f"endpoint:{endpoint}" in tags
+                and value.startswith("swh_objstorage_request_duration_seconds:")
+            ):
+                assert unit == "ms"
+                return
+        assert False, "Missing expected statsd message"
+
+    def test_get_statsd(self, statsd):
+        content1, obj_id1 = self.compositehash_content(b"add_get_batch_1")
+        content2, obj_id2 = self.compositehash_content(b"add_get_batch_2")
+        self.storage.add(content1, obj_id1)
+        self.storage.add(content2, obj_id2)
+        while statsd.socket.recv():
+            pass
+        content = self.storage.get(obj_id1)
+        assert content == content1
+        content = self.storage.get(obj_id2)
+        assert content == content2
+        content = self.storage.get(obj_id2)
+        content3, obj_id3 = self.hash_content(b"get_missing")
+        with pytest.raises(ObjNotFoundError):
+            self.storage.get(obj_id3)
+
+        for endpoint in ("get", "get", "get"):
+            self.check_statsd(statsd, endpoint)
+
     def test_restore_content(self):
         self.storage.allow_delete = True
 
         valid_content, valid_obj_id = self.hash_content(b"restore_content")
         invalid_content = b"unexpected content"
         self.storage.add(invalid_content, valid_obj_id)
         with pytest.raises((ObjCorruptedError, ObjNotFoundError)):
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_interface.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_api.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_api.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_azure.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_azure.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_cloud.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,38 @@
     ObjectDoesNotExistError,
     Provider,
 )
 import pytest
 
 from swh.objstorage.backends.libcloud import CloudObjStorage
 from swh.objstorage.exc import ObjCorruptedError
+from swh.objstorage.factory import OBJSTORAGE_IMPLEMENTATIONS
 from swh.objstorage.objstorage import decompressors
 
 from .objstorage_testing import ObjStorageTestFixture
 
 API_KEY = "API_KEY"
 API_SECRET_KEY = "API SECRET KEY"
 CONTAINER_NAME = "test_container"
 
 
+@pytest.fixture(scope="module", autouse=True)
+def cloud_provider_mock():
+    # register the cloud MockCloudObjStorage class defined in this file so the
+    # helper test function get_cls() defined in objstorage_testing works OK and
+    # ObjStorageTestFixture.test_name() is green here
+    OBJSTORAGE_IMPLEMENTATIONS[
+        "cloud"
+    ] = f"{MockCloudObjStorage.__module__}.{MockCloudObjStorage.__name__}"
+    try:
+        yield
+    finally:
+        del OBJSTORAGE_IMPLEMENTATIONS["cloud"]
+
+
 class MockLibcloudObject:
     """Libcloud object mock that replicates its API"""
 
     def __init__(self, name, content):
         self.name = name
         self.content = list(content)
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_http.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_http.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import pytest
 import requests
 import requests_mock
 from requests_mock.contrib import fixture
 
 from swh.model import hashutil
 from swh.objstorage.exc import (
-    NonIterableObjStorage,
+    NonIterableObjStorageError,
     ObjCorruptedError,
     ObjNotFoundError,
-    ReadOnlyObjStorage,
+    ReadOnlyObjStorageError,
 )
 from swh.objstorage.factory import get_objstorage
 from swh.objstorage.objstorage import compute_hash
 
 
 def build_objstorage(multi_hash=False):
     """Build an HTTPReadOnlyObjStorage suitable for tests
@@ -106,28 +106,28 @@
 
 
 def test_http_objstorage_read_only():
     sto_front, sto_back, objids = build_objstorage()
 
     content = b""
     obj_id = compute_hash(content)
-    with pytest.raises(ReadOnlyObjStorage):
+    with pytest.raises(ReadOnlyObjStorageError):
         sto_front.add(content, obj_id=obj_id)
-    with pytest.raises(ReadOnlyObjStorage):
+    with pytest.raises(ReadOnlyObjStorageError):
         sto_front.restore(b"", obj_id=compute_hash(b""))
-    with pytest.raises(ReadOnlyObjStorage):
+    with pytest.raises(ReadOnlyObjStorageError):
         sto_front.delete(b"\x00" * 20)
 
 
 def test_http_objstorage_not_iterable():
     sto_front, sto_back, objids = build_objstorage()
 
-    with pytest.raises(NonIterableObjStorage):
+    with pytest.raises(NonIterableObjStorageError):
         len(sto_front)
-    with pytest.raises(NonIterableObjStorage):
+    with pytest.raises(NonIterableObjStorageError):
         iter(sto_front)
 
 
 def test_http_cannonical_url():
     url = "http://127.0.0.1/content"
     sto = get_objstorage(cls="http", url=url)
     assert sto.root_path == url + "/"
```

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_instantiation.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_instantiation.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_noop.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_noop.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_pathslicing.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_random_generator.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_random_generator.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_seaweedfs.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_seaweedfs.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_objstorage_winery.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_objstorage_winery.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_pathslicer.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_pathslicer.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/test_server.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/winery_benchmark.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/winery_benchmark.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/tests/winery_testing_helpers.py` & `swh_objstorage-3.1.0/swh/objstorage/tests/winery_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh/objstorage/utils.py` & `swh_objstorage-3.1.0/swh/objstorage/utils.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/swh.objstorage.egg-info/PKG-INFO` & `swh_objstorage-3.1.0/swh.objstorage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 3.0.2
+Version: 3.1.0
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: click
+Requires-Dist: deprecated
 Requires-Dist: msgpack
 Requires-Dist: typing-extensions>=3.7.4
 Requires-Dist: requests
 Requires-Dist: swh.core[http]>=3.0.0
 Requires-Dist: swh.model>=0.0.27
 Requires-Dist: swh.perfecthash>=1.3.0
 Provides-Extra: azure
```

### Comparing `swh_objstorage-3.0.2/swh.objstorage.egg-info/SOURCES.txt` & `swh_objstorage-3.1.0/swh.objstorage.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 swh.objstorage.egg-info/requires.txt
 swh.objstorage.egg-info/top_level.txt
 swh/objstorage/cli.py
 swh/objstorage/constants.py
 swh/objstorage/exc.py
 swh/objstorage/factory.py
 swh/objstorage/interface.py
+swh/objstorage/multiplexer.py
 swh/objstorage/objstorage.py
 swh/objstorage/py.typed
 swh/objstorage/pytest_plugin.py
 swh/objstorage/utils.py
 swh/objstorage/api/client.py
 swh/objstorage/api/server.py
 swh/objstorage/backends/__init__.py
@@ -66,19 +67,15 @@
 swh/objstorage/backends/winery/rwshard.py
 swh/objstorage/backends/winery/sharedbase.py
 swh/objstorage/backends/winery/sleep.py
 swh/objstorage/backends/winery/stats.py
 swh/objstorage/backends/winery/throttler.py
 swh/objstorage/backends/winery/sql/30-schema.sql
 swh/objstorage/backends/winery/sql/__init__.py
-swh/objstorage/multiplexer/__init__.py
-swh/objstorage/multiplexer/multiplexer_objstorage.py
-swh/objstorage/multiplexer/filter/__init__.py
-swh/objstorage/multiplexer/filter/filter.py
-swh/objstorage/multiplexer/filter/read_write_filter.py
+swh/objstorage/proxies/readonly.py
 swh/objstorage/tests/__init__.py
 swh/objstorage/tests/objstorage_testing.py
 swh/objstorage/tests/test_interface.py
 swh/objstorage/tests/test_objstorage_api.py
 swh/objstorage/tests/test_objstorage_azure.py
 swh/objstorage/tests/test_objstorage_cloud.py
 swh/objstorage/tests/test_objstorage_http.py
```

### Comparing `swh_objstorage-3.0.2/tox.ini` & `swh_objstorage-3.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/README.md` & `swh_objstorage-3.1.0/winery-test-environment/README.md`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/bootstrap.yml` & `swh_objstorage-3.1.0/winery-test-environment/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/build-vms.sh` & `swh_objstorage-3.1.0/winery-test-environment/build-vms.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/ceph.yml` & `swh_objstorage-3.1.0/winery-test-environment/ceph.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/fed4fire.rspec` & `swh_objstorage-3.1.0/winery-test-environment/fed4fire.rspec`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/fed4fire.sh` & `swh_objstorage-3.1.0/winery-test-environment/fed4fire.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/grid5000.yml` & `swh_objstorage-3.1.0/winery-test-environment/grid5000.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/inventory/hosts.yml` & `swh_objstorage-3.1.0/winery-test-environment/inventory/hosts.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/mitogen.py` & `swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/mitogen_free.py` & `swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py` & `swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/mitogen-strategy/mitogen_linear.py` & `swh_objstorage-3.1.0/winery-test-environment/mitogen-strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/osd.yml` & `swh_objstorage-3.1.0/winery-test-environment/osd.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/remote-tox.sh` & `swh_objstorage-3.1.0/winery-test-environment/remote-tox.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/render-stats.py` & `swh_objstorage-3.1.0/winery-test-environment/render-stats.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/rw.yml` & `swh_objstorage-3.1.0/winery-test-environment/rw.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.0.2/winery-test-environment/tests.yml` & `swh_objstorage-3.1.0/winery-test-environment/tests.yml`

 * *Files identical despite different names*

