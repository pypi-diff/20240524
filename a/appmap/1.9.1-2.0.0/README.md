# Comparing `tmp/appmap-1.9.1.tar.gz` & `tmp/appmap-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appmap-1.9.1.tar", max compression
+gzip compressed data, was "appmap-2.0.0.tar", max compression
```

## Comparing `appmap-1.9.1.tar` & `appmap-2.0.0.tar`

### file list

```diff
@@ -1,131 +1,163 @@
--rw-r--r--   0        0        0     1925 2022-10-11 15:21:34.391612 appmap-1.9.1/LICENSE
--rw-r--r--   0        0        0     4678 2022-10-11 15:21:34.391612 appmap-1.9.1/README.md
--rw-r--r--   0        0        0      471 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/__init__.py
--rw-r--r--   0        0        0      431 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/__init__.py
--rw-r--r--   0        0        0    10672 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/configuration.py
--rw-r--r--   0        0        0     3421 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/env.py
--rw-r--r--   0        0        0    13581 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/event.py
--rw-r--r--   0        0        0     3413 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/generation.py
--rw-r--r--   0        0        0     9914 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/importer.py
--rw-r--r--   0        0        0     4312 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/instrument.py
--rw-r--r--   0        0        0     1859 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/labels.py
--rw-r--r--   0        0        0     3924 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/metadata.py
--rw-r--r--   0        0        0      538 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/py_version_check.py
--rw-r--r--   0        0        0     4736 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/recorder.py
--rw-r--r--   0        0        0     1101 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/recording.py
--rw-r--r--   0        0        0     3949 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/testing_framework.py
--rw-r--r--   0        0        0     5180 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap/_implementation/utils.py
--rw-r--r--   0        0        0     7588 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/_implementation/web_framework.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/command/__init__.py
--rw-r--r--   0        0        0      435 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/command/appmap_agent_init.py
--rw-r--r--   0        0        0     3433 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/command/appmap_agent_status.py
--rw-r--r--   0        0        0     2103 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/command/appmap_agent_validate.py
--rw-r--r--   0        0        0    12163 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/django.py
--rw-r--r--   0        0        0     5551 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/flask.py
--rw-r--r--   0        0        0     2722 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/http.py
--rw-r--r--   0        0        0      605 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/labeling/__init__.py
--rw-r--r--   0        0        0     3387 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/labeling/crypto.yml
--rw-r--r--   0        0        0      273 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/labeling/formats.yml
--rw-r--r--   0        0        0       50 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/labeling/http.yml
--rw-r--r--   0        0        0      196 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/labeling/jobs.yml
--rw-r--r--   0        0        0     2855 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/pytest.py
--rw-r--r--   0        0        0     2329 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/sqlalchemy.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/__init__.py
--rw-r--r--   0        0        0     3550 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/appmap_test_base.py
--rw-r--r--   0        0        0     2723 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/conftest.py
--rw-r--r--   0        0        0       50 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/appmap-broken.yml
--rw-r--r--   0        0        0       82 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/appmap-class.yml
--rw-r--r--   0        0        0       87 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/appmap-func.yml
--rw-r--r--   0        0        0      300 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/appmap.yml
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/config/src/package/__init__.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/config/test/__init__.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/config/test/foo.py
--rw-r--r--   0        0        0       16 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/config-exclude/.hide/hidden_mod/__init__.py
--rw-r--r--   0        0        0       25 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/config-exclude/node_modules/node_mod/__init__.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/config-exclude/src/package/__init__.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/config-exclude/test/__init__.py
--rw-r--r--   0        0        0       14 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/config-exclude/venv/venv_mod/__init__.py
--rw-r--r--   0        0        0      458 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/app/__init__.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/app/app.py
--rw-r--r--   0        0        0       39 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/app/hello_world.html
--rw-r--r--   0        0        0      154 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/app/middleware.py
--rw-r--r--   0        0        0      554 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/app/settings.py
--rw-r--r--   0        0        0     1917 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/app/urls.py
--rw-r--r--   0        0        0       38 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/appmap.yml
--rwxr-xr-x   0        0        0      659 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/manage.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/test/__init__.py
--rw-r--r--   0        0        0      453 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/django/test/test_app.py
--rw-r--r--   0        0        0     2591 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/example_class.py
--rw-r--r--   0        0        0     7826 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/expected.appmap.json
--rw-r--r--   0        0        0      930 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/flask/app.py
--rw-r--r--   0        0        0       38 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/flask/appmap.yml
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/flask/templates/test.html
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/package1/__init__.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/package1/package2/__init__.py
--rw-r--r--   0        0        0       69 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/package1/package2/mod1.py
--rw-r--r--   0        0        0      653 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/params.py
--rw-r--r--   0        0        0       38 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/pytest/appmap.yml
--rw-r--r--   0        0        0     2958 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/pytest/expected/pytest.appmap.json
--rw-r--r--   0        0        0      113 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/pytest/expected/status_failed.metadata.json
--rw-r--r--   0        0        0      186 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/pytest/simple.py
--rw-r--r--   0        0        0      393 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/pytest/test_simple.py
--rw-r--r--   0        0        0     1622 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/remote.appmap.json
--rw-r--r--   0        0        0       18 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/trial/.gitignore
--rw-r--r--   0        0        0       38 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/trial/appmap.yml
--rw-r--r--   0        0        0     1899 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/trial/expected/pytest.appmap.json
--rw-r--r--   0        0        0       14 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/trial/init/sitecustomize.py
--rw-r--r--   0        0        0        0 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/trial/test/__init__.py
--rw-r--r--   0        0        0      386 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/trial/test/test_deferred.py
--rw-r--r--   0        0        0        6 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/.gitignore
--rw-r--r--   0        0        0       38 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/appmap.yml
--rw-r--r--   0        0        0     4430 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/expected/pytest.appmap.json
--rw-r--r--   0        0        0      109 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/expected/status_errored.metadata.json
--rw-r--r--   0        0        0      118 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/expected/status_failed.metadata.json
--rw-r--r--   0        0        0       33 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/expected/status_xsucceeded.metadata.json
--rw-r--r--   0        0        0     4432 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/expected/unittest.appmap.json
--rw-r--r--   0        0        0       14 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/init/sitecustomize.py
--rw-r--r--   0        0        0      275 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/simple/__init__.py
--rw-r--r--   0        0        0      991 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/data/unittest/simple/test_simple.py
--rw-r--r--   0        0        0      440 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/helpers.py
--rw-r--r--   0        0        0     4182 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/normalize.py
--rw-r--r--   0        0        0     4862 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_command.py
--rw-r--r--   0        0        0     6287 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_configuration.py
--rw-r--r--   0        0        0     7026 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_django.py
--rw-r--r--   0        0        0     3258 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_events.py
--rw-r--r--   0        0        0     3024 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_flask.py
--rw-r--r--   0        0        0     2266 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_generation.py
--rw-r--r--   0        0        0     1258 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_http.py
--rw-r--r--   0        0        0      865 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_importer.py
--rw-r--r--   0        0        0     1979 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_metadata.py
--rw-r--r--   0        0        0     9754 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_params.py
--rw-r--r--   0        0        0     5474 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_recording.py
--rw-r--r--   0        0        0     2738 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_sqlalchemy.py
--rw-r--r--   0        0        0     5063 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_test_frameworks.py
--rw-r--r--   0        0        0      362 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/test_util.py
--rw-r--r--   0        0        0    13577 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/test/web_framework.py
--rw-r--r--   0        0        0     1933 2022-10-11 15:21:34.395612 appmap-1.9.1/appmap/unittest.py
--rw-r--r--   0        0        0       13 2022-10-11 15:21:34.391612 appmap-1.9.1/appmap.pth
--rw-r--r--   0        0        0     2813 2022-10-11 15:40:11.139546 appmap-1.9.1/pyproject.toml
--rw-r--r--   0        0        0      658 2022-10-11 15:21:34.915665 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__init__.py
--rw-r--r--   0        0        0      972 2022-10-11 15:34:51.668291 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      966 2022-10-11 15:25:29.815421 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      970 2022-10-11 15:28:10.135058 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      970 2022-10-11 15:31:22.477058 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9216 2022-10-11 15:34:51.676291 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/decorators.cpython-310.pyc
--rw-r--r--   0        0        0     9077 2022-10-11 15:25:29.819421 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/decorators.cpython-37.pyc
--rw-r--r--   0        0        0     9242 2022-10-11 15:28:10.143058 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/decorators.cpython-38.pyc
--rw-r--r--   0        0        0     9294 2022-10-11 15:31:22.485058 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/decorators.cpython-39.pyc
--rw-r--r--   0        0        0     4266 2022-10-11 15:34:51.676291 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/importer.cpython-310.pyc
--rw-r--r--   0        0        0     4194 2022-10-11 15:25:29.823422 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/importer.cpython-37.pyc
--rw-r--r--   0        0        0     4250 2022-10-11 15:28:10.143058 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/importer.cpython-38.pyc
--rw-r--r--   0        0        0     4274 2022-10-11 15:31:22.485058 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/importer.cpython-39.pyc
--rw-r--r--   0        0        0    25103 2022-10-11 15:34:51.672291 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/wrappers.cpython-310.pyc
--rw-r--r--   0        0        0    25550 2022-10-11 15:25:29.819421 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/wrappers.cpython-37.pyc
--rw-r--r--   0        0        0    25601 2022-10-11 15:28:10.139058 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/wrappers.cpython-38.pyc
--rw-r--r--   0        0        0    25631 2022-10-11 15:31:22.485058 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/__pycache__/wrappers.cpython-39.pyc
--rw-r--r--   0        0        0    92703 2022-10-11 15:21:34.915665 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/_wrappers.c
--rw-r--r--   0        0        0    20247 2022-10-11 15:21:34.915665 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/decorators.py
--rw-r--r--   0        0        0     7896 2022-10-11 15:21:34.915665 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/importer.py
--rw-r--r--   0        0        0    36016 2022-10-11 15:21:34.915665 appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/wrappers.py
--rw-r--r--   0        0        0     7131 1970-01-01 00:00:00.000000 appmap-1.9.1/setup.py
--rw-r--r--   0        0        0     5954 1970-01-01 00:00:00.000000 appmap-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1925 2024-05-23 19:26:41.876407 appmap-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4534 2024-05-23 19:26:41.876407 appmap-2.0.0/README.md
+-rw-r--r--   0        0        0      502 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/__init__.py
+-rw-r--r--   0        0        0    15857 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/configuration.py
+-rw-r--r--   0        0        0     1082 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/django.py
+-rw-r--r--   0        0        0     6699 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/env.py
+-rw-r--r--   0        0        0    15677 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/event.py
+-rw-r--r--   0        0        0      694 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/fastapi.py
+-rw-r--r--   0        0        0      822 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/flask.py
+-rw-r--r--   0        0        0     3573 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/generation.py
+-rw-r--r--   0        0        0    11495 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/importer.py
+-rw-r--r--   0        0        0     4323 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/instrument.py
+-rw-r--r--   0        0        0     1786 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/labels.py
+-rw-r--r--   0        0        0     3071 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/metadata.py
+-rw-r--r--   0        0        0      267 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/noappmap.py
+-rw-r--r--   0        0        0      538 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/py_version_check.py
+-rw-r--r--   0        0        0     5513 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/recorder.py
+-rw-r--r--   0        0        0     2868 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/recording.py
+-rw-r--r--   0        0        0      926 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/remote_recording.py
+-rw-r--r--   0        0        0      340 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/singleton.py
+-rw-r--r--   0        0        0      174 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/__init__.py
+-rw-r--r--   0        0        0     3607 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/appmap_test_base.py
+-rwxr-xr-x   0        0        0      121 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/bin/server_runner
+-rw-r--r--   0        0        0     6048 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/conftest.py
+-rw-r--r--   0        0        0      112 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap-all-paths-malformed.yml
+-rw-r--r--   0        0        0       50 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap-broken.yml
+-rw-r--r--   0        0        0       82 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap-class.yml
+-rw-r--r--   0        0        0       59 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap-empty-path.yml
+-rw-r--r--   0        0        0      126 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap-exclude-fn.yml
+-rw-r--r--   0        0        0       87 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap-func.yml
+-rw-r--r--   0        0        0       82 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap-malformed-path.yml
+-rw-r--r--   0        0        0      308 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap-no-pyyaml.yml
+-rw-r--r--   0        0        0      323 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap_testing/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/appmap_testing/django_simplelazyobject.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config/src/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config/test/foo.py
+-rw-r--r--   0        0        0       16 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config-exclude/.hide/hidden_mod/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config-exclude/node_modules/node_mod/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config-exclude/src/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config-exclude/test/__init__.py
+-rw-r--r--   0        0        0       14 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config-exclude/venv/venv_mod/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config-up/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config-up/project/p1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/config-up/project/p2/sub1/__init__.py
+-rw-r--r--   0        0        0       44 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/appmap.yml
+-rw-r--r--   0        0        0      495 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/djangoapp/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/djangoapp/djangoapp.py
+-rw-r--r--   0        0        0       39 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/djangoapp/hello_world.html
+-rw-r--r--   0        0        0      154 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/djangoapp/middleware.py
+-rw-r--r--   0        0        0      426 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/djangoapp/settings.py
+-rw-r--r--   0        0        0      563 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/djangoapp/settings_dev.py
+-rw-r--r--   0        0        0     2148 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/djangoapp/urls.py
+-rw-r--r--   0        0        0       14 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/init/sitecustomize.py
+-rwxr-xr-x   0        0        0      665 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/manage.py
+-rw-r--r--   0        0        0       53 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/pytest.ini
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/test/__init__.py
+-rw-r--r--   0        0        0      935 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/django/test/test_app.py
+-rw-r--r--   0        0        0     2591 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/example_class.py
+-rw-r--r--   0        0        0     7942 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/expected.appmap.json
+-rw-r--r--   0        0        0       47 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/fastapi/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/fastapi/fastapiapp/__init__.py
+-rw-r--r--   0        0        0     1647 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/fastapi/fastapiapp/main.py
+-rw-r--r--   0        0        0       14 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/fastapi/init/sitecustomize.py
+-rw-r--r--   0        0        0      240 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/fastapi/test_app.py
+-rw-r--r--   0        0        0       38 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/flask/appmap.yml
+-rw-r--r--   0        0        0     1200 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/flask/flaskapp.py
+-rw-r--r--   0        0        0       14 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/flask/init/sitecustomize.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/flask/templates/test.html
+-rw-r--r--   0        0        0      268 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/flask/test_app.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/package1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/package1/package2/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/package1/package2/__main__.py
+-rw-r--r--   0        0        0       69 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/package1/package2/mod1.py
+-rw-r--r--   0        0        0      653 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/params.py
+-rw-r--r--   0        0        0       38 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/pytest/appmap.yml
+-rw-r--r--   0        0        0     2931 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/pytest/expected/pytest.appmap.json
+-rw-r--r--   0        0        0      213 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/pytest/expected/status_errored.metadata.json
+-rw-r--r--   0        0        0      221 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/pytest/expected/status_failed.metadata.json
+-rw-r--r--   0        0        0      221 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/pytest/expected/status_xfailed.metadata.json
+-rw-r--r--   0        0        0      186 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/pytest/simple.py
+-rw-r--r--   0        0        0      295 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/pytest/test_noappmap.py
+-rw-r--r--   0        0        0      393 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/pytest/test_simple.py
+-rw-r--r--   0        0        0     1246 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/remote.appmap.json
+-rw-r--r--   0        0        0       13 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/trial/.gitignore
+-rw-r--r--   0        0        0       38 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/trial/appmap.yml
+-rw-r--r--   0        0        0     1897 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/trial/expected/pytest.appmap.json
+-rw-r--r--   0        0        0       14 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/trial/init/sitecustomize.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/trial/test/__init__.py
+-rw-r--r--   0        0        0      400 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/trial/test/test_deferred.py
+-rw-r--r--   0        0        0       38 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/appmap.yml
+-rw-r--r--   0        0        0     4428 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/expected/pytest.appmap.json
+-rw-r--r--   0        0        0      220 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/expected/status_errored.metadata.json
+-rw-r--r--   0        0        0      238 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/expected/status_failed.metadata.json
+-rw-r--r--   0        0        0      238 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/expected/status_xfailed.metadata.json
+-rw-r--r--   0        0        0       33 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/expected/status_xsucceeded.metadata.json
+-rw-r--r--   0        0        0     4430 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/expected/unittest.appmap.json
+-rw-r--r--   0        0        0       14 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/init/sitecustomize.py
+-rw-r--r--   0        0        0      275 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/simple/__init__.py
+-rw-r--r--   0        0        0      183 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/simple/test_noappmap.py
+-rw-r--r--   0        0        0     1263 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/data/unittest/simple/test_simple.py
+-rw-r--r--   0        0        0      734 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/helpers.py
+-rw-r--r--   0        0        0     4761 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/normalize.py
+-rw-r--r--   0        0        0     4983 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/test_command.py
+-rw-r--r--   0        0        0    11609 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/test_configuration.py
+-rw-r--r--   0        0        0     3401 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/test_describe_value.py
+-rw-r--r--   0        0        0     8341 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/test_django.py
+-rw-r--r--   0        0        0      943 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/test_django_simplelazyobject.py
+-rw-r--r--   0        0        0      338 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/test_env.py
+-rw-r--r--   0        0        0     3198 2024-05-23 19:26:41.880407 appmap-2.0.0/_appmap/test/test_events.py
+-rw-r--r--   0        0        0     2732 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_fastapi.py
+-rw-r--r--   0        0        0     5065 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_flask.py
+-rw-r--r--   0        0        0     1703 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_generation.py
+-rw-r--r--   0        0        0     1548 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_http.py
+-rw-r--r--   0        0        0     1533 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_importer.py
+-rw-r--r--   0        0        0     2931 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_labels.py
+-rw-r--r--   0        0        0     1470 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_metadata.py
+-rw-r--r--   0        0        0     9877 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_params.py
+-rw-r--r--   0        0        0     6706 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_recording.py
+-rw-r--r--   0        0        0     2006 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_runner.py
+-rw-r--r--   0        0        0     3086 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7261 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_test_frameworks.py
+-rw-r--r--   0        0        0      861 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/test_util.py
+-rw-r--r--   0        0        0    15340 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/test/web_framework.py
+-rw-r--r--   0        0        0     4828 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/testing_framework.py
+-rw-r--r--   0        0        0      370 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/trace_logger.py
+-rw-r--r--   0        0        0     2950 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/unittest.py
+-rw-r--r--   0        0        0     6652 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/utils.py
+-rw-r--r--   0        0        0     8622 2024-05-23 19:26:41.884408 appmap-2.0.0/_appmap/web_framework.py
+-rw-r--r--   0        0        0     1731 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/command/__init__.py
+-rw-r--r--   0        0        0      420 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/command/appmap_agent_init.py
+-rw-r--r--   0        0        0     3475 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/command/appmap_agent_status.py
+-rw-r--r--   0        0        0     2096 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/command/appmap_agent_validate.py
+-rw-r--r--   0        0        0     3874 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/command/runner.py
+-rw-r--r--   0        0        0    11401 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/django.py
+-rw-r--r--   0        0        0     6590 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/fastapi.py
+-rw-r--r--   0        0        0     7219 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/flask.py
+-rw-r--r--   0        0        0     2695 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/http.py
+-rw-r--r--   0        0        0      675 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/__init__.py
+-rw-r--r--   0        0        0     3387 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/crypto.yml
+-rw-r--r--   0        0        0     2097 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/django.yml
+-rw-r--r--   0        0        0      630 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/flask.yml
+-rw-r--r--   0        0        0      831 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/formats.yml
+-rw-r--r--   0        0        0       50 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/http.yml
+-rw-r--r--   0        0        0      196 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/jobs.yml
+-rw-r--r--   0        0        0       55 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/jwt.yml
+-rw-r--r--   0        0        0      137 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/logger.yml
+-rw-r--r--   0        0        0      214 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/labeling/random.yml
+-rw-r--r--   0        0        0     3282 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/pytest.py
+-rw-r--r--   0        0        0     2295 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/sqlalchemy.py
+-rw-r--r--   0        0        0      294 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/unittest.py
+-rw-r--r--   0        0        0      818 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap/uvicorn.py
+-rw-r--r--   0        0        0       14 2024-05-23 19:26:41.884408 appmap-2.0.0/appmap.pth
+-rw-r--r--   0        0        0     3272 2024-05-23 19:29:36.879827 appmap-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1304 2024-05-23 19:26:41.884408 appmap-2.0.0/vendor/_appmap/wrapt/LICENSE
+-rw-r--r--   0        0        0     1200 2024-05-23 19:26:41.884408 appmap-2.0.0/vendor/_appmap/wrapt/__init__.py
+-rw-r--r--   0        0        0     1746 2024-05-23 19:26:41.884408 appmap-2.0.0/vendor/_appmap/wrapt/arguments.py
+-rw-r--r--   0        0        0    21332 2024-05-23 19:26:41.884408 appmap-2.0.0/vendor/_appmap/wrapt/decorators.py
+-rw-r--r--   0        0        0    10782 2024-05-23 19:26:41.884408 appmap-2.0.0/vendor/_appmap/wrapt/importer.py
+-rw-r--r--   0        0        0    38753 2024-05-23 19:26:41.884408 appmap-2.0.0/vendor/_appmap/wrapt/wrappers.py
+-rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 appmap-2.0.0/PKG-INFO
```

### Comparing `appmap-1.9.1/LICENSE` & `appmap-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `appmap-1.9.1/README.md` & `appmap-2.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 - [About](#about)
 - [Usage](#usage)
 - [Development](#development)
   - [Getting the code](#getting-the-code)
   - [Python version support](#python-version-support)
   - [Dependency management](#dependency-management)
+    - [wrapt](#wrapt)
   - [Linting](#linting)
   - [Testing](#testing)
     - [pytest](#pytest)
     - [tox](#tox)
   - [Code Coverage](#code-coverage)
 
 # About
@@ -21,42 +22,28 @@
 
 # Usage
 
 Visit the [AppMap for Python](https://appland.com/docs/reference/appmap-python.html) reference page on AppLand.com for a complete reference guide.
 
 # Development
 
-[![Build Status](https://travis-ci.com/applandinc/appmap-python.svg?branch=master)](https://travis-ci.com/applandinc/appmap-python)
+[![Build Status](https://travis-ci.com/getappmap/appmap-python.svg?branch=master)](https://travis-ci.com/getappmap/appmap-python)
 
 ## Getting the code
-Clone the repo to begin development. Note that vendored dependencies are included as
-submodules.
+Clone the repo to begin development.
 
 ```shell
-% git clone --recurse-submodules https://github.com/applandinc/appmap-python.git
+% git clone https://github.com/applandinc/appmap-python.git
 Cloning into 'appmap-python'...
 remote: Enumerating objects: 167, done.
 remote: Counting objects: 100% (167/167), done.
 remote: Compressing objects: 100% (100/100), done.
 remote: Total 962 (delta 95), reused 116 (delta 61), pack-reused 795
 Receiving objects: 100% (962/962), 217.31 KiB | 4.62 MiB/s, done.
 Resolving deltas: 100% (653/653), done.
-Submodule 'extern/wrapt' (https://github.com/applandinc/wrapt.git) registered for path 'vendor/wrapt'
-Cloning into '/private/tmp/appmap-python/vendor/wrapt'...
-remote: Enumerating objects: 46, done.
-remote: Counting objects: 100% (46/46), done.
-remote: Compressing objects: 100% (39/39), done.
-remote: Total 2537 (delta 9), reused 19 (delta 4), pack-reused 2491
-Receiving objects: 100% (2537/2537), 755.94 KiB | 7.48 MiB/s, done.
-Resolving deltas: 100% (1643/1643), done.
-Submodule path 'vendor/wrapt': checked out '9bdfbe54b88a64069cba1f3c36e77edc3c1339c9'
-
-% ls appmap-python/vendor/wrapt
-LICENSE		Makefile	appveyor.yml	docs		src		tests
-MANIFEST.in	README.rst	blog		setup.py	tddium.yml	tox.ini
 ```
 
 ## Python version support
 As a package intended to be installed in as many environments as possible, `appmap-python`
 needs to avoid using features of Python or the standard library that were added after the
 oldest version currently supported (see the
 [supported versions](https://appland.com/docs/reference/appmap-python.html#supported-versions)).
@@ -67,49 +54,61 @@
 
 ```
 % brew install poetry
 % cd appmap-python
 % poetry install
 ```
 
+### wrapt
+The one dependency that is not managed using `poetry` is `wrapt`. Because it's possible that
+projects that use `appmap` may also need an unmodified version of `wrapt` (e.g. `pylint` depends on
+`astroid`, which in turn depends on `wrapt`), we use
+[vendoring](https://github.com/pradyunsg/vendoring) to vendor `wrapt`.
+
+To update `wrapt`, use `tox` (described below) to run the `vendoring` environment.
+
 ## Linting
 [pylint](https://www.pylint.org/) for linting:
 
 ```
 % cd appmap-python
 % poetry run pylint appmap
 
 --------------------------------------------------------------------
 Your code has been rated at 10.00/10 (previous run: 10.00/10, +0.00)
 
 ```
 
-[Note that the current configuration requires a 10.0 for the Travis build to pass. To make
-this easier to achieve, convention and refactoring checks have both been disabled. They
-should be reenabled as soon as possible.]
+[Note that the current configuration has a threshold set which must be met for the Travis build to
+pass. To make this easier to achieve, a number of checks have both been disabled. They should be
+reenabled as soon as possible.]
 
 
 ## Testing
 ### pytest
 
 Note that you must install the dependencies contained in
-[requirements-test.txt](requirements-test.txt) before running tests. See the explanation in
+[requirements-dev.txt](requirements-dev.txt) before running tests. See the explanation in
 [pyproject.toml](pyproject.toml) for details.
 
+Additionally, the tests currently require that you set `APPMAP=true`. You can
+either run `pytest` with `appmap-python` (see [tox.ini](tox.ini)), or you can explicitly
+set the environment variable.
+
 [pytest](https://docs.pytest.org/en/stable/) for testing:
 
 ```
 % cd appmap-python
 % pip install -r requirements-test.txt
 % poetry run pytest
 ```
 
 ### tox
 Additionally, the `tox` configuration provides the ability to run the tests for all
-supported versions of Python and djanggo. 
+supported versions of Python and Django.
 
 `tox` requires that all the correct versions of Python to be available to create
 the test environments. [pyenv](https://github.com/pyenv/pyenv) is an easy way to manage
 multiple versions of Python, and the [xxenv-latest
 plugin](https://github.com/momo-lab/xxenv-latest) can help get all the latest versions.
```

### Comparing `appmap-1.9.1/appmap/_implementation/event.py` & `appmap-2.0.0/_appmap/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+# pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
 import inspect
 import logging
 import threading
 from functools import lru_cache, partial
 from inspect import Parameter, Signature
 from itertools import chain
 
 from .env import Env
 from .recorder import Recorder
 from .utils import (
     FnType,
+    FqFnName,
     appmap_tls,
     compact_dict,
     fqname,
     get_function_location,
-    split_function_name,
 )
 
-logger = logging.getLogger(__name__)
+logger = Env.current.getLogger(__name__)
 
 
 class _EventIds:
     # The identifiers returned by threading.get_ident() aren't
     # guaranteed to be unique: they may be recycled after the thread
     # exits. We need a unique id, so we'll manage it ourselves.
     _next_thread_id = 0
@@ -59,30 +60,73 @@
         class_name = fqname(type(val))
         object_id = id(val)
         value = "<%s object at %#02x>" % (class_name, object_id)
 
     return value
 
 
-def describe_value(val):
+def _is_list_or_dict(val_type):
+    # We cannot use isinstance here because it uses __class__
+    # and val could be overloading it and calling it could cause side effects.
+    #
+    # For example lazy objects such as django.utils.functional.LazyObject
+    # pretend to be the wrapped object, but they don't know its class
+    # a priori, so __class__ attribute lookup has to force evaluation.
+    # If the object hasn't been evaluated before it could change the
+    # observed behavior by doing that prematurely (perhaps even before
+    # the evaluation can even succeed).
+
+    return issubclass(val_type, list), issubclass(val_type, dict)
+
+
+def _describe_schema(name, val, depth, max_depth):
+
+    val_type = type(val)
+
+    ret = {}
+    if name is not None:
+        ret["name"] = name
+    ret["class"] = fqname(val_type)
+
+    islist, isdict = _is_list_or_dict(val_type)
+    if not (islist or isdict) or (depth >= max_depth and isdict):
+        return ret
+
+    if islist:
+        elts = [(None, v) for v in val]
+        schema_key = "items"
+    elif isdict:
+        elts = val.items()
+        schema_key = "properties"
+
+    schema = [_describe_schema(k, v, depth + 1, max_depth) for k, v in elts]
+    # schema will be [None] if depth is exceeded, don't use it
+    if any(schema):
+        ret[schema_key] = schema
+
+    return ret
+
+
+def describe_value(name, val, max_depth=5):
     ret = {
-        "class": fqname(type(val)),
         "object_id": id(val),
         "value": display_string(val),
     }
-    if isinstance(val, list) or isinstance(val, dict):
+    ret.update(_describe_schema(name, val, 0, max_depth))
+    if any(_is_list_or_dict(type(val))):
         ret["size"] = len(val)
+
     return ret
 
 
 class Event:
     __slots__ = ["id", "event", "thread_id"]
 
     def __init__(self, event):
-        self.id = Recorder.get_current().next_event_id()
+        self.id = Recorder.next_event_id()
         self.event = event
         self.thread_id = _EventIds.get_thread_id()
 
     def to_dict(self, attrs=None):
         ret = {}
         if attrs is None:
             attrs = chain.from_iterable(
@@ -103,18 +147,15 @@
 
 class Param:
     __slots__ = ["name", "kind", "default", "default_class"]
 
     def __init__(self, sigp):
         self.name = sigp.name
         has_default = sigp.default is not Signature.empty
-        if (
-            sigp.kind == Parameter.POSITIONAL_ONLY
-            or sigp.kind == Parameter.POSITIONAL_OR_KEYWORD
-        ):  # noqa: E129
+        if sigp.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD):
             self.kind = "opt" if has_default else "req"
         elif sigp.kind == Parameter.VAR_POSITIONAL:
             self.kind = "rest"
         elif sigp.kind == Parameter.KEYWORD_ONLY:
             self.kind = "key" if has_default else "keyreq"
         elif sigp.kind == Parameter.VAR_KEYWORD:
             self.kind = "keyrest"
@@ -122,21 +163,22 @@
             self.default = sigp.default
             self.default_class = fqname(type(self.default))
 
     def __repr__(self):
         return "<Param name: %s kind: %s>" % (self.name, self.kind)
 
     def to_dict(self, value):
-        ret = {"name": self.name, "kind": self.kind}
-        ret.update(describe_value(value))
+        ret = {"kind": self.kind}
+        ret.update(describe_value(self.name, value))
         return ret
 
 
 class CallEvent(Event):
-    __slots__ = ["_fn", "static", "receiver", "parameters", "labels"]
+    # pylint: disable=method-cache-max-size-none
+    __slots__ = ["_fn", "_fqfn", "static", "receiver", "parameters", "labels"]
 
     @staticmethod
     def make(fn, fntype):
         """
         Return a factory for creating new CallEvents based on
         introspecting the given function.
         """
@@ -164,23 +206,23 @@
 
         if logger.isEnabledFor(logging.DEBUG):
             # inspect.signature is relatively expensive, and signature
             # mismatches are frequent. Only compare them if we're
             # going to log a message about a mismatch.
             wrapped_sig = inspect.signature(fn, follow_wrapped=True)
             if sig != wrapped_sig:
-                logger.debug(
-                    "signature of wrapper %s.%s doesn't match wrapped",
-                    *split_function_name(fn)
-                )
+                logger.debug("signature of wrapper %r doesn't match wrapped", fn)
+                logger.debug("sig: %r", sig)
+                logger.debug("wrapped_sig: %r", wrapped_sig)
 
         return [Param(p) for p in sig.parameters.values()]
 
     @staticmethod
     def set_params(params, instance, args, kwargs):
+        # pylint: disable=too-many-branches
         # Note that set_params expects args and kwargs as a tuple and
         # dict, respectively. It operates on them as collections, so
         # it doesn't unpack them.
         ret = []
 
         # HACK: this is to detect cases when this is a method, yet the self
         # parameter is None. Unfortunately wrapt tries to be too smart
@@ -209,15 +251,15 @@
                     else:
                         continue  # required argument missing
             elif p.kind == "keyreq":
                 if p.name in kwargs:
                     value = kwargs[p.name]
                 else:
                     continue  # required argument missing
-            elif p.kind == "opt" or p.kind == "key":
+            elif p.kind in ("opt", "key"):
                 value = kwargs.get(p.name, p.default)
             elif p.kind == "rest":
                 value = tuple(args)
             elif p.kind == "keyrest":
                 value = kwargs
             else:
                 # If all the parameter types are handled, this
@@ -225,25 +267,25 @@
                 raise RuntimeError("Unknown parameter with desc %s" % (repr(p)))
             ret.append(p.to_dict(value))
         return ret
 
     @property
     @lru_cache(maxsize=None)
     def function_name(self):
-        return split_function_name(self._fn)
+        return self._fqfn.fqfn
 
     @property
     @lru_cache(maxsize=None)
     def defined_class(self):
-        return self.function_name[0]
+        return self._fqfn.fqclass
 
     @property
     @lru_cache(maxsize=None)
     def method_id(self):
-        return self.function_name[1]
+        return self._fqfn.fqfn[1]
 
     @property
     @lru_cache(maxsize=None)
     def function_location(self):
         return get_function_location(self._fn)
 
     @property
@@ -263,14 +305,15 @@
         if comment is None:
             comment = inspect.getcomments(self._fn)
         return comment
 
     def __init__(self, fn, fntype, parameters, labels):
         super().__init__("call")
         self._fn = fn
+        self._fqfn = FqFnName(fn)
         self.static = fntype in FnType.STATIC | FnType.CLASS | FnType.MODULE
         self.receiver = None
         if fntype in FnType.CLASS | FnType.INSTANCE:
             self.receiver = parameters[0]
             parameters = parameters[1:]
         self.parameters = parameters
         self.labels = labels
@@ -284,15 +327,15 @@
         ret.update(
             super().to_dict(attrs=["defined_class", "method_id", "path", "lineno"])
         )
 
         return ret
 
 
-class SqlEvent(Event):
+class SqlEvent(Event):  # pylint: disable=too-few-public-methods
     __slots__ = ["sql_query"]
 
     def __init__(self, sql, vendor=None, version=None):
         super().__init__("call")
         self.sql_query = compact_dict(
             {
                 "sql": sql,
@@ -300,23 +343,30 @@
                 "server_version": ".".join([str(v) for v in version])
                 if version
                 else None,
             }
         )
 
 
-class MessageEvent(Event):
+class MessageEvent(Event):  # pylint: disable=too-few-public-methods
     __slots__ = ["message"]
 
     def __init__(self, message_parameters):
         super().__init__("call")
         self.message = []
-        for name, value in message_parameters.items():
-            message_object = {"name": name}
-            message_object.update(describe_value(value))
+        self.message_parameters = message_parameters
+
+    @property
+    def message_parameters(self):
+        return self.message
+
+    @message_parameters.setter
+    def message_parameters(self, params):
+        for name, value in params.items():
+            message_object = describe_value(name, value)
             self.message.append(message_object)
 
 
 def none_if_empty(collection):
     """Return collection or None if it's empty."""
     return collection if len(collection) > 0 else None
 
@@ -342,19 +392,21 @@
                 }
             )
 
         self.http_client_request = compact_dict(request)
 
 
 # pylint: disable=too-few-public-methods
+_NORMALIZED_PATH_INFO_ATTR = "normalized_path_info"
 class HttpServerRequestEvent(MessageEvent):
     """A call AppMap event representing an HTTP server request."""
 
     __slots__ = ["http_server_request"]
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         request_method,
         path_info,
         message_parameters,
         normalized_path_info=None,
         protocol=None,
@@ -362,28 +414,36 @@
     ):
         super().__init__(message_parameters)
 
         request = {
             "request_method": request_method,
             "protocol": protocol,
             "path_info": path_info,
-            "normalized_path_info": normalized_path_info,
+            _NORMALIZED_PATH_INFO_ATTR: normalized_path_info,
         }
 
         if headers is not None:
             request.update(
                 {
                     "mime_type": headers.get("Content-Type"),
                     "authorization": headers.get("Authorization"),
                     "headers": none_if_empty(dict(headers)),
                 }
             )
 
         self.http_server_request = compact_dict(request)
 
+    @property
+    def normalized_path_info(self):
+        return self.http_server_request.get(_NORMALIZED_PATH_INFO_ATTR, None)
+
+    @normalized_path_info.setter
+    def normalized_path_info(self, npi):
+        self.http_server_request[_NORMALIZED_PATH_INFO_ATTR] = npi
+
 
 class ReturnEvent(Event):
     __slots__ = ["parent_id", "elapsed"]
 
     def __init__(self, parent_id, elapsed):
         super().__init__("return")
         self.parent_id = parent_id
@@ -391,15 +451,15 @@
 
 
 class FuncReturnEvent(ReturnEvent):
     __slots__ = ["return_value"]
 
     def __init__(self, parent_id, elapsed, return_value):
         super().__init__(parent_id, elapsed)
-        self.return_value = describe_value(return_value)
+        self.return_value = describe_value(None, return_value)
 
 
 class HttpResponseEvent(ReturnEvent):
     """A generic HTTP response event."""
 
     def __init__(self, status_code, headers=None, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `appmap-1.9.1/appmap/_implementation/generation.py` & `appmap-2.0.0/_appmap/generation.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,49 +6,49 @@
 
 
 # ClassMapDict needs to quack a little like a dict. If it's actually a
 # subclass of dict, though, json tries to process it without calling
 # our encoder. So, just implement the methods we need.
 class ClassMapDict:
     def __init__(self):
-        self._dict = dict()
+        self._dict = {}
 
     def setdefault(self, k, default):
         return self._dict.setdefault(k, default)
 
     def values(self):
         return self._dict.values()
 
 
-class ClassMapEntry:
+class ClassMapEntry:  # pylint: disable=too-few-public-methods
     # pylint: disable=redefined-builtin
     def __init__(self, name, type):
         self.name = name
         # `type` is a builtin, but the appmap attribute is named
         # `type`. So, ignore this warning, unless it turns out to
         # actually be a problem, of course.
         self.type = type
 
     def to_dict(self):
         return {k: v for k, v in vars(self).items() if v is not None}
 
 
-class PackageEntry(ClassMapEntry):
+class PackageEntry(ClassMapEntry):  # pylint: disable=too-few-public-methods
     def __init__(self, name):
         super().__init__(name, "package")
         self.children = ClassMapDict()
 
 
-class ClassEntry(ClassMapEntry):
+class ClassEntry(ClassMapEntry):  # pylint: disable=too-few-public-methods
     def __init__(self, name):
         super().__init__(name, "class")
         self.children = ClassMapDict()
 
 
-class FuncEntry(ClassMapEntry):
+class FuncEntry(ClassMapEntry):  # pylint: disable=too-few-public-methods
     def __init__(self, e):
         super().__init__(e.method_id, "function")
         self.location = "%s:%s" % (e.path, e.lineno)
         self.static = e.static
         self.labels = e.labels
         self.comment = e.comment
 
@@ -102,17 +102,17 @@
     }
 
 
 class AppMapEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, Event):
             return o.to_dict()
-        elif isinstance(o, ClassMapDict):
+        if isinstance(o, ClassMapDict):
             return list(o.values())
-        elif isinstance(o, ClassMapEntry):
+        if isinstance(o, ClassMapEntry):
             return o.to_dict()
 
         return json.JSONEncoder.default(self, o)
 
 
 def dump(recording, metadata=None, indent=None):
     a = appmap(recording, metadata)
```

### Comparing `appmap-1.9.1/appmap/_implementation/importer.py` & `appmap-2.0.0/_appmap/importer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,96 @@
 import functools
 import inspect
-import logging
 import sys
 import types
 from abc import ABC, abstractmethod
 from collections import namedtuple
 from collections.abc import MutableSequence
+from functools import reduce
 
-import appmap.wrapt as wrapt
+from _appmap import wrapt
 
 from .env import Env
-from .utils import FnType
+from .utils import FnType, Scope
 
-logger = logging.getLogger(__name__)
+logger = Env.current.getLogger(__name__)
 
 
-Filterable = namedtuple("Filterable", "fqname obj")
+Filterable = namedtuple("Filterable", "scope fqname obj")
 
 
 class FilterableMod(Filterable):
     __slots__ = ()
 
-    def __new__(c, mod):
+    def __new__(cls, mod):
         fqname = mod.__name__
-        return super(FilterableMod, c).__new__(c, fqname, mod)
-
-    def classify_fn(self, _):
-        return FnType.MODULE
+        return super(FilterableMod, cls).__new__(cls, Scope.MODULE, fqname, mod)
 
 
 class FilterableCls(Filterable):
     __slots__ = ()
 
-    def __new__(c, cls):
-        fqname = "%s.%s" % (cls.__module__, cls.__qualname__)
-        return super(FilterableCls, c).__new__(c, fqname, cls)
-
-    def classify_fn(self, static_fn):
-        return FnType.classify(static_fn)
+    def __new__(cls, clazz):
+        fqname = "%s.%s" % (clazz.__module__, clazz.__qualname__)
+        return super(FilterableCls, cls).__new__(cls, Scope.CLASS, fqname, clazz)
 
 
 class FilterableFn(
     namedtuple(
         "FilterableFn",
-        Filterable._fields
-        + (
-            "scope",
-            "static_fn",
-        ),
+        Filterable._fields + ("static_fn",),
     )
 ):
     __slots__ = ()
 
-    def __new__(c, scope, fn, static_fn):
+    def __new__(cls, scope, fn, static_fn):
         fqname = "%s.%s" % (scope.fqname, fn.__name__)
-        self = super(FilterableFn, c).__new__(c, fqname, fn, scope, static_fn)
+        self = super(FilterableFn, cls).__new__(cls, scope.scope, fqname, fn, static_fn)
         return self
 
     @property
     def fntype(self):
-        return self.scope.classify_fn(self.static_fn)
+        if self.scope == Scope.MODULE:
+            return FnType.MODULE
+
+        return FnType.classify(self.static_fn)
 
 
-class Filter(ABC):
+class Filter(ABC):  # pylint: disable=too-few-public-methods
     def __init__(self, next_filter):
         self.next_filter = next_filter
 
     @abstractmethod
     def filter(self, filterable):
         """
         Determine whether the given class should have its methods
         instrumented.  Return True if it should be, False if it should
         not be, or call the next filter if this filter can't decide.
         """
 
-    @abstractmethod
-    def wrap(self, filterable):
-        """
-        Determine whether the given filterable function should be
-        instrumented.  If so, return a new function that wraps the
-        old.  If not, return the original function.
-        """
-
 
-class NullFilter(Filter):
+class NullFilter(Filter):  # pylint: disable=too-few-public-methods
     def __init__(self, next_filter=None):
         super().__init__(next_filter)
 
     def filter(self, filterable):
         return False
 
-    def wrap(self, filterable):
-        return filterable.obj
-
 
 def is_class(c):
     # We don't want to use inspect.isclass here. It uses isinstance to
     # check the class of the object, which will invoke any method
     # bound to __class__. (For example, celery.local.Proxy uses this
     # mechanism to return the class of the proxied object.)
     #
-    return inspect._is_type(c)  # pylint: disable=protected-access
+    try:
+        inspect._static_getmro(c)  # pylint: disable=protected-access
+    except TypeError:
+        return False
+    return True
 
 
 def get_classes(module):
     return [v for __, v in module.__dict__.items() if is_class(v)]
 
 
 def get_members(cls):
@@ -117,17 +103,15 @@
       * key is the attribute name
       * dict_value is cls.__dict__[key]
       * and attr_value is getattr(cls, key)
     """
 
     def is_member_func(m):
         t = type(m)
-        if (
-            t == types.BuiltinFunctionType or t == types.BuiltinMethodType  # noqa: E721
-        ):  # noqa: E129
+        if t in (types.BuiltinFunctionType, types.BuiltinMethodType):
             return False
 
         return (
             t == types.FunctionType  # noqa: E721
             or t == types.MethodType
             or FnType.classify(m) in FnType.STATIC | FnType.CLASS
         )
@@ -151,85 +135,107 @@
             continue
         ret.append((key, static_value, value))
     return ret
 
 
 class Importer:
     filter_stack = [NullFilter]
-    filter_chain = []
+    filter_chain = None
 
     def get_filter_stack(self):
         return self.filter_stack
 
     @classmethod
     def initialize(cls):
-        cls.filter_stack = [NullFilter]
+        cls.filter_stack = []
         cls.filter_chain = []
+        cls._skip_instrumenting = ("appmap", "_appmap")
 
     @classmethod
     def use_filter(cls, filter_class):
         cls.filter_stack.append(filter_class)
 
     @classmethod
+    def instrument_function(cls, fn_name, filterableFn: FilterableFn, selected_functions=None):
+        # Only instrument the function if it was specifically called out for the package
+        # (e.g. because it should be labeled), or it's included by the filters
+        matched = cls.filter_chain.filter(filterableFn)
+        selected = selected_functions and fn_name in selected_functions
+        if selected or matched:
+            return cls.filter_chain.wrap(filterableFn)
+
+        return filterableFn.obj
+
+    @classmethod
     def do_import(cls, *args, **kwargs):
         mod = args[0]
-        if mod.__name__.startswith("appmap"):
+        if mod.__name__.startswith(cls._skip_instrumenting):
             return
 
-        logger.debug("do_import, mod %s args %s kwargs %s", mod, args, kwargs)
+        logger.trace("do_import, mod %s args %s kwargs %s", mod, args, kwargs)
         if not cls.filter_chain:
-            logger.debug("  filter_stack %s", cls.filter_stack)
-            cls.filter_chain = cls.filter_stack[0](None)
-            for filter_ in cls.filter_stack[1:]:
-                cls.filter_chain = filter_(cls.filter_chain)
-                logger.debug("  self.filter chain: %s", cls.filter_chain)
-
-        def instrument_functions(filterable):
-            if not cls.filter_chain.filter(filterable):
-                return
+            cls.filter_chain = reduce(lambda acc, e: e(acc), cls.filter_stack, NullFilter(None))
 
-            logger.info("  looking for members of %s", filterable.obj)
+        def instrument_functions(filterable, selected_functions=None):
+            logger.trace("  looking for members of %s", filterable.obj)
             functions = get_members(filterable.obj)
-            logger.debug("  functions %s", functions)
+            logger.trace("  functions %s", functions)
 
             for fn_name, static_fn, fn in functions:
-                new_fn = cls.filter_chain.wrap(FilterableFn(filterable, fn, static_fn))
-                if fn != new_fn:
+                filterableFn = FilterableFn(filterable, fn, static_fn)
+                new_fn = cls.instrument_function(fn_name, filterableFn, selected_functions)
+                if new_fn != fn:
                     wrapt.wrap_function_wrapper(filterable.obj, fn_name, new_fn)
 
-        instrument_functions(FilterableMod(mod))
+        # Import Config here, to avoid circular top-level imports.
+        from .configuration import Config  # pylint: disable=import-outside-toplevel
+
+        package_functions = Config.current.package_functions
+        fm = FilterableMod(mod)
+        if fm.fqname in package_functions:
+            instrument_functions(fm, package_functions.get(fm.fqname))
+        elif cls.filter_chain.filter(fm):
+            instrument_functions(fm)
+
         classes = get_classes(mod)
-        logger.debug("  classes %s", classes)
+        logger.trace("  classes %s", classes)
         for c in classes:
-            instrument_functions(FilterableCls(c))
+            fc = FilterableCls(c)
+            if fc.fqname.startswith(cls._skip_instrumenting):
+                logger.trace("  not instrumenting %s", fc.fqname)
+                continue
+            if fc.fqname in package_functions:
+                instrument_functions(fc, package_functions.get(fc.fqname))
+            elif cls.filter_chain.filter(fc):
+                instrument_functions(fc)
 
 
 def wrap_finder_function(fn, decorator):
     ret = fn
     fn_name = fn.func.__name__ if isinstance(fn, functools.partial) else fn.__name__
     marker = "_appmap_wrapped_%s" % fn_name
 
     # Figure out which object should get the marker attribute. If fn
     # is a bound function, put it on the object it's bound to,
     # otherwise put it on the function itself.
     obj = fn.__self__ if hasattr(fn, "__self__") else fn
 
     if getattr(obj, marker, None) is None:
-        logger.debug("wrapping %r", fn)
+        logger.trace("wrapping %r", fn)
         ret = decorator(fn)
         setattr(obj, marker, True)
     else:
-        logger.debug("already wrapped, %r", fn)
+        logger.trace("already wrapped, %r", fn)
 
     return ret
 
 
 @wrapt.decorator
 def wrapped_exec_module(exec_module, _, args, kwargs):
-    logger.debug("exec_module %r args %s kwargs %s", exec_module, args, kwargs)
+    logger.trace("exec_module %r args %s kwargs %s", exec_module, args, kwargs)
     exec_module(*args, **kwargs)
     # Only process imports if we're currently enabled. This
     # handles the case where we previously hooked the finders, but
     # were subsequently disabled (e.g. during testing).
     if Env.current.enabled:
         Importer.do_import(*args, **kwargs)
 
@@ -244,34 +250,48 @@
     if spec is not None:
         if getattr(spec.loader, "exec_module", None) is not None:
             loader = spec.loader
             # This is kind of gross. As the comment linked to below describes, wrapt has trouble
             # identifying methods decorated with @staticmethod. It offers two suggested fixes:
             # update the class definition, or patch the function found in __dict__. We can't do the
             # former, so do the latter instead.
-            #   https://github.com/GrahamDumpleton/wrapt/blob/68316bea668fd905a4acb21f37f12596d8c30d80/src/wrapt/wrappers.py#L691
+            #   https://github.com/GrahamDumpleton/wrapt/blob/1.14.1/src/wrapt/wrappers.py#L730
             #
             # TODO: determine if we can use wrapt.wrap_function_wrapper to simplify this code
             exec_module = inspect.getattr_static(loader, "exec_module")
             if isinstance(exec_module, staticmethod):
                 loader.exec_module = wrap_exec_module(exec_module)
             else:
                 loader.exec_module = wrap_exec_module(loader.exec_module)
         else:
-            logger.debug("no exec_module for loader %r", spec.loader)
+            logger.trace("no exec_module for loader %r", spec.loader)
     return spec
 
 
 def wrap_finder_find_spec(finder):
-    find_spec = getattr(finder, "find_spec", None)
-    if find_spec is None:
-        logger.debug("no find_spec for finder %r", finder)
-        return
+    # Prior to 3.11, it worked fine to just grab find_spec from the finder and wrap it. The
+    # implementation of builtin finders must have changed with 3.11, because we now need the same
+    # kind of workaround we use above for exec_module.
+    if sys.version_info[1] < 11:
+        find_spec = getattr(finder, "find_spec", None)
+        if find_spec is None:
+            logger.trace("no find_spec for finder %r", finder)
+            return
 
-    finder.find_spec = wrap_finder_function(find_spec, wrapped_find_spec)
+        finder.find_spec = wrap_finder_function(find_spec, wrapped_find_spec)
+    else:
+        find_spec = inspect.getattr_static(finder, "find_spec", None)
+        if find_spec is None:
+            logger.trace("no find_spec for finder %r", finder)
+            return
+
+        if isinstance(find_spec, (classmethod, staticmethod)):
+            finder.find_spec = wrap_finder_function(find_spec, wrapped_find_spec)
+        else:
+            finder.find_spec = wrap_finder_function(finder.find_spec, wrapped_find_spec)
 
 
 class MetapathObserver(MutableSequence):
     def __init__(self, meta_path):
         self._meta_path = meta_path
 
     def __getitem__(self, key):
@@ -294,15 +314,15 @@
         return self._meta_path.copy()
 
 
 def initialize():
     Importer.initialize()
     # If we're not enabled, there's no reason to hook the finders.
     if Env.current.enabled:
-        logger.debug("sys.metapath: %s", sys.meta_path)
+        logger.trace("sys.metapath: %s", sys.meta_path)
         for finder in sys.meta_path:
             wrap_finder_find_spec(finder)
 
         # Make sure we instrument any finders that get added in the
         # future.
         sys.meta_path = MetapathObserver(sys.meta_path.copy())
```

### Comparing `appmap-1.9.1/appmap/_implementation/instrument.py` & `appmap-2.0.0/_appmap/instrument.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import logging
 import sys
 import time
 from collections import namedtuple
 from contextlib import contextmanager
 
 from . import event
+from .env import Env
 from .event import CallEvent
 from .recorder import Recorder
 from .utils import appmap_tls
 
-logger = logging.getLogger(__name__)
+logger = Env.current.getLogger(__name__)
 
 
 @contextmanager
 def recording_disabled():
     tls = appmap_tls()
     tls["instrumentation_disabled"] = True
     try:
@@ -44,15 +44,15 @@
     while ignoring their internals, it's an effective way of limiting
     appmap size.  If you want anything more complicated and can take
     the performance hit, your best bet is to record without shallow
     and postprocess the appmap to your liking.
     """
     tls = appmap_tls()
     rule = getattr(fn, "_appmap_shallow", None)
-    logger.debug("track_shallow(%r) [%r]", fn, rule)
+    logger.trace("track_shallow(%r) [%r]", fn, rule)
     result = rule and tls.get("last_rule", None) == rule
     tls["last_rule"] = rule
     return result
 
 
 @contextmanager
 def saved_shallow_rule():
@@ -78,15 +78,15 @@
         (not Recorder.get_enabled())
         or is_instrumentation_disabled()
         or track_shallow(f.instrumented_fn)
     ):
         return f.fn(*args, **kwargs)
 
     with recording_disabled():
-        logger.debug("%s args %s kwargs %s", f.fn, args, kwargs)
+        logger.trace("%s args %s kwargs %s", f.fn, args, kwargs)
         params = CallEvent.set_params(f.params, instance, args, kwargs)
         call_event = f.make_call_event(parameters=params)
     Recorder.add_event(call_event)
     call_event_id = call_event.id
     start_time = time.time()
     try:
         ret = f.fn(*args, **kwargs)
@@ -105,15 +105,15 @@
             )
         )
         raise
 
 
 def instrument(filterable):
     """return an instrumented function"""
-    logger.info("hooking %s", filterable.fqname)
+    logger.debug("hooking %s", filterable.fqname)
     fn = filterable.obj
 
     make_call_event = event.CallEvent.make(fn, filterable.fntype)
     params = CallEvent.make_params(filterable)
 
     # django depends on being able to find the cache_clear attribute
     # on functions. (You can see this by trying to map
```

### Comparing `appmap-1.9.1/appmap/_implementation/labels.py` & `appmap-2.0.0/_appmap/labels.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from collections import defaultdict
 from typing import Dict, List, Optional, Union
 
+from .env import Env
 from .importer import Filterable
 
+logger = Env.current.getLogger(__name__)
 
-class labels:
+
+class labels:  # pylint: disable=too-few-public-methods
     def __init__(self, *args):
         self._labels = args
 
     def __call__(self, fn):
         # For simplicity, set _appmap_labels right on the
         # function. We'll delete it when we instrument the function.
         setattr(fn, "_appmap_labels", self._labels)
@@ -19,19 +22,16 @@
 FunctionName = str  # fully qualified
 Config = Dict[Label, Union[FunctionName, List[FunctionName]]]
 
 
 class LabelSet:
     """A set of labels defined to be applied on specific functions."""
 
-    def __init__(self, config: Optional[Config] = None):
-        """Create the LabelSet, optionally pre-populating it with the provided config."""
+    def __init__(self):
         self.labels = defaultdict(list)
-        if config:
-            self.append(config)
 
     def append(self, config: Config):
         """Update this LabelSet to contain definitions from the config."""
         for label, functions in config.items():
             if isinstance(functions, str):
                 functions = (functions,)
             for function in functions:
@@ -46,11 +46,11 @@
         labels(*applicable)(function.obj)
         return applicable
 
     def __repr__(self):
         if not self.labels:
             return "LabelSet()"
         inverted = defaultdict(list)
-        for function, labels in self.labels.items():
-            for label in labels:
+        for function, lbls in self.labels.items():
+            for label in lbls:
                 inverted[label].append(function)
         return "LabelSet(%s)" % dict(inverted)
```

### Comparing `appmap-1.9.1/appmap/_implementation/py_version_check.py` & `appmap-2.0.0/_appmap/py_version_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 
 
 def _get_platform_version():
     return platform.python_version()
 
 
 def check_py_version():
-    req = (3, 6)
+    req = (3, 8)
     actual = _get_platform_version()
     if _get_py_version() < req:
         raise AppMapPyVerException(
             f"Minimum Python version supported is {req[0]}.{req[1]}, found {actual}"
         )
```

### Comparing `appmap-1.9.1/appmap/_implementation/recorder.py` & `appmap-2.0.0/_appmap/recorder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import logging
 import threading
 import traceback
 from abc import ABC, abstractmethod
 
-from appmap._implementation.utils import appmap_tls
+from .env import Env
+from .utils import appmap_tls
 
-logger = logging.getLogger(__name__)
+logger = Env.current.getLogger(__name__)
 
+# pylint: disable=global-statement
 _default_recorder = None
 
 
 class Recorder(ABC):
     """
     A base class for Recorders.
 
@@ -18,18 +19,22 @@
     """
 
     @property
     @abstractmethod
     def events(self):
         return self._events
 
-    @abstractmethod
-    def next_event_id(self):
-        self._next_event_id += 1
-        return self._next_event_id
+    _next_event_id = 0
+    _next_event_id_lock = threading.Lock()
+
+    @classmethod
+    def next_event_id(cls):
+        with cls._next_event_id_lock:
+            cls._next_event_id += 1
+            return cls._next_event_id
 
     # It might be nice to put @property on the getters here. The python maintainers have gone back
     # and forth on whether you should be able to combine @classmethod and @property. In 3.11,
     # they've decided you can't: https://docs.python.org/3.11/library/functions.html#classmethod.
     @classmethod
     def get_current(cls):
         """
@@ -40,69 +45,82 @@
         return perthread if perthread else shared
 
     @classmethod
     def set_current(cls, r):
         """
         Set the recorder for the current thread.
         """
-        appmap_tls()[cls._RECORDER_KEY] = r
+        tls = appmap_tls()
+        if r:
+            tls[cls._RECORDER_KEY] = r
+        else:
+            del tls[cls._RECORDER_KEY]
+
         return r
 
     @classmethod
+    def get_global(cls):
+        _, shared = cls._get_current()
+        return shared
+
+    @classmethod
+    def new_global(cls):
+        global _default_recorder
+        _default_recorder = SharedRecorder()
+        return _default_recorder
+
+    @classmethod
     def get_enabled(cls):
-        return cls.get_current()._enabled
+        return cls.get_current()._enabled  # pylint: disable=protected-access
 
     @classmethod
     def set_enabled(cls, e):
-        cls.get_current()._enabled = e
+        cls.get_current()._enabled = e  # pylint: disable=protected-access
 
     @classmethod
     def start_recording(cls):
-        cls.get_current()._start_recording()
+        cls.get_current()._start_recording()  # pylint: disable=protected-access
 
     @classmethod
     def stop_recording(cls):
-        return cls.get_current()._stop_recording()
+        return cls.get_current()._stop_recording()  # pylint: disable=protected-access
 
     @classmethod
     def add_event(cls, event):
         """
         Add the given event to the global recorder, as well as the thread's recorder (if it has
         one).
         """
         perthread, shared = cls._get_current()
-        shared._add_event(event)
+        shared._add_event(event)  # pylint: disable=protected-access
         if perthread:
-            perthread._add_event(event)
+            perthread._add_event(event)  # pylint: disable=protected-access
 
     _RECORDER_KEY = "appmap_recorder"
 
     @classmethod
     def _get_current(cls):
-        global _default_recorder
         perthread = appmap_tls().get(cls._RECORDER_KEY, None)
 
         return [perthread, _default_recorder]
 
     def clear(self):
         self._events = []
-        self._next_event_id = 0
 
     def __init__(self, enabled=False):
         self._events = []
         self._enabled = enabled
         self.start_tb = None
-        self._next_event_id = 0
 
     @abstractmethod
     def _start_recording(self):
         logger.debug("AppMap recording started")
         if self._enabled:
-            logger.error("Recording already in progress, previous start:")
-            logger.error("".join(traceback.format_list(self.start_tb)))
+            logger.debug("Recording already in progress, previous start:")
+            logger.debug("".join(traceback.format_list(self.start_tb)))
             raise RuntimeError("Recording already in progress")
         self.start_tb = traceback.extract_stack()
         self._enabled = True
 
     @abstractmethod
     def _stop_recording(self):
         logger.debug("AppMap recording stopped")
@@ -118,64 +136,68 @@
     def _initialize():
         """Create a new default, shared recorder.
 
         This method is intentionally not thread-safe. It really doesn't make sense have multiple
         threads initializing the default recorder. If you find yourself wanting to do that, you
         should probably be using per-thread recording.
         """
-        global _default_recorder
-        _default_recorder = SharedRecorder()
+        Recorder.new_global()
 
 
 class ThreadRecorder(Recorder):
     """
     A Recorder to use for a thread. Not thread-safe, of course.
     """
 
     @property
     def events(self):
         return super().events
 
-    def next_event_id(self):
-        return super().next_event_id()
-
+    # They're not useless, because they're abtract with a default implementation
+    # pragma pylint: disable=useless-super-delegation
     def _start_recording(self):
         super()._start_recording()
 
     def _stop_recording(self):
         return super()._stop_recording()
 
     def _add_event(self, event):
         super()._add_event(event)
 
+    # pragma pylint: enable=useless-super-delegation
+
 
 class SharedRecorder(Recorder):
     """
     A shared Recorder. The global recorder is an instance of this class.
     """
 
     _lock = threading.Lock()
 
+    def __init__(self):
+        super().__init__()
+        Recorder._next_event_id = 0
+
+    def clear(self):
+        super().clear()
+        Recorder._next_event_id = 0
+
     @property
     def events(self):
         with self._lock:
             return super().events
 
     def _start_recording(self):
         with self._lock:
             super()._start_recording()
 
     def _stop_recording(self):
         with self._lock:
             return super()._stop_recording()
 
-    def next_event_id(self):
-        with self._lock:
-            return super().next_event_id()
-
     def _add_event(self, event):
         with self._lock:
             super()._add_event(event)
 
 
 def initialize():
-    Recorder._initialize()
+    Recorder._initialize()  # pylint: disable=protected-access
```

### Comparing `appmap-1.9.1/appmap/_implementation/utils.py` & `appmap-2.0.0/_appmap/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import inspect
 import os
 import re
 import shlex
 import subprocess
-import threading
 import types
-from collections.abc import MutableMapping
-from enum import IntFlag, auto
+from contextlib import contextmanager
+from contextvars import ContextVar
+from enum import Enum, IntFlag, auto
+from pathlib import Path
+from typing import Any, Callable
 
 from .env import Env
 
 
+class Scope(Enum):
+    MODULE = 0
+    CLASS = 1
+
+
 def compact_dict(dictionary):
     """Return a copy of dictionary with None values filtered out."""
     return {k: v for k, v in dictionary.items() if v is not None}
 
 
 def values_dict(items):
     """Given a list of (key, list) values returns a dictionary where
@@ -28,68 +35,84 @@
     CLASS = auto()
     INSTANCE = auto()
     MODULE = auto()
 
     @staticmethod
     def classify(fn):
         fn_type = type(fn)
-        if fn_type == staticmethod or fn_type == types.BuiltinMethodType:
+        if fn_type in (staticmethod, types.BuiltinMethodType):
             return FnType.STATIC
-        elif fn_type == classmethod or fn_type == types.BuiltinMethodType:
+        if fn_type in (classmethod, types.BuiltinMethodType):
             return FnType.CLASS
-        else:
-            return FnType.INSTANCE
 
+        return FnType.INSTANCE
 
-class ThreadLocalDict(threading.local, MutableMapping):
-    def __init__(self):
-        super().__init__()
-        self.values = {}
 
-    def __getitem__(self, k):
-        return self.values[k]
+_appmap_tls = ContextVar("tls")
 
-    def __setitem__(self, k, v):
-        self.values[k] = v
 
-    def __delitem__(self, k):
-        del self.values[k]
+def appmap_tls():
+    try:
+        return _appmap_tls.get()
+    except LookupError:
+        _appmap_tls.set({})
+        return _appmap_tls.get()
 
-    def __iter__(self):
-        return iter(self.values)
 
-    def __len__(self):
-        return len(self.values)
+@contextmanager
+def appmap_tls_context():
+    token = _appmap_tls.set({})
+    try:
+        yield
+    finally:
+        _appmap_tls.reset(token)
 
 
-_appmap_tls = ThreadLocalDict()
+def fqname(cls):
+    return "%s.%s" % (cls.__module__, cls.__qualname__)
 
+class FqFnName:
+    """
+    FqFnName makes it easy to reference the parts of the fully-qualified name of a callable.
+    """
 
-def appmap_tls():
-    return _appmap_tls
+    def __init__(self, fn: Callable[..., Any]):
 
+        self._modname = fn.__module__
+        qualname = fn.__qualname__
+        if "." in qualname:
+            self._scope = Scope.CLASS
+            self._class_name, self._fn_name = qualname.rsplit(".", 1)
+        else:
+            self._scope = Scope.MODULE
+            self._class_name = None
+            self._fn_name = qualname
 
-def fqname(cls):
-    return "%s.%s" % (cls.__module__, cls.__qualname__)
+    @property
+    def scope(self) -> Scope:
+        """The scope of the Callable, i.e. whether it's contained in a module or a class."""
+        return self._scope
 
+    @property
+    def fqmod(self):
+        return self._modname
 
-def split_function_name(fn):
-    """
-    Given a method, return a tuple containing its fully-qualified
-    class name and the method name.
-    """
-    qualname = fn.__qualname__
-    if "." in qualname:
-        class_name, fn_name = qualname.rsplit(".", 1)
-        class_name = "%s.%s" % (fn.__module__, class_name)
-    else:
-        class_name = fn.__module__
-        fn_name = qualname
-    return (class_name, fn_name)
+    @property
+    def fqclass(self):
+        return self._modname if self._class_name is None else f"{self._modname}.{self._class_name}"
+
+    @property
+    def fqfn(self):
+        return (self.fqclass, self._fn_name)
+
+    @property
+    def fn_name(self):
+        return self._fn_name
 
+FqFnName(fqname)
 
 def root_relative_path(path):
     """Returns the path relative to the current root_dir.
 
     The path should be absolute.
     If it's not under the current root_dir, it's returned unchanged.
     """
@@ -196,7 +219,36 @@
 
 
 # this is different than appmap-ruby: part of its logic is in write_appmap
 def scenario_filename(name, separator="_"):
     pattern = r"[^a-z0-9\-_]+"
     replacement = separator
     return re.sub(pattern, replacement, name, flags=re.IGNORECASE)
+
+
+def locate_file_up(filename, start_dir=None, stop_dir=None):
+    """
+    Search for a file in the current directory and recursively up to the root directory.
+
+    :param filename: The name of the file to locate.
+    :param start_dir: The directory to start the search from. Defaults to the current.
+    :param stop_dir: The directory to stop the search. If None search is performed until
+                     the root of the file system.
+    :return: The path to the directory containing the file or None if the file cannot be found.
+    """
+
+    if start_dir is None:
+        start_dir = Path.cwd()
+    elif isinstance(start_dir, str):
+        start_dir = Path(start_dir)
+
+    file_path = start_dir.joinpath(filename)
+    if Path.exists(file_path):
+        return start_dir
+
+    for p in start_dir.parents:
+        if Path.exists(p.joinpath(filename)):
+            return p
+        if p == stop_dir:
+            return None
+
+    return None
```

### Comparing `appmap-1.9.1/appmap/_implementation/web_framework.py` & `appmap-2.0.0/_appmap/web_framework.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 """Common utilities for web framework integration"""
 
 import datetime
 import os
 import os.path
 import re
+import sys
+import textwrap
 import time
 from abc import ABC, abstractmethod
+from contextvars import ContextVar
 from hashlib import sha256
-from tempfile import NamedTemporaryFile
+from json.decoder import JSONDecodeError
+from typing import Any, Optional, Protocol, Tuple
 
-from appmap._implementation import generation
-from appmap._implementation.env import Env
-from appmap._implementation.event import Event, ReturnEvent, _EventIds, describe_value
-from appmap._implementation.recorder import Recorder, ThreadRecorder
-from appmap._implementation.utils import root_relative_path, scenario_filename
+from _appmap import recording
 
+from . import remote_recording
+from .env import Env
+from .event import (
+    Event,
+    ExceptionEvent,
+    HttpServerResponseEvent,
+    ReturnEvent,
+    describe_value,
+)
+from .recorder import Recorder, ThreadRecorder
+from .utils import root_relative_path, scenario_filename
+
+logger = Env.current.getLogger(__name__)
+request_recorder: ContextVar[Optional[Recorder]] = ContextVar("appmap_request_recorder")
+
+# These are the errors that can get raised when trying to update params based on the results of
+# parsing the body of an application/json request:
+JSON_ERRORS = (JSONDecodeError, AttributeError, TypeError, ValueError)
+
+REQUEST_ENABLED_ATTR = "_appmap_request_enabled"
+REMOTE_ENABLED_ATTR = "_appmap_remote_enabled"
 
 class TemplateEvent(Event):  # pylint: disable=too-few-public-methods
     """A special call event that records template rendering."""
 
     __slots__ = ["receiver", "path"]
 
     def __init__(self, path, instance=None):
         super().__init__("call")
-        self.receiver = describe_value(instance)
+        self.receiver = describe_value(None, instance)
         self.path = root_relative_path(path)
 
     def to_dict(self, attrs=None):
         result = super().to_dict(attrs)
         classlike_name = re.sub(r"\W", "", self.path.title())
         result.update(
             {
@@ -35,33 +56,38 @@
                 "method_id": "render",
                 "static": False,
             }
         )
         return result
 
 
-class TemplateHandler:  # pylint: disable=too-few-public-methods
+class HasFilename(Protocol):  # pylint: disable=too-few-public-methods
+    filename: str
+
+
+class TemplateHandler(HasFilename):  # pylint: disable=too-few-public-methods
     """Patch for a template class to capture and record template
     rendering (if recording is enabled).
 
     This patch can be used with .utils.patch_class to patch any template class
     which has a .render() method. Note it requires a .filename property; if
     there is no such property, this handler can be subclassed first to provide it.
     """
 
     def render(self, orig, *args, **kwargs):
         """Calls the original implementation.
 
         If recording is enabled, adds appropriate TemplateEvent
         and ReturnEvent.
         """
+
         rec = Recorder.get_current()
         if rec.get_enabled():
             start = time.monotonic()
-            call_event = TemplateEvent(self.filename, self)  # pylint: disable=no-member
+            call_event = TemplateEvent(self.filename, self)
             Recorder.add_event(call_event)
         try:
             return orig(self, *args, **kwargs)
         finally:
             if rec.get_enabled():
                 Recorder.add_event(ReturnEvent(call_event.id, time.monotonic() - start))
 
@@ -72,151 +98,178 @@
 
 
 def name_hash(namepart):
     """Returns the hex digits of the sha256 of the os.fsencode()d namepart."""
     return sha256(os.fsencode(namepart)).hexdigest()
 
 
-def write_appmap(basedir, basename, contents):
-    """Write an appmap file into basedir.
-
-    Adds APPMAP_SUFFIX to basename; shortens the name if necessary.
-    Atomically replaces existing files. Creates the basedir if required.
-    """
-
-    if len(basename) > NAME_MAX - len(APPMAP_SUFFIX):
-        part = NAME_MAX - len(APPMAP_SUFFIX) - 1 - HASH_LEN
-        basename = basename[:part] + "-" + name_hash(basename[part:])[:HASH_LEN]
-    filename = basename + APPMAP_SUFFIX
-
-    if not basedir.exists():
-        basedir.mkdir(parents=True, exist_ok=True)
-
-    with NamedTemporaryFile(mode="w", dir=basedir, delete=False) as tmp:
-        tmp.write(contents)
-    os.replace(tmp.name, basedir / filename)
-
-
+# pylint: disable=too-many-arguments
 def create_appmap_file(
     output_dir,
     request_method,
     request_path_info,
     request_full_path,
-    response,
+    status,
     headers,
     rec,
 ):
     start_time = datetime.datetime.now()
     appmap_name = (
         request_method
         + " "
         + request_path_info
         + " ("
-        + str(response.status_code)
+        + str(status)
         + ") - "
         + start_time.strftime("%T.%f")[:-3]
     )
-    appmap_basename = scenario_filename(
-        "_".join([str(start_time.timestamp()), request_full_path])
-    )
+    appmap_basename = scenario_filename("_".join([str(start_time.timestamp()), request_full_path]))
     appmap_file_path = os.path.join(output_dir, appmap_basename)
+
+    recorder_type = "requests"
     metadata = {
         "name": appmap_name,
         "timestamp": start_time.timestamp(),
-        "recorder": {"name": "record_requests"},
+        "recorder": {"name": "record_requests", "type": recorder_type},
     }
-    write_appmap(output_dir, appmap_basename, generation.dump(rec, metadata))
+    recording.write_appmap(rec, appmap_basename, recorder_type, metadata)
     headers["AppMap-Name"] = os.path.abspath(appmap_name)
     headers["AppMap-File-Name"] = os.path.abspath(appmap_file_path) + APPMAP_SUFFIX
 
 
 class AppmapMiddleware(ABC):
-    def before_request_hook(
-        self, request, request_path, record_url, recording_is_running
-    ):
-        if request_path == record_url:
-            return None, None, None
-
-        start = None
-        call_event_id = None
-        if Env.current.enabled or recording_is_running:
-            # It should be recording or it's currently recording.  The
-            # recording is either
-            # a) remote, enabled by POST to /_appmap/record, which set
-            #    recording_is_running, or
-            # b) requests, set by Env.current.record_all_requests, or
-            # c) both remote and requests; there are multiple active recorders.
-            if not Env.current.record_all_requests and recording_is_running:
-                # a)
-                rec = Recorder.get_current()
-            else:
-                # b) or c)
-                rec = ThreadRecorder()
-                Recorder.set_current(rec)
-                rec.start_recording()
+    @abstractmethod
+    def before_request_main(self, rec, req: Any) -> Tuple[float, int]:
+        """Specify the main operations to be performed by a request is processed."""
+        raise NotImplementedError
+
+    # pylint: disable=too-many-arguments
+    def after_request_main(self, rec, status, headers, start, call_event_id) -> None:
+
+        duration = time.monotonic() - start
+        return_event = HttpServerResponseEvent(
+            parent_id=call_event_id,
+            elapsed=duration,
+            status_code=status,
+            headers=headers,
+        )
+        rec.add_event(return_event)
 
-            if rec.get_enabled():
-                start, call_event_id = self.before_request_main(rec, request)
+    def __init__(self, framework_name):
+        self.record_url = "/_appmap/record"
+        env = Env.current
+        record_requests = env.enables("requests")
+        if record_requests:
+            logger.info("Requests will be recorded (%s)", framework_name)
+
+        self.should_record = env.enables("remote") or record_requests
+
+    def before_request_hook(self, request) -> Tuple[Optional[Recorder], float, int]:
+        rec = None
+        start = 0
+        call_event_id = 0
+        env = Env.current
+        if env.enables("requests"):
+            rec = ThreadRecorder()
+            Recorder.set_current(rec)
+            rec.start_recording()
+            request_recorder.set(rec)
+        elif env.enables("remote"):
+            rec = Recorder.get_global()
 
-        return rec, start, call_event_id
+        if rec and rec.get_enabled():
+            start, call_event_id = self.before_request_main(rec, request)
 
-    @abstractmethod
-    def before_request_main(self, rec):
-        pass
+        return rec, start, call_event_id
 
+    # pylint: disable=too-many-arguments
     def after_request_hook(
         self,
-        request,
         request_path,
-        record_url,
-        recording_is_running,
         request_method,
         request_base_url,
-        response,
-        response_headers,
+        status,
+        headers,
         start,
         call_event_id,
-    ):
-        if request_path == record_url:
-            return response
-
-        if Env.current.enabled or recording_is_running:
-            # It should be recording or it's currently recording.  The
-            # recording is either
-            # a) remote, enabled by POST to /_appmap/record, which set
-            #    self.recording.is_running, or
-            # b) requests, set by Env.current.record_all_requests, or
-            # c) both remote and requests; there are multiple active recorders.
-            if not Env.current.record_all_requests and recording_is_running:
-                # a)
-                rec = Recorder.get_current()
-                if rec.get_enabled():
-                    self.after_request_main(rec, response, start, call_event_id)
-            else:
-                # b) or c)
-                rec = Recorder.get_current()
-                # Each time an event is added for a thread_id it's also
-                # added to the global Recorder().  So don't add the event
-                # to the global Recorder() explicitly because that would
-                # add the event in it twice.
-                try:
-                    if rec.get_enabled():
-                        self.after_request_main(rec, response, start, call_event_id)
-
-                    output_dir = Env.current.output_dir / "requests"
-                    create_appmap_file(
-                        output_dir,
-                        request_method,
-                        request_path,
-                        request_base_url,
-                        response,
-                        response_headers,
-                        rec,
-                    )
-                finally:
-                    rec.stop_recording()
+    ) -> None:
+        if request_path == self.record_url:
+            return
+
+        env = Env.current
+        if env.enables("requests"):
+            rec = request_recorder.get()
+            assert rec is not None
+
+            try:
+                self.after_request_main(rec, status, headers, start, call_event_id)
+
+                output_dir = Env.current.output_dir / "requests"
+                create_appmap_file(
+                    output_dir,
+                    request_method,
+                    request_path,
+                    request_base_url,
+                    status,
+                    headers,
+                    rec,
+                )
+            finally:
+                rec.stop_recording()
+                Recorder.set_current(None)
+                request_recorder.set(None)
+        elif env.enables("remote"):
+            rec = Recorder.get_global()
+            assert rec is not None
+            if rec.get_enabled():
+                self.after_request_main(rec, status, headers, start, call_event_id)
+
+    def on_exception(self, rec, start, call_event_id, exc_info):
+        duration = time.monotonic() - start
+        exception_event = ExceptionEvent(
+            parent_id=call_event_id,
+            elapsed=duration,
+            exc_info=exc_info,
+        )
+        rec.add_event(exception_event)
+
+
+class MiddlewareInserter(ABC):
+    def __init__(self, debug):
+        self.debug = debug
 
-        return response
+    @abstractmethod
+    def middleware_present(self):
+        """Return True if the AppMap middleware is present, False otherwise."""
+
+    @abstractmethod
+    def insert_middleware(self):
+        """Insert the AppMap middleware. Optionally return a new instance of the app."""
 
     @abstractmethod
-    def after_request_main(self, rec, response, start, call_event_id):
-        pass
+    def remote_enabled(self):
+        """Return True if the AppMap middleware has enabled remote recording, False otherwise."""
+
+    def run(self):
+        if not self.middleware_present():
+            return self.insert_middleware()
+
+        if self.remote_enabled() and not self.debug:
+            self._show_warning()
+
+        return None
+
+    def _show_warning(self):
+        # The user has explicitly asked for remote recording to be enabled in production. Let them
+        # know this probably isn't a good idea.
+        print("\n\n*** SECURITY RISK ***", file=sys.stderr)
+        msg = "Enabling remote recording in production can expose secret information."
+        print(
+            textwrap.fill(msg),
+            file=sys.stderr,
+        )
+        print("*** SECURITY RISK ***\n\n", file=sys.stderr)
+        logger.warning(msg)
+
+
+def initialize():
+    remote_recording.initialize()
```

### Comparing `appmap-1.9.1/appmap/command/appmap_agent_status.py` & `appmap-2.0.0/appmap/command/appmap_agent_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 import json
-import logging
-import os
 import sys
-import time
 from argparse import ArgumentParser
-from pathlib import Path
+from importlib.metadata import PackageNotFoundError, distribution, version
 
-import yaml
-from importlib_metadata import PackageNotFoundError, distribution, version
+from _appmap.configuration import Config
+from _appmap.env import Env
 
-from .._implementation.configuration import Config
-
-logger = logging.getLogger(__name__)
+logger = Env.current.getLogger(__name__)
 
 
 def has_dist(dist):
     try:
         distribution(dist)
         return True
     except PackageNotFoundError:
         pass
     return False
 
 
-class AgentFileCollector:
+class AgentFileCollector:  # pylint: disable=too-few-public-methods
     def __init__(self):
         self.collected = set()
 
     def pytest_collection_modifyitems(self, items):
         for item in items:
             self.collected.add(item.fspath)
         items.clear()
@@ -44,15 +39,15 @@
     logger.info("discovering pytest tests")
     # --capture=no => don't muck with stdout/stderr
     # --verbosity=-2 => don't do any logging during collection, and don't show warning summary
     # --disable-warnings => don't show warning summary
     #
     collector = AgentFileCollector()
 
-    import pytest
+    import pytest  # pylint: disable=import-outside-toplevel
 
     pytest.main(
         [
             "--collect-only",
             "--capture=no",
             "--verbosity=-2",
             "--disable-warnings",
@@ -69,26 +64,26 @@
 
 
 def has_unittest_tests():
     return False
 
 
 def _run(*, discover_tests):
-    config = Config()
+    config = Config.current
     uses_pytest = has_dist("pytest")
 
     has_tests = None
     if discover_tests:
         if uses_pytest:
             has_tests = has_pytest_tests()
         else:
             has_tests = has_unittest_tests()
 
     if has_tests:
-        test_command = {"args": [], "environment": {"APPMAP": "true"}}
+        test_command = {"args": []}
 
         if uses_pytest:
             test_command.update({"framework": "pytest", "command": "pytest"})
         else:
             test_command.update(
                 {
                     "framework": "unittest",
@@ -132,7 +127,11 @@
 def run():
     parser = ArgumentParser(description="Report project status for AppMap agent.")
     parser.add_argument(
         "--discover-tests", action="store_true", help="Scan the project for tests"
     )
     args = parser.parse_args()
     sys.exit(_run(discover_tests=args.discover_tests))
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `appmap-1.9.1/appmap/command/appmap_agent_validate.py` & `appmap-2.0.0/appmap/command/appmap_agent_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 import json
 import sys
+from importlib.metadata import PackageNotFoundError, version
 
-from importlib_metadata import PackageNotFoundError, version
-from packaging.version import Version, parse
+from packaging.version import parse
 
-from .._implementation.py_version_check import AppMapPyVerException, check_py_version
+from _appmap.py_version_check import AppMapPyVerException, check_py_version
 
 
 class ValidationFailure(Exception):
     def __init__(self, message, level="error", detailed_message=None, help_urls=None):
+        super().__init__()
         self.message = message
         self.level = level
         self.detailed_message = detailed_message
         self.help_urls = help_urls
 
     def to_dict(self):
         return {k: v for k, v in vars(self).items() if v is not None}
 
 
 def check_python_version():
     try:
         check_py_version()
     except AppMapPyVerException as e:
-        raise ValidationFailure(str(e))
+        raise ValidationFailure(str(e)) from e
 
 
 def _check_version(dist, v):
     dist_version = None
     try:
         dist_version = version(dist)
 
         required = parse(v)
         actual = parse(dist_version)
 
         if actual < required:
-            raise ValidationFailure(
-                f"{dist} must have version >= {required}, found {actual}"
-            )
+            raise ValidationFailure(f"{dist} must have version >= {required}, found {actual}")
     except PackageNotFoundError:
         pass
 
     return dist_version
 
 
 # Note that, per https://www.python.org/dev/peps/pep-0426/#name,
 # comparison of distribution names are case-insensitive.
 def check_django_version():
     return _check_version("django", "3.2")
 
 
 def check_flask_version():
-    return _check_version("flask", "1.1")
+    return _check_version("flask", "2.0")
 
 
 def check_pytest_version():
     return _check_version("pytest", "6.2")
 
 
 def _run():
     errors = [ValidationFailure("internal error")]  # shouldn't ever see this
     try:
         check_python_version()
         django_version = check_django_version()
         flask_version = check_flask_version()
         if not (django_version or flask_version):
-            raise ValidationFailure(
-                f"No web framework found. Expected one of: Django, Flask"
-            )
+            raise ValidationFailure("No web framework found. Expected one of: Django, Flask")
 
         check_pytest_version()
         errors = []
     except ValidationFailure as e:
         errors = [e]
 
     print(json.dumps([e.to_dict() for e in errors], indent=2))
 
     return 0 if len(errors) == 0 else 1
 
 
 def run():
     sys.exit(_run())
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `appmap-1.9.1/appmap/django.py` & `appmap-2.0.0/appmap/django.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,37 @@
 """Django integration. Captures HTTP requests and SQL queries.
 
-Automatically used in pytest tests. To enable remote recording,
-add appmap.django.Middleware to MIDDLEWARE in your app configuration
-and run with APPMAP=true set in the environment.
+Automatically used in pytest tests.
 """
 
 import json
 import re
 import sys
 import time
 
 import django
-from django.conf import settings
+from django.conf import settings as django_settings
 from django.core.handlers.base import BaseHandler
 from django.db.backends.signals import connection_created
 from django.db.backends.utils import CursorDebugWrapper
 from django.dispatch import receiver
-from django.http import HttpResponse, HttpResponseBadRequest, JsonResponse
 from django.template import Template
 from django.urls import get_resolver, resolve
 from django.urls.exceptions import Resolver404
-from django.urls.resolvers import _route_to_regex
 
-from appmap._implementation import generation, recorder, web_framework
-from appmap._implementation.env import Env
-from appmap._implementation.event import (
-    ExceptionEvent,
-    HttpServerRequestEvent,
-    HttpServerResponseEvent,
-    ReturnEvent,
-    SqlEvent,
-    _EventIds,
-)
-from appmap._implementation.instrument import is_instrumentation_disabled
-from appmap._implementation.recorder import Recorder
-from appmap._implementation.web_framework import AppmapMiddleware
-from appmap._implementation.web_framework import TemplateHandler as BaseTemplateHandler
+from _appmap.env import Env
+from _appmap.event import HttpServerRequestEvent, ReturnEvent, SqlEvent
+from _appmap.instrument import is_instrumentation_disabled
+from _appmap.metadata import Metadata
+from _appmap.recorder import Recorder
+from _appmap.utils import patch_class, values_dict
+from _appmap.web_framework import JSON_ERRORS, AppmapMiddleware, MiddlewareInserter
+from _appmap.web_framework import TemplateHandler as BaseTemplateHandler
 
-from ._implementation.metadata import Metadata
-from ._implementation.utils import patch_class, values_dict
+logger = Env.current.getLogger(__name__)
 
 
 def parse_pg_version(version):
     """Transform postgres version number like 120005 to a tuple like 12.0.5."""
     return (version // 10000 % 100, version // 100 % 100, version % 100)
 
 
@@ -61,19 +50,20 @@
 
 
 def add_metadata():
     """Adds Django framework to metadata for the next appmap generation."""
     Metadata.add_framework("Django", django.get_version())
 
 
-class ExecuteWrapper:
+class ExecuteWrapper:  # pylint: disable=too-few-public-methods
     def __init__(self):
         self.recorder = Recorder.get_current()
 
-    def __call__(self, execute, sql, params, many, context):
+    # This signature is correct, the implementation confuses pylint:
+    def __call__(self, execute, sql, params, many, context):  # pylint: disable=too-many-arguments
         start = time.monotonic()
         try:
             return execute(sql, params, many, context)
         finally:
             if is_instrumentation_disabled():
                 # We must be in the middle of fetching object representation.
                 # Don't record this query in the appmap.
@@ -91,17 +81,15 @@
                         times = len(params)
                     except TypeError:
                         times = "?"
                     sql = "%s times %s" % (times, sql)
                 else:
                     cursor = context["cursor"]
                     sql = conn.ops.last_executed_query(cursor, sql, params)
-                call_event = SqlEvent(
-                    sql, vendor=conn.vendor, version=database_version(conn)
-                )
+                call_event = SqlEvent(sql, vendor=conn.vendor, version=database_version(conn))
                 Recorder.add_event(call_event)
                 return_event = ReturnEvent(parent_id=call_event.id, elapsed=duration)
                 Recorder.add_event(return_event)
 
 
 # CursorDebugWrapper is used in tests to capture and examine queries.
 # However, recording appmap can cause additional queries to run when fetching
@@ -111,20 +99,21 @@
 
 
 def wrapped_execute(self, sql, params=None):
     """Directly execute the query if instrumentation is temporarily
     disabled, to avoid capturing queries not issued by the application."""
     if is_instrumentation_disabled():
         # fmt: off
-        return super().execute(sql, params) # pyright: ignore (seems like [superCallZeroArgForm] should suppress this, it doesn't)
+        # Seems like pyright: ignore [superCallZeroArgForm] should suppress this, it doesn't:
+        return super().execute(sql, params) # pyright: ignore
         # fmt on
     return original_execute(self, sql, params)
 
 
-CursorDebugWrapper.execute = wrapped_execute
+CursorDebugWrapper.execute = wrapped_execute  # type: ignore[method-assign]
 
 
 @receiver(connection_created)
 def connected(sender, connection, **_):
     # pylint: disable=unused-argument
 
     # warm the version cache in the backend to avoid running
@@ -146,45 +135,37 @@
 
     if request.content_type == "application/json":
         try:
             # Note: it's important to use request.body here instead of
             # directly reading request. This way the application can still
             # access the body which is now cached in the request object.
             params.update(json.loads(request.body))
-        except (json.decoder.JSONDecodeError, AttributeError):
+        except JSON_ERRORS:
             pass  # invalid json or not an object
 
     return values_dict(params.lists())
 
 
 def get_resolved_match(path_info, resolver):
     resolver_match = resolver.resolve(path_info)
 
-    # Sometimes the route returned by resolve is a regex, sometimes
-    # it's a url pattern.
-
-    # Start by assuming it's a regex.
-    regex = resolver_match.route
-
-    match = re.match(regex, path_info[1:])
-    if match:
-        return (regex, match)
-
-    # If it didn't match, it's a url pattern. Use _route_to_regex to
-    # turn it into a regex.  (url patterns sometimes start with a
-    # caret, which needs to be stripped before conversion.)
-    if regex[0] == "^":
-        regex = regex[1:]
-    regex = _route_to_regex(regex)[0]
+    # The last element of resolver_match.tried is the list of URLResolvers that matched path_info.
+    # Each URLResolver knows how to turn itself into a regex that will match the appropriate portion
+    # of the path. Iterate through them and create a complete regex for the path.
+    parts = []
+    for part in resolver_match.tried[-1]:
+        # Django inserts a leading '^'.
+        r = part.pattern.regex.pattern.lstrip("^")
+        parts.append(r)
+    regex = "".join(parts)
 
     match = re.match(regex, path_info[1:])
     if not match:
         raise RuntimeError(
-            "No match for %s found with resolver %r, regex %s"
-            % (path_info, resolver, regex)
+            "No match for %s found with resolver %r, regex %s" % (path_info, resolver, regex)
         )
 
     return (regex, match)
 
 
 def normalize_path_info(path_info, resolved):
     if not resolved.kwargs:
@@ -221,130 +202,121 @@
     ensure that requests get handled in separate threads.
 
     More discussion about sync vs async middleware can be found in the Django
     doc: https://docs.djangoproject.com/en/4.1/topics/http/middleware/#async-middleware.
     """
 
     def __init__(self, get_response):
+        super().__init__("Django")
         self.get_response = get_response
         self.recorder = Recorder.get_current()
-        self.record_url = "/_appmap/record"
 
     def __call__(self, request):
-        if not Env.current.enabled:
+        if not self.should_record:
             return self.get_response(request)
 
-        if request.path_info == self.record_url:
-            return self.recording(request)
-
-        rec, start, call_event_id = self.before_request_hook(
-            request, request.path_info, self.record_url, self.recorder.get_enabled()
-        )
+        rec, start, call_event_id = self.before_request_hook(request)
+        if rec is None:
+            return self.get_response(request)
 
         try:
             response = self.get_response(request)
         except:
-            if rec.get_enabled():
-                duration = time.monotonic() - start
-                exception_event = ExceptionEvent(
-                    parent_id=call_event_id,
-                    elapsed=duration,
-                    exc_info=sys.exc_info(),
-                )
-                rec.add_event(exception_event)
+            self.on_exception(rec, start, call_event_id, sys.exc_info())
             raise
 
         self.after_request_hook(
-            request,
             request.path_info,
-            self.record_url,
-            self.recorder.get_enabled(),
             request.method,
             request.build_absolute_uri(),
-            response,
-            response,
+            response.status_code,
+            response.headers,
             start,
             call_event_id,
         )
 
         return response
 
-    def before_request_main(self, rec, request):
+    def before_request_main(self, rec, req):
         add_metadata()
         start = time.monotonic()
-        params = request_params(request)
+        params = request_params(req)
         try:
-            resolved = resolve(request.path_info)
+            resolved = resolve(req.path_info)
             params.update(resolved.kwargs)
-            normalized_path_info = normalize_path_info(request.path_info, resolved)
+            normalized_path_info = normalize_path_info(req.path_info, resolved)
         except Resolver404:
             # If the request was for a bad path (e.g. when an app
             # is testing 404 handling), resolving will fail.
             normalized_path_info = None
 
         call_event = HttpServerRequestEvent(
-            request_method=request.method,
-            path_info=request.path_info,
+            request_method=req.method,
+            path_info=req.path_info,
             message_parameters=params,
             normalized_path_info=normalized_path_info,
-            protocol=request.META["SERVER_PROTOCOL"],
-            headers=request.headers,
+            protocol=req.META["SERVER_PROTOCOL"],
+            headers=req.headers,
         )
         rec.add_event(call_event)
 
         return start, call_event.id
 
-    def after_request_main(self, rec, response, start, call_event_id):
-        duration = time.monotonic() - start
-        return_event = HttpServerResponseEvent(
-            parent_id=call_event_id,
-            elapsed=duration,
-            status_code=response.status_code,
-            headers=dict(response.items()),
-        )
-        rec.add_event(return_event)
 
-    def recording(self, request):
-        """Handle recording requests."""
-        if request.method == "GET":
-            return JsonResponse({"enabled": self.recorder.get_enabled()})
-        if request.method == "POST":
-            if self.recorder.get_enabled():
-                return HttpResponse("Recording is already in progress", status=409)
-            self.recorder.start_recording()
-            return HttpResponse()
-
-        if request.method == "DELETE":
-            if not self.recorder.get_enabled():
-                return HttpResponse("No recording is in progress", status=404)
-
-            self.recorder.stop_recording()
-            return HttpResponse(
-                generation.dump(self.recorder), content_type="application/json"
+class DjangoInserter(MiddlewareInserter):
+    def __init__(self, settings):
+        super().__init__(settings.DEBUG)
+        self.settings = settings
+
+    def middleware_present(self):
+        return "appmap.django.Middleware" in self.settings.MIDDLEWARE
+
+    def insert_middleware(self):
+        stack = list(self.settings.MIDDLEWARE)
+
+        new_middleware = ["appmap.django.Middleware"]
+        enable_by_default = "true" if self.debug else "false"
+        if Env.current.enables("remote", enable_by_default):
+            new_middleware.insert(0, "_appmap.django.RemoteRecording")
+
+        stack[0:0] = new_middleware
+        # Django is ok with settings.MIDDLEWARE being any kind iterable. Update it, without changing
+        # its type, if we can.
+        msg = (
+            "Don't know how to update settings.MIDDLEWARE of type %s, recording is not enabled.",
+        )
+        if isinstance(self.settings.MIDDLEWARE, list):
+            self.settings.MIDDLEWARE = stack
+        elif isinstance(self.settings.MIDDLEWARE, tuple):
+            self.settings.MIDDLEWARE = tuple(stack)
+        else:
+            logger.warning(
+                msg,
+                type(self.settings.MIDDLEWARE),
             )
 
-        return HttpResponseBadRequest()
+    def remote_enabled(self):
+        return "_appmap.django.RemoteRecording" in self.settings.MIDDLEWARE
 
 
 def inject_middleware():
     """Make sure AppMap middleware is added to the stack"""
-    if "appmap.django.Middleware" not in settings.MIDDLEWARE:
-        settings.MIDDLEWARE.insert(0, "appmap.django.Middleware")
+    DjangoInserter(django_settings).run()
 
 
 original_load_middleware = BaseHandler.load_middleware
 
 
 def load_middleware(*args, **kwargs):
     """Patched wrapper to inject AppMap middleware first"""
     inject_middleware()
     return original_load_middleware(*args, **kwargs)
 
 
-BaseHandler.load_middleware = load_middleware
+BaseHandler.load_middleware = load_middleware  # type: ignore[method-assign]
 
 
 @patch_class(Template)
 class TemplateHandler(BaseTemplateHandler):
     @property
     def filename(self):
         """The full path of the template file."""
```

### Comparing `appmap-1.9.1/appmap/http.py` & `appmap-2.0.0/appmap/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 appmap events of any HTTP requests.
 """
 
 import time
 from http.client import HTTPConnection
 from urllib.parse import parse_qs, urlsplit
 
-from ._implementation.event import HttpClientRequestEvent, HttpClientResponseEvent
-from ._implementation.recorder import Recorder
-from ._implementation.utils import patch_class, values_dict
+from _appmap.event import HttpClientRequestEvent, HttpClientResponseEvent
+from _appmap.recorder import Recorder
+from _appmap.utils import patch_class, values_dict
 
 
 def is_secure(self: HTTPConnection):
     """Checks whether HTTP connection is secure."""
     # isinstance(self, HTTPSConnection) won't work with
     # eg. urllib3 HTTPConnection. Instead try duck typing.
     return hasattr(self, "key_file")
@@ -48,15 +48,15 @@
         orig(self, method, url, *args, **kwargs)
 
     def putheader(self, orig, header, *values):
         request = self._appmap_request.http_client_request
         if not hasattr(request, "headers"):
             request["headers"] = {}
         headers = request["headers"]
-        if not header in headers:
+        if header not in headers:
             headers[header] = []
         headers[header].extend(values)
         orig(self, header, *values)
 
     def getresponse(self, orig):
         event = self._appmap_request
         del self._appmap_request
```

### Comparing `appmap-1.9.1/appmap/labeling/crypto.yml` & `appmap-2.0.0/appmap/labeling/crypto.yml`

 * *Files identical despite different names*

### Comparing `appmap-1.9.1/appmap/pytest.py` & `appmap-2.0.0/appmap/pytest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+from importlib.metadata import version
+
 import pytest
 
-import appmap
-import appmap.wrapt as wrapt
-from appmap._implementation import testing_framework
+from _appmap import noappmap, testing_framework, wrapt
+from _appmap.env import Env
+
+logger = Env.current.getLogger(__name__)
 
 
-class recorded_testcase:
+class recorded_testcase:  # pylint: disable=too-few-public-methods
     def __init__(self, item):
         self.item = item
 
     @wrapt.decorator
     def __call__(self, wrapped, _, args, kwargs):
         item = self.item
         with item.session.appmap.record(
             item.cls, item.name, method_id=item.originalname, location=item.location
         ) as metadata:
             with testing_framework.collect_result_metadata(metadata):
                 return wrapped(*args, **kwargs)
 
 
-if appmap.enabled():
+if not Env.current.is_appmap_repo and Env.current.enables("tests"):
+    logger.debug("Test recording is enabled (Pytest)")
 
     @pytest.hookimpl
     def pytest_sessionstart(session):
         session.appmap = testing_framework.session(
-            name="pytest", recorder_type="tests", version=pytest.__version__
+            name="pytest", recorder_type="tests", version=version("pytest")
         )
 
     @pytest.hookimpl
     def pytest_runtest_call(item):
         # The presence of a `_testcase` attribute on an item indicates
         # that it was created from a `unittest.TestCase`. An item
         # created from a TestCase has an `obj` attribute, assigned
@@ -45,29 +49,36 @@
         # instrumentation decorator will be called, recording the
         # `call` event. Finally, the original function will be called,
         # running the test case. (This nesting of function calls is
         # verified by the expected appmap in the test for a unittest
         # TestCase run by pytest.)
         if hasattr(item, "_testcase"):
             setattr(
-                item._testcase, "_appmap_pytest_recording", True
-            )  # pylint: disable=protected-access
-            item.obj = recorded_testcase(item)(item.obj)
+                item._testcase,  # pylint: disable=protected-access
+                "_appmap_pytest_recording",
+                True,
+            )
+            if not noappmap.disables(item.obj, item.cls):
+                item.obj = recorded_testcase(item)(item.obj)
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_pyfunc_call(pyfuncitem):
         # There definitely shouldn't be a `_testcase` attribute on a
         # pytest test.
         assert not hasattr(pyfuncitem, "_testcase")
 
+        if noappmap.disables(pyfuncitem.function, pyfuncitem.cls):
+            yield
+            return
+
         with pyfuncitem.session.appmap.record(
             pyfuncitem.cls,
             pyfuncitem.name,
             method_id=pyfuncitem.originalname,
             location=pyfuncitem.location,
         ) as metadata:
             result = yield
             try:
                 with testing_framework.collect_result_metadata(metadata):
                     result.get_result()
-            except:  # pylint: disable=bare-except
+            except:  # pylint: disable=bare-except   # noqa: E722
                 pass  # exception got recorded in metadata
```

### Comparing `appmap-1.9.1/appmap/sqlalchemy.py` & `appmap-2.0.0/appmap/sqlalchemy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """SQL statement capture for SQLAlchemy."""
 
 import time
+from importlib.metadata import version
 
-import sqlalchemy
 from sqlalchemy import event
 from sqlalchemy.engine import Engine
 
-from appmap._implementation.event import ReturnEvent, SqlEvent
-from appmap._implementation.instrument import is_instrumentation_disabled
-from appmap._implementation.recorder import Recorder
-
-from ._implementation.metadata import Metadata
+from _appmap.event import ReturnEvent, SqlEvent
+from _appmap.instrument import is_instrumentation_disabled
+from _appmap.metadata import Metadata
+from _appmap.recorder import Recorder
 
 
 @event.listens_for(Engine, "before_cursor_execute")
 # pylint: disable=too-many-arguments,unused-argument
 def capture_sql_call(conn, cursor, statement, parameters, context, executemany):
-    """Capture SQL query callinto appmap."""
+    """Capture SQL query call into appmap."""
     if is_instrumentation_disabled():
         # We must be in the middle of fetching object representation.
         # Don't record this query in the appmap.
         pass
     elif Recorder.get_enabled():
-        Metadata.add_framework("SQLAlchemy", sqlalchemy.__version__)
+        Metadata.add_framework("SQLAlchemy", version("sqlalchemy"))
         if executemany:
             # Sometimes the same query is executed with different parameter sets.
             # Instead of substituting them all, just say how many times it was run.
             try:
                 times = len(parameters)
             except TypeError:
                 times = "?"
```

### Comparing `appmap-1.9.1/appmap/test/appmap_test_base.py` & `appmap-2.0.0/_appmap/test/appmap_test_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import json
 import platform
 import re
+from importlib.metadata import version as dist_version
 from operator import itemgetter
 
 import pytest
 
-import appmap._implementation
-from appmap._implementation.recorder import Recorder
+import _appmap
+from _appmap.recorder import Recorder
 
 
 def normalize_path(path):
     """
     Normalize absolute path to a file in a package down to a package path.
     Not foolproof, but good enough for the tests.
     """
     return re.sub(r"^.*site-packages/", "", path)
 
 
 class AppMapTestBase:
     def setup_method(self, _):
-        appmap._implementation.initialize()  # pylint: disable=protected-access
+        _appmap.initialize()  # pylint: disable=protected-access
 
     @staticmethod
     @pytest.fixture
     def events():
+        # pylint: disable=protected-access
         rec = Recorder.get_current()
         rec.clear()
         rec._enabled = True
         return rec.events
 
     @staticmethod
     def normalize_git(git):
@@ -56,15 +58,15 @@
         assert version == platform.python_version()
 
         if "frameworks" in metadata:
             frameworks = metadata["frameworks"]
             for f in frameworks:
                 if f["name"] == "pytest":
                     v = f.pop("version")
-                    assert v == pytest.__version__
+                    assert v == dist_version("pytest")
 
     def normalize_appmap(self, generated_appmap):
         """
         Normalize the data in generated_appmap, removing any
         environment-specific values.
 
         Note that attempts to access required keys will raise
```

### Comparing `appmap-1.9.1/appmap/test/data/django/app/urls.py` & `appmap-2.0.0/_appmap/test/data/django/djangoapp/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,18 @@
     return django.http.HttpResponse("testing")
 
 
 def user_view(_request, username):
     return django.http.HttpResponse(f"user {username}")
 
 
+def org_user_posts_view(_request, org, username):
+    return django.http.HttpResponse(f"org {org} user {username}")
+
+
 def post_view(_request, post_id):
     return django.http.HttpResponse(f"post {post_id}")
 
 
 def post_unnamed_view(_request, arg):
     return django.http.HttpResponse(f"post with unnamed, {arg}")
 
@@ -65,9 +69,13 @@
     re_path("^user/(?P<username>[^/]+)$", user_view),
     path("post/<int:post_id>", post_view),
     path("post/<username>/<int:post_id>/summary", user_post_view),
     re_path(r"^post/unnamed/(\d+)$", post_unnamed_view),
     path("echo", echo_view),
     path("exception", exception_view),
     re_path(r"^post/included/", include([path("<username>", user_view)])),
+    re_path(
+        r"^(?P<org>\d+)/posts/",
+        include([path("<username>", org_user_posts_view)]),
+    ),
     re_path(r"^admincp/", include((admincp_patterns, "admin"), namespace="admin")),
 ]
```

### Comparing `appmap-1.9.1/appmap/test/data/django/manage.py` & `appmap-2.0.0/_appmap/test/data/django/manage.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Django's command-line utility for administrative tasks."""
 import os
 import sys
 
 
 def main():
     """Run administrative tasks."""
-    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "app.settings")
+    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "djangoapp.settings")
     try:
         from django.core.management import execute_from_command_line
     except ImportError as exc:
         raise ImportError(
             "Couldn't import Django. Are you sure it's installed and "
             "available on your PYTHONPATH environment variable? Did you "
             "forget to activate a virtual environment?"
```

### Comparing `appmap-1.9.1/appmap/test/data/example_class.py` & `appmap-2.0.0/_appmap/test/data/example_class.py`

 * *Files identical despite different names*

### Comparing `appmap-1.9.1/appmap/test/data/expected.appmap.json` & `appmap-2.0.0/_appmap/test/data/expected.appmap.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968026620370372%*

 * *Differences: {"'classMap'": "{0: {'children': {0: {'children': {0: {'location': "*

 * *               "'_appmap/test/data/example_class.py'}}}, 1: {'children': {0: {'location': "*

 * *               "'_appmap/test/data/example_class.py'}, 1: {'location': "*

 * *               "'_appmap/test/data/example_class.py'}, 2: {'location': "*

 * *               "'_appmap/test/data/example_class.py'}, 3: {'location': "*

 * *               "'_appmap/test/data/example_class.py'}}}, 2: {'children': {0: {'location': "*

 * *               "'_appmap/test/data/examp […]*

```diff
@@ -1,60 +1,60 @@
 {
     "classMap": [
         {
             "children": [
                 {
                     "children": [
                         {
-                            "location": "appmap/test/data/example_class.py",
+                            "location": "_appmap/test/data/example_class.py",
                             "name": "class_method",
                             "static": true,
                             "type": "function"
                         }
                     ],
                     "name": "ClassMethodMixin",
                     "type": "class"
                 },
                 {
                     "children": [
                         {
-                            "location": "appmap/test/data/example_class.py",
+                            "location": "_appmap/test/data/example_class.py",
                             "name": "call_yaml",
                             "static": true,
                             "type": "function"
                         },
                         {
-                            "location": "appmap/test/data/example_class.py",
+                            "location": "_appmap/test/data/example_class.py",
                             "name": "dump_yaml",
                             "static": true,
                             "type": "function"
                         },
                         {
-                            "location": "appmap/test/data/example_class.py",
+                            "location": "_appmap/test/data/example_class.py",
                             "name": "static_method",
                             "static": true,
                             "type": "function"
                         },
                         {
                             "labels": [
                                 "example-label"
                             ],
-                            "location": "appmap/test/data/example_class.py",
+                            "location": "_appmap/test/data/example_class.py",
                             "name": "test_exception",
                             "static": false,
                             "type": "function"
                         }
                     ],
                     "name": "ExampleClass",
                     "type": "class"
                 },
                 {
                     "children": [
                         {
-                            "location": "appmap/test/data/example_class.py",
+                            "location": "_appmap/test/data/example_class.py",
                             "name": "instance_method",
                             "static": false,
                             "type": "function"
                         }
                     ],
                     "name": "Super",
                     "type": "class"
@@ -65,14 +65,15 @@
         },
         {
             "children": [
                 {
                     "comment": "function comment",
                     "labels": [
                         "format.yaml.generate",
+                        "serialize",
                         "serialization",
                         "example-label"
                     ],
                     "location": "yaml/__init__.py",
                     "name": "dump",
                     "static": true,
                     "type": "function"
@@ -85,15 +86,15 @@
     "events": [
         {
             "defined_class": "example_class.ExampleClass",
             "event": "call",
             "id": 1,
             "method_id": "static_method",
             "parameters": [],
-            "path": "appmap/test/data/example_class.py",
+            "path": "_appmap/test/data/example_class.py",
             "static": true,
             "thread_id": 1
         },
         {
             "event": "return",
             "id": 2,
             "parent_id": 1,
@@ -105,15 +106,15 @@
         },
         {
             "defined_class": "example_class.ClassMethodMixin",
             "event": "call",
             "id": 3,
             "method_id": "class_method",
             "parameters": [],
-            "path": "appmap/test/data/example_class.py",
+            "path": "_appmap/test/data/example_class.py",
             "receiver": {
                 "class": "builtins.type",
                 "kind": "req",
                 "name": "cls",
                 "value": "<class 'example_class.ExampleClass'>"
             },
             "static": true,
@@ -131,15 +132,15 @@
         },
         {
             "defined_class": "example_class.Super",
             "event": "call",
             "id": 5,
             "method_id": "instance_method",
             "parameters": [],
-            "path": "appmap/test/data/example_class.py",
+            "path": "_appmap/test/data/example_class.py",
             "receiver": {
                 "class": "example_class.ExampleClass",
                 "kind": "req",
                 "name": "self",
                 "value": "ExampleClass and ExampleClass#another_method"
             },
             "static": false,
@@ -157,15 +158,15 @@
         },
         {
             "defined_class": "example_class.ExampleClass",
             "event": "call",
             "id": 7,
             "method_id": "test_exception",
             "parameters": [],
-            "path": "appmap/test/data/example_class.py",
+            "path": "_appmap/test/data/example_class.py",
             "receiver": {
                 "class": "example_class.ExampleClass",
                 "kind": "req",
                 "name": "self",
                 "value": "ExampleClass and ExampleClass#another_method"
             },
             "static": false,
@@ -185,15 +186,15 @@
         },
         {
             "defined_class": "example_class.ExampleClass",
             "event": "call",
             "id": 9,
             "method_id": "call_yaml",
             "parameters": [],
-            "path": "appmap/test/data/example_class.py",
+            "path": "_appmap/test/data/example_class.py",
             "static": true,
             "thread_id": 1
         },
         {
             "defined_class": "example_class.ExampleClass",
             "event": "call",
             "id": 10,
@@ -202,15 +203,15 @@
                 {
                     "class": "builtins.str",
                     "kind": "req",
                     "name": "data",
                     "value": "'ExampleClass.call_yaml'"
                 }
             ],
-            "path": "appmap/test/data/example_class.py",
+            "path": "_appmap/test/data/example_class.py",
             "static": true,
             "thread_id": 1
         },
         {
             "defined_class": "yaml",
             "event": "call",
             "id": 11,
```

### Comparing `appmap-1.9.1/appmap/test/data/flask/app.py` & `appmap-2.0.0/_appmap/test/data/flask/flaskapp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""Rudimentary Flask application for testing."""
+"""
+Rudimentary Flask application for testing.
+
+NB: This should not explicitly reference the `appmap` module in any way. Doing so invalidates
+testing of record-by-default.
+"""
 # pylint: disable=missing-function-docstring
 
 from flask import Flask, make_response
 from markupsafe import escape
 
-from appmap.flask import AppmapFlask
-
 app = Flask(__name__)
 
-appmap_flask = AppmapFlask(app)
-
 
 @app.route("/")
 def hello_world():
     return "Hello, World!"
 
 
 @app.route("/test")
@@ -35,7 +36,17 @@
     return "Post %d" % post_id
 
 
 @app.route("/post/<username>/<int:post_id>/summary")
 def show_user_post(username, post_id):
     # Show the summary of a user's post
     return f"User {escape(username)} post {post_id}"
+
+
+@app.route("/<int:org>/posts/<username>")
+def show_org_user_posts(org, username):
+    return f"org {org} username {username}"
+
+
+@app.route("/exception")
+def raise_exception():
+    raise Exception("An exception")
```

### Comparing `appmap-1.9.1/appmap/test/data/params.py` & `appmap-2.0.0/_appmap/test/data/params.py`

 * *Files identical despite different names*

### Comparing `appmap-1.9.1/appmap/test/data/pytest/expected/pytest.appmap.json` & `appmap-2.0.0/_appmap/test/data/pytest/expected/pytest.appmap.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'metadata'": "{'source_location': 'test_simple.py:5', delete: ['recording']}"}*

```diff
@@ -125,14 +125,12 @@
             "name": "python"
         },
         "name": "hello world",
         "recorder": {
             "name": "pytest",
             "type": "tests"
         },
-        "recording": {
-            "source_location": "test_simple.py:5"
-        },
+        "source_location": "test_simple.py:5",
         "test_status": "succeeded"
     },
     "version": "1.9"
 }
```

### Comparing `appmap-1.9.1/appmap/test/data/trial/expected/pytest.appmap.json` & `appmap-2.0.0/_appmap/test/data/trial/expected/pytest.appmap.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9854166666666666%*

 * *Differences: {"'metadata'": "{'recording': {delete: ['source_location']}, 'source_location': "*

 * *               "'test/test_deferred.py:7'}"}*

```diff
@@ -68,14 +68,14 @@
         "name": "Deferred hello world",
         "recorder": {
             "name": "pytest",
             "type": "tests"
         },
         "recording": {
             "defined_class": "test.test_deferred.TestDeferred",
-            "method_id": "test_hello_world",
-            "source_location": "test/test_deferred.py:7"
+            "method_id": "test_hello_world"
         },
+        "source_location": "test/test_deferred.py:7",
         "test_status": "succeeded"
     },
     "version": "1.9"
 }
```

### Comparing `appmap-1.9.1/appmap/test/data/unittest/expected/pytest.appmap.json` & `appmap-2.0.0/_appmap/test/data/unittest/expected/pytest.appmap.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9854166666666666%*

 * *Differences: {"'metadata'": "{'recording': {delete: ['source_location']}, 'source_location': "*

 * *               "'simple/test_simple.py:13'}"}*

```diff
@@ -180,14 +180,14 @@
         "name": "Unit test test hello world",
         "recorder": {
             "name": "pytest",
             "type": "tests"
         },
         "recording": {
             "defined_class": "simple.test_simple.UnitTestTest",
-            "method_id": "test_hello_world",
-            "source_location": "simple/test_simple.py:13"
+            "method_id": "test_hello_world"
         },
+        "source_location": "simple/test_simple.py:13",
         "test_status": "succeeded"
     },
     "version": "1.9"
 }
```

### Comparing `appmap-1.9.1/appmap/test/data/unittest/expected/unittest.appmap.json` & `appmap-2.0.0/_appmap/test/data/unittest/expected/unittest.appmap.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9854166666666666%*

 * *Differences: {"'metadata'": "{'recording': {delete: ['source_location']}, 'source_location': "*

 * *               "'simple/test_simple.py:14'}"}*

```diff
@@ -180,14 +180,14 @@
         "name": "Unit test test hello world",
         "recorder": {
             "name": "unittest",
             "type": "tests"
         },
         "recording": {
             "defined_class": "simple.test_simple.UnitTestTest",
-            "method_id": "test_hello_world",
-            "source_location": "simple/test_simple.py:14"
+            "method_id": "test_hello_world"
         },
+        "source_location": "simple/test_simple.py:14",
         "test_status": "succeeded"
     },
     "version": "1.9"
 }
```

### Comparing `appmap-1.9.1/appmap/test/data/unittest/simple/test_simple.py` & `appmap-2.0.0/_appmap/test/data/unittest/simple/test_simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import unittest
 from unittest.mock import patch
 
-import simple
+import simple  # isort: skip
 
 # Importing from decouple will cause a failure if we're not hooking
 # finders correctly.
-from decouple import config
+from decouple import config  # noqa: F401
 
-import appmap.unittest
+import appmap
 
 
 class UnitTestTest(unittest.TestCase):
     def test_hello_world(self):
         self.assertEqual(simple.Simple().hello_world("!"), "Hello world!")
 
     @patch("simple.Simple.hello_world")
@@ -35,7 +35,15 @@
         raise RuntimeError("test error")
 
     def setUp(self):
         simple.Simple().getReady()
 
     def tearDown(self):
         simple.Simple().finishUp()
+
+    def test_with_subtest(self):
+        with self.subTest("subtest"):
+            self.assertEqual(simple.Simple().hello_world("!"), "Hello world!")
+
+    @appmap.noappmap
+    def test_unrecorded(self):
+        print(simple.Simple().hello_world("!"))
```

### Comparing `appmap-1.9.1/appmap/test/normalize.py` & `appmap-2.0.0/_appmap/test/normalize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import platform
 import re
+from importlib.metadata import version as dist_version
 from operator import itemgetter
 from typing import List
 
-import pytest
-
 
 def normalize_path(path):
     """
     Normalize absolute path to a file in a package down to a package path.
     Not foolproof, but good enough for the tests.
     """
     return re.sub(r"^.*site-packages/", "", path)
@@ -41,33 +40,38 @@
     assert version == platform.python_version()
 
     if "frameworks" in metadata:
         frameworks = metadata["frameworks"]
         for f in frameworks:
             if f["name"] == "pytest":
                 v = f.pop("version")
-                assert v == pytest.__version__
+                assert v == dist_version("pytest")
 
 
 def normalize_headers(dct):
     """Remove some headers which are variable between implementations.
     This allows sharing tests between web frameworks, for example.
     """
-    for hdr in ["User-Agent", "Content-Length", "ETag", "Cookie", "Host"]:
-        value = dct.pop(hdr, None)
-        assert value is None or isinstance(value, str)
+    for key in list(dct.keys()):
+        value = dct.pop(key, None)
+        key = key.lower()
+        if key in ["user-agent", "content-length", "content-type", "etag", "cookie", "host"]:
+            assert value is None or isinstance(value, str)
+        else:
+            dct[key] = value
 
 
 def normalize_appmap(generated_appmap):
     """
     Normalize the data in generated_appmap, removing any
     environment-specific values.
     """
 
     def normalize(dct):
+        # pylint: disable=too-many-branches
         if "classMap" in dct:
             dct["classMap"].sort(key=itemgetter("name"))
         if "children" in dct:
             dct["children"].sort(key=itemgetter("name"))
         if "comment" in dct:
             dct["comment"] = "function comment"
         if "elapsed" in dct:
@@ -79,14 +83,19 @@
         if "git" in dct:
             normalize_git(dct.pop("git"))
         if "headers" in dct:
             normalize_headers(dct["headers"])
             if len(dct["headers"]) == 0:
                 del dct["headers"]
         if "http_server_request" in dct:
+            # the "headers" property is optional, and will be different
+            # depending on the client sending the request. Rather than expecting
+            # particular headers, the test code should verify that other
+            # properties based on headers (e.g. "mime_type") are set correctly.
+            dct["http_server_request"].pop("headers", None)
             normalize(dct["http_server_request"])
             if "message" in dct:
                 del dct["message"]
         if "location" in dct:
             dct["location"] = normalize_path(dct["location"])
         if "path" in dct:
             dct["path"] = normalize_path(dct["path"])
```

### Comparing `appmap-1.9.1/appmap/test/test_command.py` & `appmap-2.0.0/_appmap/test/test_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,140 +1,141 @@
 import json
-import os
 import re
 from distutils.dir_util import copy_tree
-from pathlib import Path
+from importlib.metadata import version
 
 import pytest
-from importlib_metadata import version
 
-import appmap._implementation
+import _appmap
 from appmap.command import appmap_agent_init, appmap_agent_status, appmap_agent_validate
 
 from .helpers import DictIncluding
 
 
-@pytest.fixture
-def cmd_setup(request, git, data_dir, monkeypatch):
+@pytest.fixture(name="_cmd_setup")
+def _cmd_setup(request, git, data_dir, monkeypatch):
     repo_root = git.cwd
     copy_tree(data_dir / request.param, str(repo_root))
     monkeypatch.chdir(repo_root)
 
     # pylint: disable=protected-access
-    appmap._implementation.initialize(cwd=repo_root)
+    _appmap.initialize(cwd=repo_root)
 
     return monkeypatch
 
 
-@pytest.mark.parametrize("cmd_setup", ["config"], indirect=True)
-def test_agent_init(cmd_setup, capsys):
-    rc = appmap_agent_init._run()
+@pytest.mark.parametrize("_cmd_setup", ["config"], indirect=True)
+def test_agent_init(_cmd_setup, capsys):
+    rc = appmap_agent_init._run()  # pylint: disable=protected-access
+
     assert rc == 0
     output = capsys.readouterr()
     config = json.loads(output.out)
 
     # Make sure the JSON has the correct form, and contains the
     # expected filename. The contents of the default appmap.yml are
     # verified by other tests
     assert config["configuration"]["filename"] == "appmap.yml"
     assert config["configuration"]["contents"] is not None
 
 
 class TestAgentStatus:
-    @pytest.mark.parametrize("cmd_setup", ["pytest"], indirect=True)
+    @pytest.mark.parametrize("_cmd_setup", ["pytest"], indirect=True)
     @pytest.mark.parametrize("do_discovery", [True, False])
-    def test_test_discovery_control(self, cmd_setup, do_discovery, mocker):
+    def test_test_discovery_control(self, _cmd_setup, do_discovery, mocker):
         mocker.patch("appmap.command.appmap_agent_status.discover_pytest_tests")
-        rc = appmap_agent_status._run(discover_tests=do_discovery)
+        rc = appmap_agent_status._run(  # pylint: disable=protected-access
+            discover_tests=do_discovery
+        )
         assert rc == 0
         call_count = 1 if do_discovery else 0
+
+        # Well, pylint, if it didn't have call_count, assertion would fail,
+        # wouldn't it?
+        # pylint: disable=no-member
         assert appmap_agent_status.discover_pytest_tests.call_count == call_count
 
-    @pytest.mark.parametrize("cmd_setup", ["pytest"], indirect=True)
-    def test_agent_status(self, cmd_setup, capsys):
-        rc = appmap_agent_status._run(discover_tests=True)
+    @pytest.mark.parametrize("_cmd_setup", ["pytest"], indirect=True)
+    def test_agent_status(self, _cmd_setup, capsys):
+        rc = appmap_agent_status._run(discover_tests=True)  # pylint: disable=protected-access
+
         assert rc == 0
         output = capsys.readouterr()
         status = json.loads(output.out)
         # XXX This will detect pytest as the test framework, because
         # appmap-python uses it. We need a better mechanism to handle
         # testing more broadly.
-        assert status == DictIncluding(
+        props = status["properties"]
+        config = props["config"]
+        assert config == DictIncluding({"app": "Simple", "present": True, "valid": True})
+        project = props["project"]
+        assert project == DictIncluding(
             {
-                "properties": {
-                    "config": {"app": "Simple", "present": True, "valid": True},
-                    "project": {
-                        "agentVersion": "0.0.0",
-                        "language": "python",
-                        "remoteRecordingCapable": True,
-                        "integrationTests": True,
-                    },
-                },
-                "test_commands": [
-                    {
-                        "args": [],
-                        "framework": "pytest",
-                        "command": "pytest",
-                        "environment": {"APPMAP": "true"},
-                    }
-                ],
+                "language": "python",
+                "remoteRecordingCapable": True,
+                "integrationTests": True,
             }
         )
+        assert "agentVersion" in project
+        test_commands = status["test_commands"]
+        assert test_commands[0] == DictIncluding(
+            {"args": [], "framework": "pytest", "command": "pytest"}
+        )
+
+    @pytest.mark.parametrize("_cmd_setup", ["package1"], indirect=True)
+    def test_agent_status_no_commands(self, _cmd_setup, capsys):
+        rc = appmap_agent_status._run(discover_tests=True)  # pylint: disable=protected-access
 
-    @pytest.mark.parametrize("cmd_setup", ["package1"], indirect=True)
-    def test_agent_status(self, cmd_setup, capsys):
-        rc = appmap_agent_status._run(discover_tests=True)
         assert rc == 0
         output = capsys.readouterr()
         status = json.loads(output.out)
 
         assert "test_commands" not in status
 
 
 class TestAgentValidate:
     def check_errors(self, capsys, status, count, msg):
-        rc = appmap_agent_validate._run()
+        rc = appmap_agent_validate._run()  # pylint: disable=protected-access
+
         assert rc == status
 
         output = capsys.readouterr()
         errors = json.loads(output.out)
 
         assert len(errors) == count
         if count > 0:
             err = errors[0]
             assert err["level"] == "error"
-            assert re.match(msg, err["message"]) != None
+            assert re.match(msg, err["message"]) is not None
 
-    def test_no_errors(self, capsys, mocker):
+    def test_no_errors(self, capsys):
         # Both Django and flask are installed in a dev environment, so
         # validation will succeed.
         self.check_errors(capsys, 0, 0, None)
 
     def test_python_version(self, capsys, mocker):
         mocker.patch(
-            "appmap._implementation.py_version_check._get_py_version",
+            "_appmap.py_version_check._get_py_version",
             return_value=(3, 5),
         )
         mocker.patch(
-            "appmap._implementation.py_version_check._get_platform_version",
+            "_appmap.py_version_check._get_platform_version",
             return_value="3.5",
         )
 
-        self.check_errors(
-            capsys, 1, 1, r"Minimum Python version supported is \d\.\d, found"
-        )
+        self.check_errors(capsys, 1, 1, r"Minimum Python version supported is \d\.\d, found")
 
     def test_django_version(self, capsys, mocker):
-        m = mocker.patch(
+        mocker.patch(
             "appmap.command.appmap_agent_validate.version",
             side_effect=lambda d: "3.1" if d == "django" else version(d),
         )
 
         self.check_errors(capsys, 1, 1, "django must have version >= 3.2, found 3.1")
 
     def test_flask_version(self, capsys, mocker):
-        m = mocker.patch(
+        mocker.patch(
             "appmap.command.appmap_agent_validate.version",
             side_effect=lambda d: "1.0" if d == "flask" else version(d),
         )
 
-        self.check_errors(capsys, 1, 1, "flask must have version >= 1.1, found 1.0")
+        self.check_errors(capsys, 1, 1, "flask must have version >= 2.0, found 1.0")
```

### Comparing `appmap-1.9.1/appmap/test/test_django.py` & `appmap-2.0.0/_appmap/test/test_django.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,97 @@
 # flake8: noqa: E402
-# pylint: disable=unused-import, redefined-outer-name, missing-function-docstring
+# pylint: disable=missing-function-docstring,redefined-outer-name
 
 import json
+import os
 import sys
 from pathlib import Path
+from types import SimpleNamespace as NS
 
 import django
-import django.conf
 import django.core.handlers.exception
 import django.db
 import django.http
 import django.test
 import pytest
 from django.template.loader import render_to_string
 from django.test.client import MULTIPART_CONTENT
 
 import appmap
 import appmap.django  # noqa: F401
-from appmap.test.helpers import DictIncluding
+from _appmap.metadata import Metadata
+
+from ..test.helpers import DictIncluding
+from .web_framework import (
+    _TestFormCapture,
+    _TestFormData,
+    _TestRecordRequests,
+    _TestRemoteRecording,
+    _TestRequestCapture,
+)
 
 sys.path += [str(Path(__file__).parent / "data" / "django")]
-import app
 
-from .._implementation.metadata import Metadata
+# Import app just for the side-effects. It must happen after sys.path has been modified.
+# pylint: disable=import-error, unused-import,wrong-import-order,wrong-import-position
+import djangoapp  # pyright: ignore  # noqa: F401
 
-# Make sure assertions in web_framework get rewritten (e.g. to show
-# diffs in generated appmaps)
-pytest.register_assert_rewrite("appmap.test.web_framework")
-from threading import Thread
 
-from .web_framework import (
-    TestRecording,
-    TestRecordRequests,
-    TestRequestCapture,
-    exec_cmd,
-    wait_until_port_is,
-)
+class TestFormCapture(_TestFormCapture):
+    pass
+
+
+class TestFormTest(_TestFormData):
+    pass
+
+
+class TestRecordRequests(_TestRecordRequests):
+    pass
+
+
+class TestRemoteRecording(_TestRemoteRecording):
+    pass
+
+
+class TestRequestCapture(_TestRequestCapture):
+    pass
 
 
 @pytest.mark.django_db
+@pytest.mark.appmap_enabled(appmap_enabled=False)
 def test_sql_capture(events):
     conn = django.db.connections["default"]
     conn.cursor().execute("SELECT 1").fetchall()
-    assert events[0].sql_query == DictIncluding(
-        {"sql": "SELECT 1", "database_type": "sqlite"}
-    )
+    assert events[0].sql_query == DictIncluding({"sql": "SELECT 1", "database_type": "sqlite"})
     assert events[0].sql_query["server_version"].startswith("3.")
-    assert Metadata()["frameworks"] == [
-        {"name": "Django", "version": django.get_version()}
-    ]
+    assert Metadata()["frameworks"] == [{"name": "Django", "version": django.get_version()}]
 
 
-@pytest.mark.appmap_enabled
+# Recording is enabled as a side-effect of requesting the events fixture. There's probably a better
+# way, but leave it here for now.
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
 def test_framework_metadata(client, events):  # pylint: disable=unused-argument
     client.get("/")
-    assert Metadata()["frameworks"] == [
-        {"name": "Django", "version": django.get_version()}
-    ]
+    assert Metadata()["frameworks"] == [{"name": "Django", "version": django.get_version()}]
 
 
-@pytest.mark.appmap_enabled
-def test_app_can_read_body(client, events):  # pylint: disable=unused-argument
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
+def test_app_can_read_body(client):
     response = client.post("/echo", json={"test": "json"})
     assert response.content == b'{"test": "json"}'
 
 
-@pytest.mark.appmap_enabled
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
 def test_template(events):
     render_to_string("hello_world.html")
     assert events[0].to_dict() == DictIncluding(
         {
-            "path": "appmap/test/data/django/app/hello_world.html",
+            "path": "_appmap/test/data/django/djangoapp/hello_world.html",
             "event": "call",
-            "defined_class": "<templates>.AppmapTestDataDjangoAppHello_WorldHtml",
+            "defined_class": "<templates>._AppmapTestDataDjangoDjangoappHello_WorldHtml",
             "method_id": "render",
             "static": False,
         }
     )
 
 
 # pylint: disable=arguments-differ
@@ -89,147 +104,147 @@
         method,
         path,
         data="",
         content_type="application/octet-stream",
         secure=False,
         headers=None,
         json=None,
-        **kwargs
+        **kwargs,
     ):
-        headers = {
-            "HTTP_" + k.replace("-", "_").upper(): v for k, v in (headers or {}).items()
-        }
+        headers = {"HTTP_" + k.replace("-", "_").upper(): v for k, v in (headers or {}).items()}
 
         if json:
             content_type = "application/json"
             data = self._encode_json(json, "application/json")
 
-        return super().generic(
-            method, path, data, content_type, secure, **headers, **kwargs
-        )
+        return super().generic(method, path, data, content_type, secure, **headers, **kwargs)
 
-    def post(
-        self, path, data=None, content_type=MULTIPART_CONTENT, secure=False, **extra
-    ):
+    def post(self, path, data=None, content_type=MULTIPART_CONTENT, secure=False, **extra):
         if content_type == "multipart/form-data":
             content_type = MULTIPART_CONTENT
         return super().post(path, data, content_type, secure, **extra)
 
 
 @pytest.fixture
-def client():
+def client(settings):
+    # We might be able to set DEBUG in the app's settings. But, using the settings fixture here
+    # ensures that all the settings (esp MIDDLEWARE) will be reset before each test run.
+    settings.DEBUG = True
     return ClientAdaptor()
 
 
-@pytest.mark.appmap_enabled
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
 def test_unnamed(client, events):
     client.get("/post/unnamed/5")
 
     assert appmap.enabled()  # sanity check
     # unnamed captures in a re_path don't show up in the event's
     # message attribute.
     assert len(events[0].message) == 0
 
 
-@pytest.mark.appmap_enabled
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
 def test_included_view(client, events):
     client.get("/post/included/test_user")
 
     assert len(events) == 2
     assert events[0].http_server_request == DictIncluding(
         {
             "path_info": "/post/included/test_user",
             "normalized_path_info": "/post/included/{username}",
         }
     )
 
 
-@pytest.mark.appmap_enabled
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
 def test_exception(client, events, monkeypatch):
     def raise_on_call(*args):
         raise RuntimeError("An error")
 
-    monkeypatch.setattr(
-        django.core.handlers.exception, "response_for_exception", raise_on_call
-    )
+    monkeypatch.setattr(django.core.handlers.exception, "response_for_exception", raise_on_call)
 
     with pytest.raises(RuntimeError):
         client.get("/exception")
 
     assert events[0].http_server_request == DictIncluding(
         {"request_method": "GET", "path_info": "/exception", "protocol": "HTTP/1.1"}
     )
 
+    assert events[1].event == "return"
     assert events[1].parent_id == events[0].id
     assert events[1].exceptions == [
         DictIncluding({"class": "builtins.RuntimeError", "message": "An error"})
     ]
 
 
-@pytest.mark.appmap_enabled
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
 def test_deeply_nested_routes(client, events):
     client.get("/admincp/permissions/edit/1")
 
     assert len(events) == 2
     assert events[0].http_server_request == DictIncluding(
         {"normalized_path_info": "/admincp/permissions/edit/{pk}"}
     )
 
 
-def test_middleware_reset(pytester, monkeypatch):
-    monkeypatch.setenv("PYTHONPATH", "init")
-    monkeypatch.setenv("APPMAP", "true")
-
-    pytester.copy_example("django")
-
-    # To really check middleware reset, the tests must run in order,
-    # so disable randomly.
-    pytester.runpytest("-svv", "-p", "no:randomly")
-
-    # Look for the http_server_request event in test_app's appmap. If
-    # middleware reset is broken, it won't be there.
-    appmap_file = pytester.path / "tmp" / "appmap" / "pytest" / "test_app.appmap.json"
-    events = json.loads(appmap_file.read_text())["events"]
-    assert "http_server_request" in events[0]
-
-
-class TestRecordRequestsDjango(TestRecordRequests):
-    @staticmethod
-    def setup_class():
-        TestRecordRequestsDjango.server_stop()  # ensure it's not running
-        TestRecordRequestsDjango.server_start()
-
-    @staticmethod
-    def teardown_class():
-        TestRecordRequestsDjango.server_stop()
-
-    @staticmethod
-    def server_start_thread():
-        exec_cmd(
-            """
-# use appmap from our working copy, not the module installed by virtualenv
-export PYTHONPATH=`pwd`
-
-cd appmap/test/data/django/
-APPMAP=true APPMAP_RECORD_REQUESTS=true APPMAP_OUTPUT_DIR=/tmp python manage.py runserver 127.0.0.1:"""
-            + str(TestRecordRequests.server_port)
-        )
-
-    @staticmethod
-    def server_start():
-        # start as background thread so running the tests can continue
-        thread = Thread(target=TestRecordRequestsDjango.server_start_thread)
-        thread.start()
-        wait_until_port_is("127.0.0.1", TestRecordRequests.server_port, "open")
-
-    @staticmethod
-    def server_stop():
-        exec_cmd(
-            "ps -ef | grep -i 'manage.py runserver' | grep -v grep | awk '{ print $2 }' | xargs kill -9"
-        )
-        wait_until_port_is("127.0.0.1", TestRecordRequests.server_port, "closed")
+class TestDjangoApp:
+    """
+    Run the tests in the fixture app. These depend on being able to manipulate the app's config in
+    ways that are difficult to do from here.
+    """
+
+    @pytest.fixture(autouse=True)
+    def beforeEach(self, monkeypatch, pytester):
+        monkeypatch.setenv("PYTHONPATH", "init")
+        pytester.copy_example("django")
+
+    def test_enabled(self, pytester):
+        # To really check middleware reset, the tests must run in order,
+        # so disable randomly.
+        result = pytester.runpytest("-svv", "-p", "no:randomly")
+        result.assert_outcomes(passed=4, failed=0, errors=0)
+        # Look for the http_server_request event in test_app's appmap. If
+        # middleware reset is broken, it won't be there.
+        appmap_file = pytester.path / "tmp" / "appmap" / "pytest" / "test_request.appmap.json"
+        assert not os.path.exists(pytester.path / "tmp" / "appmap" / "requests")
+
+        events = json.loads(appmap_file.read_text())["events"]
+        assert "http_server_request" in events[0]
+
+    def test_disabled(self, pytester, monkeypatch):
+        monkeypatch.setenv("_APPMAP", "false")
+        result = pytester.runpytest("-svv", "-p", "no:randomly", "-k", "test_request")
+        result.assert_outcomes(passed=1, failed=0, errors=0)
+        assert not (pytester.path / "tmp").exists()
+
+    def test_disabled_for_process(self, pytester, monkeypatch):
+        monkeypatch.setenv("APPMAP_RECORD_PROCESS", "true")
+
+        result = pytester.runpytest("-svv")
+
+        # There are two tests for remote recording. They should both fail,
+        # because process recording should disable remote recording.
+        result.assert_outcomes(passed=2, failed=2, errors=0)
+
+        assert (pytester.path / "tmp" / "appmap" / "process").exists()
+        assert not (pytester.path / "tmp" / "appmap" / "requests").exists()
+        assert not (pytester.path / "tmp" / "appmap" / "pytest").exists()
+
+
+@pytest.fixture(name="server")
+def django_server(xprocess, server_base):
+    debug = server_base.debug
+    host = server_base.host
+    port = server_base.port
+    settings = "settings_dev" if debug else "settings"
+
+    name = "django"
+    pattern = f"server at http://{host}:{port}"
+    cmd = f"manage.py runserver {host}:{port}"
+    env = {"DJANGO_SETTINGS_MODULE": f"djangoapp.{settings}"}
+
+    xprocess.ensure(name, server_base.factory(name, cmd, pattern, env))
 
-    def test_record_request_no_remote(client, events):
-        TestRecordRequests.record_request(client, events, False)
+    url = f"http://{server_base.host}:{port}"
+    yield NS(debug=debug, url=url)
 
-    def test_record_request_and_remote(client, events):
-        TestRecordRequests.record_request(client, events, True)
+    xprocess.getinfo(name).terminate()
```

### Comparing `appmap-1.9.1/appmap/test/test_events.py` & `appmap-2.0.0/_appmap/test/test_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from functools import partial
 from queue import Queue
 from threading import Thread
 
 import pytest
 
 import appmap
-import appmap._implementation
-from appmap._implementation.env import Env
-from appmap._implementation.event import _EventIds
+from _appmap.env import Env
+from _appmap.event import _EventIds
 
 
 # pylint: disable=import-error
 def test_per_thread_id():
     """thread ids should be constant for a  thread"""
     assert _EventIds.get_thread_id() == _EventIds.get_thread_id()
```

### Comparing `appmap-1.9.1/appmap/test/test_http.py` & `appmap-2.0.0/_appmap/test/test_http.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 # pylint: disable=missing-function-docstring,missing-function-docstring,missing-module-docstring
 # pylint: disable=unused-argument,unused-import
 import httpretty
 import pytest
 import requests
 
-import appmap.http
-from appmap.test.helpers import DictIncluding
+import appmap.http  # noqa: F401
+
+from ..test.helpers import DictIncluding
 
 
 def test_http_client_capture(mock_requests, events):
-    requests.get("https://example.test/foo/bar?q=one&q=two&q2=%F0%9F%A6%A0")
+    requests.get("https://example.test/foo/bar?q=one&q=two&q2=%F0%9F%A6%A0", timeout=1)
+
+    assert events[0].to_dict() == DictIncluding(
+        {
+            "event": "call",
+            "defined_class": "http.client.HTTPConnection",
+            "method_id": "request",
+        }
+    )
+    assert events[1].to_dict() == DictIncluding({"event": "return"})
 
-    request = events[0]
+    request = events[2]
     assert request.http_client_request == {
         "request_method": "GET",
         "url": "https://example.test/foo/bar",
         "headers": {"Connection": "keep-alive"},
     }
     message = request.message
     assert message[0] == DictIncluding({"name": "q", "value": "['one', 'two']"})
     assert (message[1] == DictIncluding({"name": "q2", "value": "'🦠'"})) or (
         message[1] == DictIncluding({"name": "q2", "value": "'\\U0001f9a0'"})
     )
 
-    assert events[1].http_client_response == DictIncluding(
+    assert events[3].http_client_response == DictIncluding(
         {"status_code": 200, "mime_type": "text/plain; charset=utf-8"}
     )
 
 
 @pytest.fixture(name="mock_requests")
 def mock_requests_fixture():
     with httpretty.enabled(allow_net_connect=False):
```

### Comparing `appmap-1.9.1/appmap/test/test_params.py` & `appmap-2.0.0/_appmap/test/test_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # pylint: disable=missing-function-docstring
 
 import inspect
 import sys
 
 import pytest
 
-import vendor.wrapt.src.appmap.wrapt as wrapt
-from appmap._implementation.event import CallEvent
-from appmap._implementation.importer import FilterableCls, FilterableFn
+from _appmap import wrapt
+from _appmap.event import CallEvent
+from _appmap.importer import FilterableCls, FilterableFn
 
 empty_args = {"name": "args", "class": "builtins.tuple", "kind": "rest", "value": "()"}
 
 empty_kwargs = {
     "name": "kwargs",
     "class": "builtins.dict",
     "kind": "keyrest",
@@ -254,14 +254,18 @@
             evt,
             1,
             {
                 "name": "kwargs",
                 "class": "builtins.dict",
                 "kind": "keyrest",
                 "size": 2,
+                "properties": [
+                    {"name": "p1", "class": "builtins.int"},
+                    {"name": "p2", "class": "builtins.int"},
+                ],
             },
         )
 
     @pytest.mark.skipif(
         sys.version_info < (3, 8), reason="positional-only added in 3.8"
     )
     @pytest.mark.parametrize("params", ["positional_only"], indirect=True)
```

### Comparing `appmap-1.9.1/appmap/test/test_recording.py` & `appmap-2.0.0/_appmap/test/test_recording.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """Test recording functions called and defined in various ways."""
-# pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring, import-outside-toplevel
 
 import json
 import os
+from distutils.dir_util import copy_tree
+from distutils.file_util import copy_file
 from threading import Thread
 
 import pytest
 
 import appmap
-from appmap._implementation.event import Event
-from appmap._implementation.recorder import Recorder, ThreadRecorder
+from _appmap.event import Event
+from _appmap.recorder import Recorder, ThreadRecorder
+from _appmap.wrapt import FunctionWrapper
 
 from .normalize import normalize_appmap, remove_line_numbers
 
 
 @pytest.mark.appmap_enabled
 @pytest.mark.usefixtures("with_data_dir")
 class TestRecordingWhenEnabled:
     def test_recording_works(self, with_data_dir):
         expected_path = os.path.join(with_data_dir, "expected.appmap.json")
-        with open(expected_path) as f:
+        with open(expected_path, encoding="utf-8") as f:
             expected_appmap = json.load(f)
 
         r = appmap.Recording()
+
         with r:
             from example_class import (  # pyright: ignore[reportMissingImports] pylint: disable=import-error
                 ExampleClass,
             )
 
             ExampleClass.static_method()
             ExampleClass.class_method()
@@ -104,30 +108,41 @@
     def test_can_deepcopy_function(self):
         from copy import deepcopy
 
         from example_class import (  # pyright: ignore[reportMissingImports] pylint: disable=import-error
             modfunc,
         )
 
-        from appmap.wrapt import FunctionWrapper
-
         rec = appmap.Recording()
         with rec:
+            assert isinstance(modfunc, FunctionWrapper)
             f1 = deepcopy(modfunc)
             f1()
 
+    def test_can_pickle(self):
+        import pickle
+
+        from example_class import (  # pyright: ignore[reportMissingImports] pylint: disable=import-error
+            modfunc,
+        )
+
+        rec = appmap.Recording()
+        with rec:
+            assert isinstance(modfunc, FunctionWrapper)
+            f = pickle.loads(pickle.dumps(modfunc))
+            f()
         evt = rec.events[-2]
         assert evt.event == "call"
         assert evt.method_id == "modfunc"
 
 
 @pytest.mark.appmap_enabled
 @pytest.mark.usefixtures("with_data_dir")
 def test_static_cached(events):
-    from example_class import (  # pyright: ignore[reportMissingImports] pylint: disable=import-outside-toplevel,import-error
+    from example_class import (  # pyright: ignore[reportMissingImports] pylint: disable=import-error
         ExampleClass,
     )
 
     ExampleClass.static_cached(42)
     assert (
         events[0].parameters[0].items()
         >= {"name": "value", "class": "builtins.int", "value": "42"}.items()
@@ -151,17 +166,15 @@
 
         def add_event(name):
             r = ThreadRecorder()
             Recorder.set_current(r)
             r.add_event(Event({"name": name}))
             recorders[name] = r
 
-        threads = [
-            Thread(target=add_event, args=(f"thread{i}",)) for i in range(thread_count)
-        ]
+        threads = [Thread(target=add_event, args=(f"thread{i}",)) for i in range(thread_count)]
         for _, t in enumerate(threads):
             t.start()
         for _, t in enumerate(threads):
             t.join()
 
         # Each thread should have gotten a recorder
         assert len(recorders) == thread_count
@@ -170,9 +183,32 @@
         default_events = rec_default.events
         assert len(default_events) == thread_count
 
         # Each event should be added as the first event to the correct recorder
         for n in range(thread_count):
             events = recorders[f"thread{n}"].events
             assert len(events) == 1
-            assert events[0].id == 1
             assert events[0].event["name"] == f"thread{n}"
+
+
+def test_process_recording(data_dir, shell, tmp_path):
+    fixture = data_dir / "package1"
+    tmp = tmp_path / "process"
+    copy_tree(fixture, str(tmp / "package1"))
+    copy_file(data_dir / "appmap.yml", str(tmp))
+    copy_tree(data_dir / "flask" / "init", str(tmp / "init"))
+
+    ret = shell.run(
+        "python",
+        "-m",
+        "package1.package2",
+        env={"PYTHONPATH": "init", "APPMAP_RECORD_PROCESS": "true"},
+        cwd=tmp,
+    )
+    assert ret.returncode == 0
+
+    appmap_dir = tmp / "tmp" / "appmap" / "process"
+    appmap_files = list(appmap_dir.glob("*.appmap.json"))
+    assert len(appmap_files) == 1, "this only fails when run from VS Code?"
+    actual = json.loads(appmap_files[0].read_text())
+    assert len(actual["events"]) > 0
+    assert len(actual["classMap"]) > 0
```

### Comparing `appmap-1.9.1/appmap/test/test_sqlalchemy.py` & `appmap-2.0.0/_appmap/test/test_sqlalchemy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,72 @@
 """Tests for the SQLAlchemy integration."""
 
+from importlib.metadata import version
+
 import pytest
-import sqlalchemy
 from sqlalchemy import (
     Column,
     ForeignKey,
     Integer,
     MetaData,
     String,
     Table,
+    text,
     create_engine,
 )
 
-import appmap.sqlalchemy  # pylint: disable=unused-import
-from appmap.test.helpers import DictIncluding
+import appmap.sqlalchemy  # pylint: disable=unused-import  # noqa: F401
+from _appmap.metadata import Metadata
 
-from .._implementation.metadata import Metadata
+from ..test.helpers import DictIncluding
 from .appmap_test_base import AppMapTestBase
 
 
 class TestSQLAlchemy(AppMapTestBase):
     @staticmethod
     def test_sql_capture(connection, events):
-        connection.execute("SELECT 1")
+        # Passing a string to execute is deprecated in 1.4
+        # and removed in 2.0. We wrap it with text().
+        # https://docs.sqlalchemy.org/en/14/core/connections.html#sqlalchemy.engine.Connection.execute
+        connection.execute(text("SELECT 1"))
         assert events[0].sql_query == DictIncluding(
             {"sql": "SELECT 1", "database_type": "sqlite"}
         )
         assert events[0].sql_query["server_version"].startswith("3.")
         assert Metadata()["frameworks"] == [
-            {"name": "SQLAlchemy", "version": sqlalchemy.__version__}
+            {"name": "SQLAlchemy", "version": version("sqlalchemy")},
         ]
 
     @staticmethod
     # pylint: disable=unused-argument
     def test_capture_ddl(events, schema):
         assert "CREATE TABLE addresses" in events[-2].sql_query["sql"]
 
     # pylint: disable=unused-argument
-    def test_capture_insert(self, connection, schema, events):
+    def test_capture_insert(self, engine, schema, events):
         ins = self.users.insert().values(name="jack", fullname="Jack Jones")
-        connection.execute(ins)
+        with engine.begin() as conn:
+            conn.execute(ins)
         assert (
             events[-2].sql_query["sql"]
             == "INSERT INTO users (name, fullname) VALUES (?, ?)"
         )
 
     # pylint: disable=unused-argument
-    def test_capture_insert_many(self, connection, schema, events):
-        connection.execute(
-            self.addresses.insert(),
-            [
-                {"user_id": 1, "email_address": "jack@yahoo.com"},
-                {"user_id": 1, "email_address": "jack@msn.com"},
-                {"user_id": 2, "email_address": "www@www.org"},
-                {"user_id": 2, "email_address": "wendy@aol.com"},
-            ],
-        )
+    def test_capture_insert_many(self, engine, schema, events):
+        with engine.begin() as conn:
+            conn.execute(
+                self.addresses.insert(),
+                [
+                    {"user_id": 1, "email_address": "jack@yahoo.com"},
+                    {"user_id": 1, "email_address": "jack@msn.com"},
+                    {"user_id": 2, "email_address": "www@www.org"},
+                    {"user_id": 2, "email_address": "wendy@aol.com"},
+                ],
+            )
         assert (
             events[-2].sql_query["sql"]
             == "-- 4 times\nINSERT INTO addresses (user_id, email_address) VALUES (?, ?)"
         )
 
     @staticmethod
     @pytest.fixture
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `appmap-1.9.1/appmap/test/web_framework.py` & `appmap-2.0.0/_appmap/test/web_framework.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,68 @@
 """Common tests for web frameworks such as django and flask."""
 # pylint: disable=missing-function-docstring
 
 import concurrent.futures
 import json
 import multiprocessing
 import os
-import socket
-import subprocess
 import time
-from abc import abstractmethod
+import traceback
 from os.path import exists
+from random import SystemRandom
 
 import pytest
 import requests
 
 import appmap
-from appmap.test.helpers import DictIncluding
+from _appmap.env import Env
 
+from ..test.helpers import DictIncluding, HeadersIncluding
 from .normalize import normalize_appmap
 
+TEST_HOST = "127.0.0.1"
+TEST_PORT = 8000
+
+_SR = SystemRandom()
+
 
 def content_type(res):
     # headers attribute is available in Flask, and in Django as of
     # 3.2. For Django 2.2, headers are accessed from the response
     # directly.
     getter = res.headers.get if hasattr(res, "headers") else res.get
     return getter("Content-Type")
 
 
-@pytest.mark.appmap_enabled
-class TestRequestCapture:
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
+class _TestFormData:
+    @staticmethod
+    @pytest.mark.parametrize("bad_json", ["bad json", 1, False, None, [2, 3]])
+    def test_post_bad_json(events, client, bad_json):
+        client.post(
+            "/test?my_param=example",
+            data=str(bad_json),
+            content_type="application/json",
+        )
+
+        assert events[0].message == [
+            DictIncluding({"name": "my_param", "class": "builtins.str", "value": "'example'"})
+        ]
+
+    @staticmethod
+    def test_post_multipart(events, client):
+        client.post("/test", data={"my_param": "example"}, content_type="multipart/form-data")
+
+        assert events[0].message == [
+            DictIncluding({"name": "my_param", "class": "builtins.str", "value": "'example'"})
+        ]
+
+
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
+class _TestRequestCapture:
     """Common tests for HTTP server request and response capture."""
 
     @staticmethod
     def test_http_capture(client, events):
         """Test GET request and response capture."""
         client.get("/test")
 
@@ -42,15 +71,15 @@
         )
 
         response = events[1].http_server_response
         assert response == DictIncluding(
             {"status_code": 200, "mime_type": "text/html; charset=utf-8"}
         )
 
-        assert "ETag" in response["headers"]
+        assert "etag" in map(str.lower, response["headers"].keys())
 
     @staticmethod
     def test_http_capture_post(client, events):
         """Test POST request with JSON body capture."""
         client.post(
             "/test",
             json={"my_param": "example"},
@@ -67,28 +96,28 @@
                 "path_info": "/test",
                 "protocol": "HTTP/1.1",
                 "authorization": 'token "test-token"',
                 "mime_type": "application/json",
             }
         )
 
-        assert events[0].http_server_request["headers"] == DictIncluding(
+        assert events[0].http_server_request["headers"] == HeadersIncluding(
             {"Accept": "application/json", "Accept-Language": "pl"}
         )
 
     @staticmethod
     def test_post(events, client):
         client.post(
             "/test",
-            data=json.dumps({"my_param": "example"}),
-            content_type="application/json; charset=UTF-8",
+            json={"my_param": "example"},
             headers={
                 "Authorization": 'token "test-token"',
                 "Accept": "application/json",
                 "Accept-Language": "pl",
+                "Content-Type": "application/json; charset=UTF-8",
             },
         )
 
         assert events[0].message == [
             DictIncluding(
                 {"name": "my_param", "class": "builtins.str", "value": "'example'"}
             )
@@ -99,15 +128,15 @@
                 "path_info": "/test",
                 "protocol": "HTTP/1.1",
                 "authorization": 'token "test-token"',
                 "mime_type": "application/json; charset=UTF-8",
             }
         )
 
-        assert events[0].http_server_request["headers"] == DictIncluding(
+        assert events[0].http_server_request["headers"] == HeadersIncluding(
             {"Accept": "application/json", "Accept-Language": "pl"}
         )
 
     @staticmethod
     def test_get(events, client):
         client.get("/test?my_param=example")
 
@@ -128,307 +157,277 @@
                     "class": "builtins.list",
                     "value": "['example', 'example2']",
                 }
             ),
         ]
 
     @staticmethod
-    def test_post_form_urlencoded(events, client):
-        client.post(
-            "/test",
-            data="my_param=example",
-            content_type="application/x-www-form-urlencoded",
-        )
-
-        assert events[0].message == [
-            DictIncluding(
-                {"name": "my_param", "class": "builtins.str", "value": "'example'"}
-            )
-        ]
-
-    @staticmethod
     def test_put(events, client):
         client.put("/test", json={"my_param": "example"})
 
         assert events[0].message == [
             DictIncluding(
                 {"name": "my_param", "class": "builtins.str", "value": "'example'"}
             )
         ]
 
     @staticmethod
-    def test_post_bad_json(events, client):
-        client.post(
-            "/test?my_param=example", data="bad json", content_type="application/json"
-        )
-
-        assert events[0].message == [
-            DictIncluding(
-                {"name": "my_param", "class": "builtins.str", "value": "'example'"}
-            )
-        ]
-
-    @staticmethod
-    def test_post_multipart(events, client):
-        client.post(
-            "/test", data={"my_param": "example"}, content_type="multipart/form-data"
-        )
-
-        assert events[0].message == [
-            DictIncluding(
-                {"name": "my_param", "class": "builtins.str", "value": "'example'"}
-            )
-        ]
-
-    @staticmethod
     def test_post_with_query(events, client):
-        client.post("/test?my_param=get", data={"my_param": "example"})
+        client.post("/test?my_param=get&my_param=an", json={"my_param": "example"})
 
         assert events[0].message == [
             DictIncluding(
                 {
                     "name": "my_param",
                     "class": "builtins.list",
-                    "value": "['get', 'example']",
+                    "value": "['get', 'an', 'example']",
                 }
             )
         ]
 
     @staticmethod
     @pytest.mark.parametrize(
         "url,expected",
         [
             ("/user/test_user", "/user/{username}"),
             ("/post/123", "/post/{post_id}"),
             ("/post/test_user/123/summary", "/post/{username}/{post_id}/summary"),
+            ("/123/posts/test_user", "/{org}/posts/{username}"),
         ],
     )
     def test_path_normalization(client, events, url, expected):
         client.get(url)
         np = events[0].http_server_request["normalized_path_info"]
         assert np == expected
 
     @staticmethod
-    @pytest.mark.appmap_enabled
     def test_message_path_segments(events, client):
         client.get("/post/alice/42/summary")
 
         assert events[0].message == [
             DictIncluding(
                 {"name": "username", "class": "builtins.str", "value": "'alice'"}
             ),
             DictIncluding({"name": "post_id", "class": "builtins.int", "value": "42"}),
         ]
 
 
-class TestRecording:
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
+class _TestFormCapture:
+    @staticmethod
+    def test_post_form_urlencoded(events, client):
+        client.post(
+            "/test",
+            data="my_param=example",
+            content_type="application/x-www-form-urlencoded",
+        )
+
+        assert events[0].message == [
+            DictIncluding({"name": "my_param", "class": "builtins.str", "value": "'example'"})
+        ]
+
+    @staticmethod
+    def test_post_multipart(events, client):
+        client.post("/test", data={"my_param": "example"}, content_type="multipart/form-data")
+
+        assert events[0].message == [
+            DictIncluding({"name": "my_param", "class": "builtins.str", "value": "'example'"})
+        ]
+
+
+@pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REQUESTS": "false"})
+class _TestRemoteRecording:
     """Common tests for remote recording."""
 
+    @property
+    def expected_content_type(self):
+        return self._expected_content_type
+
+    @expected_content_type.setter
+    def expected_content_type(self, value):
+        self._expected_content_type = value
+
+    def setup_method(self):
+        self.expected_content_type = "text/html; charset=utf-8"
+
     @staticmethod
+    # since APPMAP records by default, disable it explicitly
+    @pytest.mark.appmap_enabled(appmap_enabled=False)
     def test_appmap_disabled(client):
         assert not appmap.enabled()
+        assert not Env.current.enables("remote")
 
         res = client.get("/_appmap/record")
         assert res.status_code == 404
 
     @staticmethod
-    @pytest.mark.appmap_enabled
     def test_starts_disabled(client):
         res = client.get("/_appmap/record")
         assert res.status_code == 200
 
         assert content_type(res) == "application/json"
 
         data = res.json
         if callable(data):
             data = data()
         assert data == {"enabled": False}
 
     @staticmethod
-    @pytest.mark.appmap_enabled
     def test_can_be_enabled(client):
         res = client.post("/_appmap/record")
         assert res.status_code == 200
 
     @staticmethod
-    @pytest.mark.appmap_enabled
     def test_can_only_enable_once(client):
         res = client.post("/_appmap/record")
         assert res.status_code == 200
         res = client.post("/_appmap/record")
         assert res.status_code == 409
 
-    @staticmethod
-    @pytest.mark.appmap_enabled
-    def test_can_record(data_dir, client):
+    def test_can_record(self, data_dir, client):
         res = client.post("/_appmap/record")
         assert res.status_code == 200
 
         res = client.get("/")
         assert res.status_code == 200
+        assert res.headers["content-type"] == self.expected_content_type
 
         res = client.get("/user/test_user")
         assert res.status_code == 200
+        assert res.headers["content-type"] == self.expected_content_type
 
         res = client.delete("/_appmap/record")
         assert res.status_code == 200
         assert content_type(res) == "application/json"
         data = res.data if hasattr(res, "data") else res.content
         generated_appmap = normalize_appmap(data)
 
+        for evt in generated_appmap["events"]:
+            # Strip out thread id. The values for these vary by framework, and
+            # may not even be the same within an AppMap (e.g. FastAPI). They
+            # should always be ints, though
+            if "thread_id" in evt:
+                value = evt.pop("thread_id")
+                assert isinstance(value, int)
+
+            # Check mime_type. These also vary by framework, but will be
+            # consistent within an AppMap.
+            if "http_server_response" in evt:
+                actual_content_type = evt["http_server_response"].pop("mime_type")
+                assert actual_content_type == self.expected_content_type
+
         expected_path = data_dir / "remote.appmap.json"
-        with open(expected_path) as expected:
+        with open(expected_path, encoding="utf-8") as expected:
             expected_appmap = json.load(expected)
 
-        assert (
-            generated_appmap == expected_appmap
-        ), f"expected appmap path {expected_path}"
-
+        assert generated_appmap == expected_appmap, f"expected appmap path {expected_path}"
         res = client.delete("/_appmap/record")
         assert res.status_code == 404
 
-
-def exec_cmd(command):
-    p = subprocess.Popen(
-        command,
-        shell=True,
-        stdout=subprocess.PIPE,
-        stdin=subprocess.PIPE,
-        stderr=subprocess.STDOUT,
-    )
-    output, errors = p.communicate()
-    return output.decode()
-
-
-def port_state(address, port):
-    ret = None
-    s = socket.socket()
-    try:
-        s.connect((address, port))
-        ret = "open"
-    except:
-        ret = "closed"
-        s.close()
-    return ret
-
-
-def wait_until_port_is(address, port, desired_state):
-    max_wait_seconds = 10
-    sleep_time = 0.1
-    max_count = 1 / sleep_time * max_wait_seconds
-    count = 0
-    # don't "while True" to not lock-up the testsuite if something goes wrong
-    while count < max_count:
-        current_state = port_state(address, port)
-        if current_state == desired_state:
-            break
-        else:
-            time.sleep(sleep_time)
-
-
-class TestRecordRequests:
+class _TestRecordRequests:
     """Common tests for per-requests recording (record requests.)"""
 
-    server_port = 8000
-
-    @abstractmethod
-    def server_start():
-        """
-        Start the webserver in the background. Don't block execution.
-        """
-
-    @abstractmethod
-    def server_stop():
-        """
-        Stop the webserver.
-        """
-
-    def server_url():
-        return "http://127.0.0.1:" + str(TestRecordRequests.server_port)
-
-    @staticmethod
-    def record_request_thread():
-        return requests.get(TestRecordRequests.server_url() + "/test")
-
-    @staticmethod
-    @pytest.mark.appmap_enabled
-    @pytest.mark.appmap_record_requests
-    def record_request(
-        client, events, record_remote
-    ):  # pylint: disable=unused-argument
+    @classmethod
+    def server_url(cls):
+        return f"http://{TEST_HOST}:{TEST_PORT}"
+
+    @classmethod
+    def record_request_thread(cls):
+        # I've seen occasional test failures, seemingly because the test servers can't handle the
+        # barrage of requests. A tiny bit of delay still causes many, many concurrent requests, but
+        # eliminates the failures.
+        time.sleep(_SR.uniform(0, 0.1))
+        return requests.get(cls.server_url() + "/test", timeout=30)
 
+    def record_requests(self, record_remote):
+        # pylint: disable=too-many-locals
         if record_remote:
             # when remote recording is enabled, this test also
             # verifies the global recorder doesn't save duplicate
             # events when per-request recording is enabled
-            response = requests.post(
-                TestRecordRequests.server_url() + "/_appmap/record"
-            )
+            response = requests.post(self.server_url() + "/_appmap/record", timeout=30)
             assert response.status_code == 200
 
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=multiprocessing.cpu_count()
         ) as executor:
             # start all threads
             max_number_of_threads = 400
             future_to_request_number = {}
             for n in range(max_number_of_threads):
-                future = executor.submit(TestRecordRequests.record_request_thread)
+                future = executor.submit(self.record_request_thread)
                 future_to_request_number[future] = n
 
             # wait for all threads to complete
             for future in concurrent.futures.as_completed(future_to_request_number):
                 try:
                     response = future.result()
-                except Exception as e:
-                    print("%r generated an exception: %s" % (e))
-
+                except Exception:  # pylint: disable=broad-except
+                    traceback.print_exc()
                 assert response.status_code == 200
 
                 if hasattr(response, "content"):
                     # django uses response.content
                     assert response.content == b"testing"
                 else:
                     # flask  uses response.get_data
                     assert response.get_data() == b"testing"
 
                 if hasattr(response, "headers"):
-                    assert response.headers["AppMap-File-Name"]
+                    assert "AppMap-File-Name" in response.headers
                     appmap_file_name = response.headers["AppMap-File-Name"]
                 else:
                     # response.headers doesn't exist in Django 2.2
-                    assert response["AppMap-File-Name"]
+                    assert "AppMap-File-Name" in response
                     appmap_file_name = response["AppMap-File-Name"]
                 assert exists(appmap_file_name)
                 appmap_file_name_basename = appmap_file_name.split("/")[-1]
                 appmap_file_name_basename_part = "_".join(
                     appmap_file_name_basename.split("_")[2:]
                 )
                 assert (
                     appmap_file_name_basename_part
                     == "http_127_0_0_1_8000_test.appmap.json"
                 )
 
-                with open(appmap_file_name) as f:
-                    appmap = json.loads(f.read())
+                with open(appmap_file_name, encoding="utf-8") as f:
+                    recording = json.loads(f.read())
 
                     # Every event should come from the same thread
                     thread_ids = {
-                        event["thread_id"]: True for event in appmap["events"]
+                        event["thread_id"]: True for event in recording["events"]
                     }
                     assert len(thread_ids) == 1
 
                     # AppMap should contain only one request and response
                     http_server_requests = [
-                        event["http_server_request"]
-                        for event in appmap["events"]
-                        if "http_server_request" in event
+                        event for event in recording["events"] if "http_server_request" in event
                     ]
                     http_server_responses = [
-                        event["http_server_response"]
-                        for event in appmap["events"]
-                        if "http_server_response" in event
+                        event for event in recording["events"] if "http_server_response" in event
                     ]
                     assert len(http_server_requests) == 1
                     assert len(http_server_responses) == 1
+                    assert http_server_responses[0]["parent_id"] == http_server_requests[0]["id"]
 
                 os.remove(appmap_file_name)
+
+    @pytest.mark.appmap_enabled
+    @pytest.mark.server(debug=True)
+    def test_record_requests_with_remote(self, server):
+        self.record_requests(server.debug)
+
+    @pytest.mark.appmap_enabled
+    @pytest.mark.server(debug=False)
+    def test_record_requests_without_remote(self, server):
+        self.record_requests(server.debug)
+
+    @pytest.mark.server(debug=False)
+    def test_remote_disabled_in_prod(self, server):
+        response = requests.get(server.url + "/_appmap/record", timeout=30)
+        assert response.status_code == 404
+
+    @pytest.mark.server(debug=False, env={"APPMAP_RECORD_REMOTE": "true"})
+    @pytest.mark.appmap_enabled(env={"APPMAP_RECORD_REMOTE": "true"})
+    def test_remote_enabled_in_prod(self, server):
+        response = requests.get(server.url + "/_appmap/record", timeout=30)
+        assert response.status_code == 200
```

### Comparing `appmap-1.9.1/pyproject.toml` & `appmap-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,122 @@
 [tool.poetry]
 name = "appmap"
-version = "1.9.1"
+version = "2.0.0"
 description = "Create AppMap files by recording a Python application."
 readme = "README.md"
 authors = [
   "Alan Potter <alan@app.land>",
   "Viraj Kanwade <viraj.kanwade@forgeahead.io>",
   "Rafał Rzepecki <rafal@app.land>"
 ]
 homepage = "https://github.com/applandinc/appmap-python"
 license = "MIT"
 classifiers = [
         'Development Status :: 4 - Beta',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.1',
+        'Framework :: Django :: 3.2',
         'Framework :: Flask',
         'Framework :: Pytest',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Software Development :: Debuggers',
         'Topic :: Software Development :: Documentation'
 ]
-include = ['appmap.pth']
+
+include = [
+    { path = 'appmap.pth', format = ['sdist','wheel'] },
+    { path = '_appmap/test/**/*', format = 'sdist' }
+]
+
+exclude = ['_appmap/wrapt']
 
 packages = [
     { include = "appmap" },
-    { include = "appmap/wrapt/*.py", from="vendor/wrapt/src" }
+    { include = "_appmap/*.py" },
+    { include = "_appmap/wrapt/**/*", from = "vendor" }
 ]
 
 [tool.poetry.dependencies]
 # Please update the documentation if changing the supported python version
 # https://github.com/applandinc/applandinc.github.io/blob/master/_docs/reference/appmap-python.md#supported-versions
-python = "^3.7"
-PyYAML = "^5.3.0"
+python = "^3.8"
+PyYAML = ">=5.3.0"
 inflection = ">=0.3.0"
-importlib-metadata = ">=0.8"
 importlib-resources = "^5.4.0"
-packaging = "^21.3"
-# If you include "Django" as an optional dependency here, you'll be able to use
-# poetry to install it in your dev environment. However, doing so causes poetry
-# v1.2.0 to remove it from the virtualenv *created and managed by tox*, i.e. not
-# your dev environment. 
-# 
-# So, if you'd like to run the tests outside of tox,
-# you'll need to `pip install` the appropriate version of Django, e.g.
-#   pip install django'>=3.2,<4.0'
-#   pip install pytest-django
+packaging = ">=19.0"
+# If you include "Django" as an optional dependency here, you'll be able to use poetry to install it
+# in your dev environment. However, doing so causes poetry v1.2.0 to remove it from the virtualenv
+# *created and managed by tox*, i.e. not your dev environment.
+#
+# So, if you'd like to run the tests outside of tox, run `pip install -r requirements-dev.txt` to
+# install it and the rest of the dev dependencies.
 
-[tool.poetry.dev-dependencies]
-httpretty = "^1.0.5"
-pytest = "^6.1.2"
-pytest-randomly = "^3.5.0"
-pylint = "^2.6.0"
+[tool.poetry.group.dev.dependencies]
+Twisted = "^22.4.0"
+asgiref = "^3.7.2"
+black = "^24.2.0"
+coverage = "^5.3"
 flake8 = "^3.8.4"
-pyfakefs = "^4.3.2"
+httpretty = "^1.0.5"
+isort = "^5.10.1"
 pprintpp = ">=0.4.0"
-coverage = "^5.3"
+pyfakefs = "^5.3.5"
+pylint = "^3.0"
+pytest = "^7.3.2"
+pytest-django = "~4.7"
 pytest-mock = "^3.5.1"
-flask = "^1.1.2"
-MarkupSafe = "2.0.1"
-jinja2 = ">=2.10.1,<3"
-itsdangerous = ">=0.24,<2"
-Werkzeug = ">=0.15,<2"
-SQLAlchemy = { version = "^1.4.11", python = "^3.7"}
-tox = "^3.22.0"
-tox-pyenv = "^1.1.0"
-tox-travis = ">=0.12"
-Twisted = "^22.4.0"
-requests = "^2.25.1"
+pytest-randomly = "^3.5.0"
+pytest-shell-utilities = "^1.8.0"
+pytest-xprocess = "^0.23.0"
 python-decouple = "^3.5"
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.8.0"
-isort = "^5.10.1"
+requests = "^2.25.1"
+tox = "^3.22.0"
+# v2.30.0 of "requests" depends on urllib3 v2, which breaks the tests for http_client_requests. Pin
+# to v1 until this gets fixed.
+urllib3 = "^1"
+uvicorn = "^0.27.1"
+fastapi = "^0.110.0"
+httpx = "^0.27.0"
+pytest-env = "^1.1.3"
+pytest-console-scripts = "^1.4.1"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."pytest11"]
 appmap = "appmap.pytest"
 
 [tool.poetry.scripts]
 appmap-agent-init = "appmap.command.appmap_agent_init:run"
 appmap-agent-status = "appmap.command.appmap_agent_status:run"
 appmap-agent-validate = "appmap.command.appmap_agent_validate:run"
+appmap-python = "appmap.command.runner:run"
 
 [tool.black]
+line-length = 102
 extend-exclude = '''
 /(
   | vendor
-  | appmap/wrapt
+  | _appmap/wrapt
 )/
 '''
 
 [tool.isort]
 profile = "black"
 extend_skip = [
   "vendor",
-  "appmap/wrapt"
+  "_appmap/wrapt"
   ]
 
+[tool.vendoring]
+destination = "vendor/_appmap/"
+requirements = "vendor/vendor.txt"
+namespace = ""
+
+protected-files = ["vendor.txt"]
+patches-dir = "vendor/patches"
+
+[tool.vendoring.transformations]
+drop = [
+    "**/*.so",
+]
```

### Comparing `appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/decorators.py` & `appmap-2.0.0/vendor/_appmap/wrapt/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 
     import builtins
 
     exec_ = getattr(builtins, "exec")
     del builtins
 
 from functools import partial
-from inspect import ismethod, isclass, formatargspec
-from collections import namedtuple
+from inspect import isclass
 from threading import Lock, RLock
 
+from .arguments import formatargspec
+
 try:
     from inspect import signature
 except ImportError:
     pass
 
 from .wrappers import (FunctionWrapper, BoundFunctionWrapper, ObjectProxy,
     CallableObjectProxy)
@@ -169,57 +170,80 @@
 # Decorator for creating other decorators. This decorator and the
 # wrappers which they use are designed to properly preserve any name
 # attributes, function signatures etc, in addition to the wrappers
 # themselves acting like a transparent proxy for the original wrapped
 # function so the wrapper is effectively indistinguishable from the
 # original wrapped function.
 
-def decorator(wrapper=None, enabled=None, adapter=None):
+def decorator(wrapper=None, enabled=None, adapter=None, proxy=FunctionWrapper):
     # The decorator should be supplied with a single positional argument
     # which is the wrapper function to be used to implement the
     # decorator. This may be preceded by a step whereby the keyword
     # arguments are supplied to customise the behaviour of the
     # decorator. The 'adapter' argument is used to optionally denote a
     # separate function which is notionally used by an adapter
     # decorator. In that case parts of the function '__code__' and
     # '__defaults__' attributes are used from the adapter function
     # rather than those of the wrapped function. This allows for the
-    # argument specification from inspect.getargspec() and similar
+    # argument specification from inspect.getfullargspec() and similar
     # functions to be overridden with a prototype for a different
     # function than what was wrapped. The 'enabled' argument provides a
     # way to enable/disable the use of the decorator. If the type of
     # 'enabled' is a boolean, then it is evaluated immediately and the
     # wrapper not even applied if it is False. If not a boolean, it will
     # be evaluated when the wrapper is called for an unbound wrapper,
     # and when binding occurs for a bound wrapper. When being evaluated,
     # if 'enabled' is callable it will be called to obtain the value to
     # be checked. If False, the wrapper will not be called and instead
     # the original wrapped function will be called directly instead.
+    # The 'proxy' argument provides a way of passing a custom version of
+    # the FunctionWrapper class used in decorating the function.
 
     if wrapper is not None:
         # Helper function for creating wrapper of the appropriate
         # time when we need it down below.
 
         def _build(wrapped, wrapper, enabled=None, adapter=None):
             if adapter:
                 if isinstance(adapter, AdapterFactory):
                     adapter = adapter(wrapped)
 
                 if not callable(adapter):
                     ns = {}
+
+                    # Check if the signature argument specification has
+                    # annotations. If it does then we need to remember
+                    # it but also drop it when attempting to manufacture
+                    # a standin adapter function. This is necessary else
+                    # it will try and look up any types referenced in
+                    # the annotations in the empty namespace we use,
+                    # which will fail.
+
+                    annotations = {}
+
                     if not isinstance(adapter, string_types):
+                        if len(adapter) == 7:
+                            annotations = adapter[-1]
+                            adapter = adapter[:-1]
                         adapter = formatargspec(*adapter)
+
                     exec_('def adapter{}: pass'.format(adapter), ns, ns)
                     adapter = ns['adapter']
 
+                    # Override the annotations for the manufactured
+                    # adapter function so they match the original
+                    # adapter signature argument specification.
+
+                    if annotations:
+                        adapter.__annotations__ = annotations
+
                 return AdapterWrapper(wrapped=wrapped, wrapper=wrapper,
                         enabled=enabled, adapter=adapter)
 
-            return FunctionWrapper(wrapped=wrapped, wrapper=wrapper,
-                    enabled=enabled)
+            return proxy(wrapped=wrapped, wrapper=wrapper, enabled=enabled)
 
         # The wrapper has been provided so return the final decorator.
         # The decorator is itself one of our function wrappers so we
         # can determine when it is applied to functions, instance methods
         # or class methods. This allows us to bind the instance or class
         # method so the appropriate self or cls attribute is supplied
         # when it is finally called.
@@ -356,15 +380,15 @@
                     #     @instance.decoratorclassmethod
                     #     def function():
                     #         pass
                     #
                     # This one is a bit strange because binding was actually
                     # performed on the wrapper created by our decorator
                     # factory. We need to apply that binding to the decorator
-                    # wrapper function which which the decorator factory
+                    # wrapper function that the decorator factory
                     # was applied to.
 
                     target_wrapper = wrapper.__get__(None, instance)
 
                 else:
                     # In this case the decorator was applied to an instance
                     # method.
@@ -380,15 +404,15 @@
                     #     @instance.decoratorclassmethod
                     #     def function():
                     #         pass
                     #
                     # This one is a bit strange because binding was actually
                     # performed on the wrapper created by our decorator
                     # factory. We need to apply that binding to the decorator
-                    # wrapper function which which the decorator factory
+                    # wrapper function that the decorator factory
                     # was applied to.
 
                     target_wrapper = wrapper.__get__(instance, type(instance))
 
             # Finally build the wrapper itself and return it.
 
             return _build(target_wrapped, target_wrapper, _enabled, adapter)
@@ -404,15 +428,16 @@
 
     else:
         # The wrapper still has not been provided, so we are just
         # collecting the optional keyword arguments. Return the
         # decorator again wrapped in a partial using the collected
         # arguments.
 
-        return partial(decorator, enabled=enabled, adapter=adapter)
+        return partial(decorator, enabled=enabled, adapter=adapter,
+                proxy=proxy)
 
 # Decorator for implementing thread synchronization. It can be used as a
 # decorator, in which case the synchronization context is determined by
 # what type of function is wrapped, or it can also be used as a context
 # manager, where the user needs to supply the correct synchronization
 # context. It is also possible to supply an object which appears to be a
 # synchronization primitive of some sort, by virtue of having release()
```

### Comparing `appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/importer.py` & `appmap-2.0.0/vendor/_appmap/wrapt/importer.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 import sys
 import threading
 
 PY2 = sys.version_info[0] == 2
 
 if PY2:
     string_types = basestring,
+    find_spec = None
 else:
-    import importlib
     string_types = str,
-
-from .decorators import synchronized
+    from importlib.util import find_spec
 
 # The dictionary registering any post import hooks to be triggered once
 # the target module has been imported. Once a module has been imported
 # and the hooks fired, the list of hooks recorded against the target
-# module will be truncacted but the list left in the dictionary. This
+# module will be truncated but the list left in the dictionary. This
 # acts as a flag to indicate that the module had already been imported.
 
 _post_import_hooks = {}
 _post_import_hooks_init = False
 _post_import_hooks_lock = threading.RLock()
 
 # Register a new post import hook for the target module name. This
@@ -40,66 +39,46 @@
         __import__(module_name)
         callback = sys.modules[module_name]
         for attr in attrs:
             callback = getattr(callback, attr)
         return callback(module)
     return import_hook
 
-@synchronized(_post_import_hooks_lock)
 def register_post_import_hook(hook, name):
     # Create a deferred import hook if hook is a string name rather than
     # a callable function.
 
     if isinstance(hook, string_types):
         hook = _create_import_hook_from_string(hook)
 
-    # Automatically install the import hook finder if it has not already
-    # been installed.
-
-    global _post_import_hooks_init
+    with _post_import_hooks_lock:
+        # Automatically install the import hook finder if it has not already
+        # been installed.
+
+        global _post_import_hooks_init
+
+        if not _post_import_hooks_init:
+            _post_import_hooks_init = True
+            sys.meta_path.insert(0, ImportHookFinder())
 
-    if not _post_import_hooks_init:
-        _post_import_hooks_init = True
-        sys.meta_path.insert(0, ImportHookFinder())
-
-    # Determine if any prior registration of a post import hook for
-    # the target modules has occurred and act appropriately.
-
-    hooks = _post_import_hooks.get(name, None)
-
-    if hooks is None:
-        # No prior registration of post import hooks for the target
-        # module. We need to check whether the module has already been
-        # imported. If it has we fire the hook immediately and add an
-        # empty list to the registry to indicate that the module has
-        # already been imported and hooks have fired. Otherwise add
-        # the post import hook to the registry.
+        # Check if the module is already imported. If not, register the hook
+        # to be called after import.
 
         module = sys.modules.get(name, None)
 
-        if module is not None:
-            _post_import_hooks[name] = []
-            hook(module)
-
-        else:
-            _post_import_hooks[name] = [hook]
-
-    elif hooks == []:
-        # A prior registration of port import hooks for the target
-        # module was done and the hooks already fired. Fire the hook
-        # immediately.
-
-        module = sys.modules[name]
-        hook(module)
+        if module is None:
+            _post_import_hooks.setdefault(name, []).append(hook)
 
-    else:
-        # A prior registration of port import hooks for the target
-        # module was done but the module has not yet been imported.
+    # If the module is already imported, we fire the hook right away. Note that
+    # the hook is called outside of the lock to avoid deadlocks if code run as a
+    # consequence of calling the module import hook in turn triggers a separate
+    # thread which tries to register an import hook.
 
-        _post_import_hooks[name].append(hook)
+    if module is not None:
+        hook(module)
 
 # Register post import hooks defined as package entry points.
 
 def _create_import_hook_from_entrypoint(entrypoint):
     def import_hook(module):
         __import__(entrypoint.module_name)
         callback = sys.modules[entrypoint.module_name]
@@ -119,24 +98,26 @@
         register_post_import_hook(callback, entrypoint.name)
 
 # Indicate that a module has been loaded. Any post import hooks which
 # were registered against the target module will be invoked. If an
 # exception is raised in any of the post import hooks, that will cause
 # the import of the target module to fail.
 
-@synchronized(_post_import_hooks_lock)
 def notify_module_loaded(module):
     name = getattr(module, '__name__', None)
-    hooks = _post_import_hooks.get(name, None)
 
-    if hooks:
-        _post_import_hooks[name] = []
+    with _post_import_hooks_lock:
+        hooks = _post_import_hooks.pop(name, ())
 
-        for hook in hooks:
-            hook(module)
+    # Note that the hook is called outside of the lock to avoid deadlocks if
+    # code run as a consequence of calling the module import hook in turn
+    # triggers a separate thread which tries to register an import hook.
+
+    for hook in hooks:
+        hook(module)
 
 # A custom module import finder. This intercepts attempts to import
 # modules and watches out for attempts to import target modules of
 # interest. When a module of interest is imported, then any post import
 # hooks which are registered will be invoked.
 
 class _ImportHookLoader:
@@ -148,33 +129,76 @@
         return module
 
 class _ImportHookChainedLoader:
 
     def __init__(self, loader):
         self.loader = loader
 
-    def load_module(self, fullname):
+        if hasattr(loader, "load_module"):
+          self.load_module = self._load_module
+        if hasattr(loader, "create_module"):
+          self.create_module = self._create_module
+        if hasattr(loader, "exec_module"):
+          self.exec_module = self._exec_module
+
+    def _set_loader(self, module):
+        # Set module's loader to self.loader unless it's already set to
+        # something else. Import machinery will set it to spec.loader if it is
+        # None, so handle None as well. The module may not support attribute
+        # assignment, in which case we simply skip it. Note that we also deal
+        # with __loader__ not existing at all. This is to future proof things
+        # due to proposal to remove the attribue as described in the GitHub
+        # issue at https://github.com/python/cpython/issues/77458. Also prior
+        # to Python 3.3, the __loader__ attribute was only set if a custom
+        # module loader was used. It isn't clear whether the attribute still
+        # existed in that case or was set to None.
+
+        class UNDEFINED: pass
+
+        if getattr(module, "__loader__", UNDEFINED) in (None, self):
+            try:
+                module.__loader__ = self.loader
+            except AttributeError:
+                pass
+
+        if (getattr(module, "__spec__", None) is not None
+                and getattr(module.__spec__, "loader", None) is self):
+            module.__spec__.loader = self.loader
+
+    def _load_module(self, fullname):
         module = self.loader.load_module(fullname)
+        self._set_loader(module)
         notify_module_loaded(module)
 
         return module
 
+    # Python 3.4 introduced create_module() and exec_module() instead of
+    # load_module() alone. Splitting the two steps.
+
+    def _create_module(self, spec):
+        return self.loader.create_module(spec)
+
+    def _exec_module(self, module):
+        self._set_loader(module)
+        self.loader.exec_module(module)
+        notify_module_loaded(module)
+
 class ImportHookFinder:
 
     def __init__(self):
         self.in_progress = {}
 
-    @synchronized(_post_import_hooks_lock)
     def find_module(self, fullname, path=None):
         # If the module being imported is not one we have registered
         # post import hooks for, we can return immediately. We will
         # take no further part in the importing of this module.
 
-        if not fullname in _post_import_hooks:
-            return None
+        with _post_import_hooks_lock:
+            if fullname not in _post_import_hooks:
+                return None
 
         # When we are interested in a specific module, we will call back
         # into the import system a second time to defer to the import
         # finder that is supposed to handle the importing of the module.
         # We set an in progress flag for the target module so that on
         # the second time through we don't trigger another call back
         # into the import system and cause a infinite loop.
@@ -183,15 +207,15 @@
             return None
 
         self.in_progress[fullname] = True
 
         # Now call back into the import system again.
 
         try:
-            if PY2:
+            if not find_spec:
                 # For Python 2 we don't have much choice but to
                 # call back in to __import__(). This will
                 # actually cause the module to be imported. If no
                 # module could be found then ImportError will be
                 # raised. Otherwise we return a loader which
                 # returns the already loaded module and invokes
                 # the post import hooks.
@@ -204,22 +228,61 @@
                 # For Python 3 we need to use find_spec().loader
                 # from the importlib.util module. It doesn't actually
                 # import the target module and only finds the
                 # loader. If a loader is found, we need to return
                 # our own loader which will then in turn call the
                 # real loader to import the module and invoke the
                 # post import hooks.
-                try:
-                    import importlib.util
-                    loader = importlib.util.find_spec(fullname).loader
-                except (ImportError, AttributeError):
-                    loader = importlib.find_loader(fullname, path)
-                if loader:
+
+                loader = getattr(find_spec(fullname), "loader", None)
+
+                if loader and not isinstance(loader, _ImportHookChainedLoader):
                     return _ImportHookChainedLoader(loader)
 
+        finally:
+            del self.in_progress[fullname]
+
+    def find_spec(self, fullname, path=None, target=None):
+        # Since Python 3.4, you are meant to implement find_spec() method
+        # instead of find_module() and since Python 3.10 you get deprecation
+        # warnings if you don't define find_spec().
+
+        # If the module being imported is not one we have registered
+        # post import hooks for, we can return immediately. We will
+        # take no further part in the importing of this module.
+
+        with _post_import_hooks_lock:
+            if fullname not in _post_import_hooks:
+                return None
+
+        # When we are interested in a specific module, we will call back
+        # into the import system a second time to defer to the import
+        # finder that is supposed to handle the importing of the module.
+        # We set an in progress flag for the target module so that on
+        # the second time through we don't trigger another call back
+        # into the import system and cause a infinite loop.
+
+        if fullname in self.in_progress:
+            return None
+
+        self.in_progress[fullname] = True
+
+        # Now call back into the import system again.
+
+        try:
+            # This should only be Python 3 so find_spec() should always
+            # exist so don't need to check.
+
+            spec = find_spec(fullname)
+            loader = getattr(spec, "loader", None)
+
+            if loader and not isinstance(loader, _ImportHookChainedLoader):
+                spec.loader = _ImportHookChainedLoader(loader)
+
+            return spec
 
         finally:
             del self.in_progress[fullname]
 
 # Decorator for marking that a function should be called as a post
 # import hook when the target module is imported.
```

### Comparing `appmap-1.9.1/vendor/wrapt/src/appmap/wrapt/wrappers.py` & `appmap-2.0.0/vendor/_appmap/wrapt/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,22 @@
         # be an actual string object instead.
 
         try:
             object.__setattr__(self, '__qualname__', wrapped.__qualname__)
         except AttributeError:
             pass
 
+        # Python 3.10 onwards also does not allow itself to be overridden
+        # using a property and it must instead be set explicitly.
+
+        try:
+            object.__setattr__(self, '__annotations__', wrapped.__annotations__)
+        except AttributeError:
+            pass
+
     @property
     def __name__(self):
         return self.__wrapped__.__name__
 
     @__name__.setter
     def __name__(self, value):
         self.__wrapped__.__name__ = value
@@ -104,22 +112,14 @@
     def __class__(self):
         return self.__wrapped__.__class__
 
     @__class__.setter
     def __class__(self, value):
         self.__wrapped__.__class__ = value
 
-    @property
-    def __annotations__(self):
-        return self.__wrapped__.__annotations__
-
-    @__annotations__.setter
-    def __annotations__(self, value):
-        self.__wrapped__.__annotations__ = value
-
     def __dir__(self):
         return dir(self.__wrapped__)
 
     def __str__(self):
         return str(self.__wrapped__)
 
     if not PY2:
@@ -180,19 +180,31 @@
                 object.__delattr__(self, '__qualname__')
             except AttributeError:
                 pass
             try:
                 object.__setattr__(self, '__qualname__', value.__qualname__)
             except AttributeError:
                 pass
+            try:
+                object.__delattr__(self, '__annotations__')
+            except AttributeError:
+                pass
+            try:
+                object.__setattr__(self, '__annotations__', value.__annotations__)
+            except AttributeError:
+                pass
 
         elif name == '__qualname__':
             setattr(self.__wrapped__, name, value)
             object.__setattr__(self, name, value)
 
+        elif name == '__annotations__':
+            setattr(self.__wrapped__, name, value)
+            object.__setattr__(self, name, value)
+
         elif hasattr(type(self), name):
             object.__setattr__(self, name, value)
 
         else:
             setattr(self.__wrapped__, name, value)
 
     def __getattribute__(self, name):
@@ -447,35 +459,50 @@
 
     def __reduce_ex__(self, protocol):
         raise NotImplementedError(
                 'object proxy must define __reduce_ex__()')
 
 class CallableObjectProxy(ObjectProxy):
 
-    def __call__(self, *args, **kwargs):
+    def __call__(*args, **kwargs):
+        def _unpack_self(self, *args):
+            return self, args
+
+        self, args = _unpack_self(*args)
+
         return self.__wrapped__(*args, **kwargs)
 
 class PartialCallableObjectProxy(ObjectProxy):
     __slots__ = ('_self_args', '_self_kwargs')
 
-    def __init__(self, *args, **kwargs):
+    def __init__(*args, **kwargs):
+        def _unpack_self(self, *args):
+            return self, args
+
+        self, args = _unpack_self(*args)
+
         if len(args) < 1:
             raise TypeError('partial type takes at least one argument')
 
         wrapped, args = args[0], args[1:]
 
         if not callable(wrapped):
             raise TypeError('the first argument must be callable')
 
         super(PartialCallableObjectProxy, self).__init__(wrapped)
 
         object.__setattr__(self, '_self_args', args)
         object.__setattr__(self, '_self_kwargs', kwargs)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(*args, **kwargs):
+        def _unpack_self(self, *args):
+            return self, args
+
+        self, args = _unpack_self(*args)
+    
         _args = self._self_args + args
 
         _kwargs = dict(self._self_kwargs)
         _kwargs.update(kwargs)
 
         return self.__wrapped__(*_args, **_kwargs)
 
@@ -552,15 +579,20 @@
                 self._self_enabled, self._self_binding,
                 self._self_parent)
             self._bfws.append(ret)
             return ret
 
         return self
 
-    def __call__(self, *args, **kwargs):
+    def __call__(*args, **kwargs):
+        def _unpack_self(self, *args):
+            return self, args
+
+        self, args = _unpack_self(*args)
+
         # If enabled has been specified, then evaluate it at this point
         # and if the wrapper is not to be executed, then simply return
         # the bound function rather than a bound wrapper for the bound
         # function. When evaluating enabled, if it is callable we call
         # it, otherwise we evaluate it as a boolean.
 
         if self._self_enabled is not None:
@@ -570,15 +602,15 @@
             elif not self._self_enabled:
                 return self.__wrapped__(*args, **kwargs)
 
         # This can occur where initial function wrapper was applied to
         # a function that was already bound to an instance. In that case
         # we want to extract the instance from the function and use it.
 
-        if self._self_binding == 'function':
+        if self._self_binding in ('function', 'classmethod'):
             if self._self_instance is None:
                 instance = getattr(self.__wrapped__, '__self__', None)
                 if instance is not None:
                     return self._self_wrapper(self.__wrapped__, instance,
                             args, kwargs)
 
         # This is generally invoked when the wrapped function is being
@@ -586,14 +618,41 @@
         # instance method. This is also invoked in the case where the
         # wrapped function was a method, but this wrapper was in turn
         # wrapped using the staticmethod decorator.
 
         return self._self_wrapper(self.__wrapped__, self._self_instance,
                 args, kwargs)
 
+    def __set_name__(self, owner, name):
+        # This is a special method use to supply information to
+        # descriptors about what the name of variable in a class
+        # definition is. Not wanting to add this to ObjectProxy as not
+        # sure of broader implications of doing that. Thus restrict to
+        # FunctionWrapper used by decorators.
+
+        if hasattr(self.__wrapped__, "__set_name__"):
+            self.__wrapped__.__set_name__(owner, name)
+
+    def __instancecheck__(self, instance):
+        # This is a special method used by isinstance() to make checks
+        # instance of the `__wrapped__`.
+        return isinstance(instance, self.__wrapped__)
+
+    def __subclasscheck__(self, subclass):
+        # This is a special method used by issubclass() to make checks
+        # about inheritance of classes. We need to upwrap any object
+        # proxy. Not wanting to add this to ObjectProxy as not sure of
+        # broader implications of doing that. Thus restrict to
+        # FunctionWrapper used by decorators.
+
+        if hasattr(subclass, "__wrapped__"):
+            return issubclass(subclass.__wrapped__, self.__wrapped__)
+        else:
+            return issubclass(subclass, self.__wrapped__)
+
 class BoundFunctionWrapper(_FunctionWrapperBase):
 
     def __new__(cls, *args, **kwargs):
         # In addition to constructing a BoundFoundWrapper internally,
         # we need to be able to handle being created as if we were an
         # instance of types.BoundMethod. Creating and using a weakref
         # to a bound function relies on being able to do this. Since a
@@ -607,15 +666,20 @@
         if len(args) == 2:
             func = args[0]      # the function
             obj = args[1]       # the object it's bound to
             return types.MethodType(func, obj)
 
         return super(BoundFunctionWrapper, cls).__new__(cls)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(*args, **kwargs):
+        def _unpack_self(self, *args):
+            return self, args
+
+        self, args = _unpack_self(*args)
+
         # If enabled has been specified, then evaluate it at this point
         # and if the wrapper is not to be executed, then simply return
         # the bound function rather than a bound wrapper for the bound
         # function. When evaluating enabled, if it is callable we call
         # it, otherwise we evaluate it as a boolean.
 
         if self._self_enabled is not None:
@@ -669,18 +733,29 @@
 
 class FunctionWrapper(_FunctionWrapperBase):
 
     __bound_function_wrapper__ = BoundFunctionWrapper
 
     # The code here is pretty complicated (see the comment below), and it's not completely clear to
     # me whether it actually keeps any state. If it does, __reduce_ex__ needs to return a tuple so a
-    # new FunctionWrapper will be created. If it doesn't, then __reduce_ex__ could simply return a
+    # new FunctionWrapper will be created. If it doesn't, then __reduce_ex__ can simply return a
     # string, which would cause deepcopy to return the original FunctionWrapper.
+    #
+    # Update: We'll return the qualname of the wrapped function instead of a tuple allows a
+    # FunctionWrapper to be pickled (as the function it wraps). This seems to be adequate for
+    # generating AppMaps, so go with that.
+
     def __reduce_ex__(self, protocol):
-        return FunctionWrapper, (self.__wrapped__, self._self_wrapper, self._self_enabled)
+         return self.__wrapped__.__qualname__
+ 
+         # return FunctionWrapper, (
+         #     self.__wrapped__,
+         #     self._self_wrapper,
+         #     self._self_enabled,
+         # )
 
     def __init__(self, wrapped, wrapper, enabled=None):
         # What it is we are wrapping here could be anything. We need to
         # try and detect specific cases though. In particular, we need
         # to detect when we are given something that is a method of a
         # class. Further, we need to know when it is likely an instance
         # method, as opposed to a class or static method. This can
@@ -974,15 +1049,20 @@
 
         except AttributeError:
             self._self_instance = None
 
             super(WeakFunctionProxy, self).__init__(
                     weakref.proxy(wrapped, _callback))
 
-    def __call__(self, *args, **kwargs):
+    def __call__(*args, **kwargs):
+        def _unpack_self(self, *args):
+            return self, args
+
+        self, args = _unpack_self(*args)
+
         # We perform a boolean check here on the instance and wrapped
         # function as that will trigger the reference error prior to
         # calling if the reference had expired.
 
         instance = self._self_instance and self._self_instance()
         function = self.__wrapped__ and self.__wrapped__
```

### Comparing `appmap-1.9.1/PKG-INFO` & `appmap-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: appmap
-Version: 1.9.1
+Version: 2.0.0
 Summary: Create AppMap files by recording a Python application.
 Home-page: https://github.com/applandinc/appmap-python
 License: MIT
 Author: Alan Potter
 Author-email: alan@app.land
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Documentation
-Requires-Dist: PyYAML (>=5.3.0,<6.0.0)
-Requires-Dist: importlib-metadata (>=0.8)
+Requires-Dist: PyYAML (>=5.3.0)
 Requires-Dist: importlib-resources (>=5.4.0,<6.0.0)
 Requires-Dist: inflection (>=0.3.0)
-Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: packaging (>=19.0)
 Description-Content-Type: text/markdown
 
 - [About](#about)
 - [Usage](#usage)
 - [Development](#development)
   - [Getting the code](#getting-the-code)
   - [Python version support](#python-version-support)
   - [Dependency management](#dependency-management)
+    - [wrapt](#wrapt)
   - [Linting](#linting)
   - [Testing](#testing)
     - [pytest](#pytest)
     - [tox](#tox)
   - [Code Coverage](#code-coverage)
 
 # About
@@ -54,42 +53,28 @@
 
 # Usage
 
 Visit the [AppMap for Python](https://appland.com/docs/reference/appmap-python.html) reference page on AppLand.com for a complete reference guide.
 
 # Development
 
-[![Build Status](https://travis-ci.com/applandinc/appmap-python.svg?branch=master)](https://travis-ci.com/applandinc/appmap-python)
+[![Build Status](https://travis-ci.com/getappmap/appmap-python.svg?branch=master)](https://travis-ci.com/getappmap/appmap-python)
 
 ## Getting the code
-Clone the repo to begin development. Note that vendored dependencies are included as
-submodules.
+Clone the repo to begin development.
 
 ```shell
-% git clone --recurse-submodules https://github.com/applandinc/appmap-python.git
+% git clone https://github.com/applandinc/appmap-python.git
 Cloning into 'appmap-python'...
 remote: Enumerating objects: 167, done.
 remote: Counting objects: 100% (167/167), done.
 remote: Compressing objects: 100% (100/100), done.
 remote: Total 962 (delta 95), reused 116 (delta 61), pack-reused 795
 Receiving objects: 100% (962/962), 217.31 KiB | 4.62 MiB/s, done.
 Resolving deltas: 100% (653/653), done.
-Submodule 'extern/wrapt' (https://github.com/applandinc/wrapt.git) registered for path 'vendor/wrapt'
-Cloning into '/private/tmp/appmap-python/vendor/wrapt'...
-remote: Enumerating objects: 46, done.
-remote: Counting objects: 100% (46/46), done.
-remote: Compressing objects: 100% (39/39), done.
-remote: Total 2537 (delta 9), reused 19 (delta 4), pack-reused 2491
-Receiving objects: 100% (2537/2537), 755.94 KiB | 7.48 MiB/s, done.
-Resolving deltas: 100% (1643/1643), done.
-Submodule path 'vendor/wrapt': checked out '9bdfbe54b88a64069cba1f3c36e77edc3c1339c9'
-
-% ls appmap-python/vendor/wrapt
-LICENSE		Makefile	appveyor.yml	docs		src		tests
-MANIFEST.in	README.rst	blog		setup.py	tddium.yml	tox.ini
 ```
 
 ## Python version support
 As a package intended to be installed in as many environments as possible, `appmap-python`
 needs to avoid using features of Python or the standard library that were added after the
 oldest version currently supported (see the
 [supported versions](https://appland.com/docs/reference/appmap-python.html#supported-versions)).
@@ -100,49 +85,61 @@
 
 ```
 % brew install poetry
 % cd appmap-python
 % poetry install
 ```
 
+### wrapt
+The one dependency that is not managed using `poetry` is `wrapt`. Because it's possible that
+projects that use `appmap` may also need an unmodified version of `wrapt` (e.g. `pylint` depends on
+`astroid`, which in turn depends on `wrapt`), we use
+[vendoring](https://github.com/pradyunsg/vendoring) to vendor `wrapt`.
+
+To update `wrapt`, use `tox` (described below) to run the `vendoring` environment.
+
 ## Linting
 [pylint](https://www.pylint.org/) for linting:
 
 ```
 % cd appmap-python
 % poetry run pylint appmap
 
 --------------------------------------------------------------------
 Your code has been rated at 10.00/10 (previous run: 10.00/10, +0.00)
 
 ```
 
-[Note that the current configuration requires a 10.0 for the Travis build to pass. To make
-this easier to achieve, convention and refactoring checks have both been disabled. They
-should be reenabled as soon as possible.]
+[Note that the current configuration has a threshold set which must be met for the Travis build to
+pass. To make this easier to achieve, a number of checks have both been disabled. They should be
+reenabled as soon as possible.]
 
 
 ## Testing
 ### pytest
 
 Note that you must install the dependencies contained in
-[requirements-test.txt](requirements-test.txt) before running tests. See the explanation in
+[requirements-dev.txt](requirements-dev.txt) before running tests. See the explanation in
 [pyproject.toml](pyproject.toml) for details.
 
+Additionally, the tests currently require that you set `APPMAP=true`. You can
+either run `pytest` with `appmap-python` (see [tox.ini](tox.ini)), or you can explicitly
+set the environment variable.
+
 [pytest](https://docs.pytest.org/en/stable/) for testing:
 
 ```
 % cd appmap-python
 % pip install -r requirements-test.txt
 % poetry run pytest
 ```
 
 ### tox
 Additionally, the `tox` configuration provides the ability to run the tests for all
-supported versions of Python and djanggo. 
+supported versions of Python and Django.
 
 `tox` requires that all the correct versions of Python to be available to create
 the test environments. [pyenv](https://github.com/pyenv/pyenv) is an easy way to manage
 multiple versions of Python, and the [xxenv-latest
 plugin](https://github.com/momo-lab/xxenv-latest) can help get all the latest versions.
```

