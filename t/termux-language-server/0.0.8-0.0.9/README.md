# Comparing `tmp/termux-language-server-0.0.8.tar.gz` & `tmp/termux-language-server-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termux-language-server-0.0.8.tar", last modified: Fri Oct 27 05:30:05 2023, max compression
+gzip compressed data, was "termux-language-server-0.0.9.tar", last modified: Fri Oct 27 07:33:05 2023, max compression
```

## Comparing `termux-language-server-0.0.8.tar` & `termux-language-server-0.0.9.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.292852 termux-language-server-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.284852 termux-language-server-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.284852 termux-language-server-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/.gitlint
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11400 2023-10-27 05:30:05.292852 termux-language-server-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.284852 termux-language-server-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.284852 termux-language-server-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/docs/api/termux-language-server.md
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.284852 termux-language-server-0.0.8/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.284852 termux-language-server-0.0.8/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (127)       60 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/requirements/colorize.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       56 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/requirements/misc.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       86 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/requirements/pkgbuild.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 05:30:05.292852 termux-language-server-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.284852 termux-language-server-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.288852 termux-language-server-0.0.8/src/termux_language_server/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-10-27 05:30:05.000000 termux-language-server-0.0.8/src/termux_language_server/_metainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-27 05:30:05.000000 termux-language-server-0.0.8/src/termux_language_server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.284852 termux-language-server-0.0.8/src/termux_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.288852 termux-language-server-0.0.8/src/termux_language_server/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/jinja2/template.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.288852 termux-language-server-0.0.8/src/termux_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (127)    20422 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/json/PKGBUILD.json
--rw-r--r--   0 runner    (1001) docker     (127)    22451 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/json/build.sh.json
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/json/color.map.json
--rw-r--r--   0 runner    (1001) docker     (127)    41542 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/json/ebuild.json
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/json/install.json
--rw-r--r--   0 runner    (1001) docker     (127)    55132 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/json/make.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/json/makepkg.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/assets/json/subpackage.sh.json
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/finders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.288852 termux-language-server-0.0.8/src/termux_language_server/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/misc/color_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/misc/ebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/misc/make_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/misc/makepkg_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/misc/pkgbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/misc/termux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.288852 termux-language-server-0.0.8/src/termux_language_server/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/packages/pkgbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9067 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.288852 termux-language-server-0.0.8/src/termux_language_server/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/tools/namcap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/src/termux_language_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.288852 termux-language-server-0.0.8/src/termux_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11400 2023-10-27 05:30:05.000000 termux-language-server-0.0.8/src/termux_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-10-27 05:30:05.000000 termux-language-server-0.0.8/src/termux_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 05:30:05.000000 termux-language-server-0.0.8/src/termux_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-10-27 05:30:05.000000 termux-language-server-0.0.8/src/termux_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-27 05:30:05.000000 termux-language-server-0.0.8/src/termux_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-27 05:30:05.000000 termux-language-server-0.0.8/src/termux_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.288852 termux-language-server-0.0.8/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 05:30:05.292852 termux-language-server-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/tests/PKGBUILD
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/tests/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/tests/neovim-0.9.4.ebuild
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-27 05:29:52.000000 termux-language-server-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.291957 termux-language-server-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.291957 termux-language-server-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11493 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.291957 termux-language-server-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.291957 termux-language-server-0.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/docs/api/termux-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.295956 termux-language-server-0.0.9/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.295956 termux-language-server-0.0.9/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/requirements/colorize.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       56 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/requirements/misc.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       86 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/requirements/pkgbuild.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.291957 termux-language-server-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.295956 termux-language-server-0.0.9/src/termux_language_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-27 07:33:05.000000 termux-language-server-0.0.9/src/termux_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-27 07:33:05.000000 termux-language-server-0.0.9/src/termux_language_server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.291957 termux-language-server-0.0.9/src/termux_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.295956 termux-language-server-0.0.9/src/termux_language_server/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/jinja2/template.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/src/termux_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (127)    22395 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/json/PKGBUILD.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22451 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/json/build.sh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/json/color.map.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41542 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/json/ebuild.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/json/install.json
+-rw-r--r--   0 runner    (1001) docker     (127)    55132 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/json/make.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/json/makepkg.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/assets/json/subpackage.sh.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/finders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/src/termux_language_server/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/misc/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/misc/ebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/misc/make_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/misc/makepkg_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/misc/pkgbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/misc/termux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/src/termux_language_server/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/packages/pkgbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/src/termux_language_server/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/tools/namcap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/src/termux_language_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.295956 termux-language-server-0.0.9/src/termux_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11493 2023-10-27 07:33:05.000000 termux-language-server-0.0.9/src/termux_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2023-10-27 07:33:05.000000 termux-language-server-0.0.9/src/termux_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 07:33:05.000000 termux-language-server-0.0.9/src/termux_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-10-27 07:33:05.000000 termux-language-server-0.0.9/src/termux_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-27 07:33:05.000000 termux-language-server-0.0.9/src/termux_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-27 07:33:05.000000 termux-language-server-0.0.9/src/termux_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/templates/metainfo.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 07:33:05.299957 termux-language-server-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/tests/PKGBUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/tests/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/tests/neovim-0.9.4.ebuild
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-27 07:32:53.000000 termux-language-server-0.0.9/tests/test_utils.py
```

### Comparing `termux-language-server-0.0.8/.github/workflows/main.yml` & `termux-language-server-0.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/.gitignore` & `termux-language-server-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/.pre-commit-config.yaml` & `termux-language-server-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/LICENSE` & `termux-language-server-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/PKG-INFO` & `termux-language-server-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-language-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: Language server for build.sh, PKGBUILD, ebuild
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://termux-language-server.readthedocs.io
 Project-URL: Download, https://github.com/termux/termux-language-server/releases
 Project-URL: Bug Report, https://github.com/termux/termux-language-server/issues
 Project-URL: Source, https://github.com/termux/termux-language-server
@@ -107,15 +107,17 @@
     - [x] style check
       - [x] `PKGBUILD`: by [namcap](https://wiki.archlinux.org/title/Namcap)
 - [x] [Document Formatting](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_formatting):
   - [x] sort variables
   - [x] sort values
 - [x] [Document Link](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_documentLink):
   - [x] `build.sh`: <https://github.com/termux/termux-packages/tree/master/packages/package_name/build.sh>
-  - [x] `PKGBUILD`: <https://archlinux.org/packages/package_name>
+  - [x] `PKGBUILD`:
+    - [x] ArchLinux: <https://archlinux.org/packages/package_name>
+    - [x] Windows Msys2: <https://packages.msys2.org/base/package_name>
   - [ ] `ebuild`: <https://packages.gentoo.org/packages/package_name>
 - [x] [Hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_hover)
 - [x] [Completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_completion)
   - [x] builtin variables
   - [x] package names
     - [ ] `build.sh`
     - [x] `PKGBUILD`: by [pyalpm](https://github.com/ornitorrincos/pyalpm)
```

### Comparing `termux-language-server-0.0.8/README.md` & `termux-language-server-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,17 @@
     - [x] style check
       - [x] `PKGBUILD`: by [namcap](https://wiki.archlinux.org/title/Namcap)
 - [x] [Document Formatting](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_formatting):
   - [x] sort variables
   - [x] sort values
 - [x] [Document Link](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_documentLink):
   - [x] `build.sh`: <https://github.com/termux/termux-packages/tree/master/packages/package_name/build.sh>
-  - [x] `PKGBUILD`: <https://archlinux.org/packages/package_name>
+  - [x] `PKGBUILD`:
+    - [x] ArchLinux: <https://archlinux.org/packages/package_name>
+    - [x] Windows Msys2: <https://packages.msys2.org/base/package_name>
   - [ ] `ebuild`: <https://packages.gentoo.org/packages/package_name>
 - [x] [Hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_hover)
 - [x] [Completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_completion)
   - [x] builtin variables
   - [x] package names
     - [ ] `build.sh`
     - [x] `PKGBUILD`: by [pyalpm](https://github.com/ornitorrincos/pyalpm)
```

### Comparing `termux-language-server-0.0.8/docs/conf.py` & `termux-language-server-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/docs/resources/configure.md` & `termux-language-server-0.0.9/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/docs/resources/install.md` & `termux-language-server-0.0.9/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/pyproject.toml` & `termux-language-server-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 
 [tool.setuptools_scm]
 write_to = "src/termux_language_server/_version.py"
 
 [tool.setuptools-generate]
 write-to = "src/termux_language_server/_metainfo.py"
 
+[tool.setuptools-generate.metainfo-template]
+file = "templates/metainfo.py.j2"
+
 [tool.mdformat]
 number = true
 
 [tool.black]
 line-length = 79
 
 [tool.isort]
```

### Comparing `termux-language-server-0.0.8/src/termux_language_server/__init__.py` & `termux-language-server-0.0.9/src/termux_language_server/__init__.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/__main__.py` & `termux-language-server-0.0.9/src/termux_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/_metainfo.py` & `termux-language-server-0.0.9/src/termux_language_server/_metainfo.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 
 # For help2man
 DESCRIPTION = "Language server for build.sh, PKGBUILD, ebuild"
 EPILOG = "Report bugs to https://github.com/termux/termux-language-server/issues"
 # format __version__ by yourself
 VERSION = """termux-language-server {__version__}
 Copyright (C) 2023
-Written by Wu Zhenyu <wuzhenyu@ustc.edu> """
+Written by Wu Zhenyu <wuzhenyu@ustc.edu> """
+SOURCE = "https://github.com/termux/termux-language-server"
```

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/jinja2/template.md.j2` & `termux-language-server-0.0.9/src/termux_language_server/assets/jinja2/template.md.j2`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/json/PKGBUILD.json` & `termux-language-server-0.0.9/src/termux_language_server/assets/json/PKGBUILD.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9851487016908212%*

 * *Differences: {"'properties'": "{'url': {'format': 'uri'}, 'arch': {'items': {'enum': ['any', 'i686', 'x86_64', "*

 * *                 "'arm', 'aarch64']}}, 'mingw_arch': OrderedDict([('type', 'array'), "*

 * *                 "('description', 'A list of MSYS2 environments the package is built for. Defaults "*

 * *                 "to an empty list.'), ('items', OrderedDict([('type', 'string'), ('enum', "*

 * *                 "['mingw32', 'mingw64', 'ucrt64', 'clang64', 'clang32', 'clangarm64'])])), "*

 * *                 "('uniqueItems', Tru […]*

```diff
@@ -20,14 +20,21 @@
             "description": "An optional prepare() function can be specified in which operations to prepare the sources for building, such as patching, are performed. This function is run after the source extraction and before the build() function. The prepare() function is skipped when source extraction is skipped."
         }
     },
     "properties": {
         "arch": {
             "description": "Defines on which architectures the given package is available (e.g., arch=(i686 x86_64)). Packages that contain no architecture specific files should use arch=(any). Valid characters for members of this array are alphanumerics and \"\\_\".",
             "items": {
+                "enum": [
+                    "any",
+                    "i686",
+                    "x86_64",
+                    "arm",
+                    "aarch64"
+                ],
                 "type": "string"
             },
             "type": "array",
             "uniqueItems": true
         },
         "b2sums": {
             "description": "Alternative integrity checks that makepkg supports; these all behave similar to the cksums option described above. To enable use and generation of these checksums, be sure to set up the INTEGRITY_CHECK option in **makepkg.conf**(5).",
@@ -125,14 +132,68 @@
             "description": "Alternative integrity checks that makepkg supports; these all behave similar to the cksums option described above. To enable use and generation of these checksums, be sure to set up the INTEGRITY_CHECK option in **makepkg.conf**(5).",
             "items": {
                 "type": "string"
             },
             "type": "array",
             "uniqueItems": true
         },
+        "mingw_arch": {
+            "description": "A list of MSYS2 environments the package is built for. Defaults to an empty list.",
+            "items": {
+                "enum": [
+                    "mingw32",
+                    "mingw64",
+                    "ucrt64",
+                    "clang64",
+                    "clang32",
+                    "clangarm64"
+                ],
+                "type": "string"
+            },
+            "type": "array",
+            "uniqueItems": true
+        },
+        "msys2_changelog_url": {
+            "description": "NEWS file in git or the GitHub releases page. In case there are multiple, the one that is more useful for packagers.",
+            "format": "uri",
+            "type": "string"
+        },
+        "msys2_documentation_url": {
+            "description": "URL to the documentation for the API, tools, etc., in case it's a different website than the homepage.",
+            "format": "uri",
+            "type": "string"
+        },
+        "msys2_internal": {
+            "description": "Whether the package is an internal or meta package and shouldn't be linked to external sources. Defaults to false.",
+            "type": "boolean"
+        },
+        "msys2_issue_tracker_url": {
+            "description": "URL to the bug tracker, mailing list archive, etc.",
+            "format": "uri",
+            "type": "string"
+        },
+        "msys2_pgp_keys_url": {
+            "description": "URL to a website containing which keys are used to sign releases.",
+            "format": "uri",
+            "type": "string"
+        },
+        "msys2_references": {
+            "description": "Maps the package to external resources, such as other package repositories.",
+            "items": {
+                "pattern": "(archlinux|aur|cygwin|cygwin-mingw64|pypi)(|: .*)",
+                "type": "string"
+            },
+            "type": "array",
+            "uniqueItems": true
+        },
+        "msys2_repository_url": {
+            "description": "URL to the web view of the repository, e.g., on GitHub or GitLab.",
+            "format": "uri",
+            "type": "string"
+        },
         "noextract": {
             "description": "An array of file names corresponding to those from the source array. Files listed here will not be extracted with the rest of the source files. This is useful for packages that use compressed data directly.",
             "items": {
                 "type": "string"
             },
             "type": "array",
             "uniqueItems": true
@@ -262,14 +323,15 @@
         },
         "startdir": {
             "description": "This contains the absolute path to the directory where the PKGBUILD is located, which is usually the output of \\$(pwd) when makepkg is started. Use of this variable is deprecated and strongly discouraged.",
             "type": "string"
         },
         "url": {
             "description": "The URL to the VCS repository. This must include the VCS in the URL protocol for makepkg to recognize this as a VCS source. If the protocol does not include the VCS name, it can be added by prefixing the URL with vcs+. For example, using a Git repository over HTTPS would have a source URL in the form: git+https://\\....",
+            "format": "uri",
             "type": "string"
         },
         "validpgpkeys": {
             "description": "An array of PGP fingerprints. If this array is non-empty, makepkg will only accept signatures from the keys listed here and will ignore the trust values from the keyring. If the source file was signed with a subkey, makepkg will still use the primary key for comparison.\nOnly full fingerprints are accepted. They must be uppercase and must not contain whitespace characters.",
             "items": {
                 "type": "string"
             },
```

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/json/build.sh.json` & `termux-language-server-0.0.9/src/termux_language_server/assets/json/build.sh.json`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/json/color.map.json` & `termux-language-server-0.0.9/src/termux_language_server/assets/json/color.map.json`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/json/ebuild.json` & `termux-language-server-0.0.9/src/termux_language_server/assets/json/ebuild.json`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/json/install.json` & `termux-language-server-0.0.9/src/termux_language_server/assets/json/install.json`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/json/make.conf.json` & `termux-language-server-0.0.9/src/termux_language_server/assets/json/make.conf.json`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/json/makepkg.conf.json` & `termux-language-server-0.0.9/src/termux_language_server/assets/json/makepkg.conf.json`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/assets/json/subpackage.sh.json` & `termux-language-server-0.0.9/src/termux_language_server/assets/json/subpackage.sh.json`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/finders.py` & `termux-language-server-0.0.9/src/termux_language_server/finders.py`

 * *Files 3% similar despite different names*

```diff
@@ -365,14 +365,31 @@
                 "makedepends",
                 "conflicts",
                 "provides",
             ]
         )
 
 
+@dataclass
+class MinGWFinder(Finder):
+    r"""Mingwfinder."""
+
+    def __call__(self, uni: UNI) -> bool:
+        r"""Call.
+
+        :param uni:
+        :type uni: UNI
+        :rtype: bool
+        """
+        text = uni.get_text()
+        return uni.node.type == "variable_name" and (
+            text.startswith("mingw_") or text.startswith("msys2_")
+        )
+
+
 DIAGNOSTICS_FINDER_CLASSES = [
     ErrorFinder,
     MissingFinder,
     BashFinder,
     UnsortedKeywordFinder,
     UnsortedCSVFinder,
 ]
```

### Comparing `termux-language-server-0.0.8/src/termux_language_server/misc/__init__.py` & `termux-language-server-0.0.9/src/termux_language_server/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/misc/color_map.py` & `termux-language-server-0.0.9/src/termux_language_server/misc/color_map.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/misc/ebuild.py` & `termux-language-server-0.0.9/src/termux_language_server/misc/ebuild.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/misc/make_conf.py` & `termux-language-server-0.0.9/src/termux_language_server/misc/make_conf.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/misc/makepkg_conf.py` & `termux-language-server-0.0.9/src/termux_language_server/misc/makepkg_conf.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/misc/termux.py` & `termux-language-server-0.0.9/src/termux_language_server/misc/termux.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/packages/__init__.py` & `termux-language-server-0.0.9/src/termux_language_server/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/packages/pkgbuild.py` & `termux-language-server-0.0.9/src/termux_language_server/packages/pkgbuild.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/schema.py` & `termux-language-server-0.0.9/src/termux_language_server/schema.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/server.py` & `termux-language-server-0.0.9/src/termux_language_server/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from tree_sitter_lsp.finders import PositionFinder
 from tree_sitter_lsp.format import get_text_edits
 
 from .finders import (
     DIAGNOSTICS_FINDER_CLASSES,
     FORMAT_FINDER_CLASSES,
     CSVFinder,
+    MinGWFinder,
     PackageFinder,
 )
 from .packages import search_package_document, search_package_names
 from .utils import get_filetype, get_schema
 
 
 class TermuxLanguageServer(LanguageServer):
@@ -118,18 +119,22 @@
             if filetype in {"build.sh", "subpackage.sh"}:
                 return CSVFinder(filetype).get_document_links(
                     document.uri,
                     self.trees[document.uri],
                     "https://github.com/termux/termux-packages/tree/master/packages/{{name}}/build.sh",
                 )
             elif filetype in {"PKGBUILD", "install"}:
+                if MinGWFinder().find(document.uri, self.trees[document.uri]):
+                    url = "https://packages.msys2.org/base/{{uni.get_text()}}"
+                else:
+                    url = "https://archlinux.org/packages/{{uni.get_text()}}"
                 return PackageFinder().get_document_links(
                     document.uri,
                     self.trees[document.uri],
-                    "https://archlinux.org/packages/{{uni.get_text()}}",
+                    url,
                 )
             raise NotImplementedError
 
         @self.feature(TEXT_DOCUMENT_HOVER)
         def hover(params: TextDocumentPositionParams) -> Hover | None:
             r"""Hover.
```

### Comparing `termux-language-server-0.0.8/src/termux_language_server/tools/namcap.py` & `termux-language-server-0.0.9/src/termux_language_server/tools/namcap.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server/utils.py` & `termux-language-server-0.0.9/src/termux_language_server/utils.py`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/src/termux_language_server.egg-info/PKG-INFO` & `termux-language-server-0.0.9/src/termux_language_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-language-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: Language server for build.sh, PKGBUILD, ebuild
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://termux-language-server.readthedocs.io
 Project-URL: Download, https://github.com/termux/termux-language-server/releases
 Project-URL: Bug Report, https://github.com/termux/termux-language-server/issues
 Project-URL: Source, https://github.com/termux/termux-language-server
@@ -107,15 +107,17 @@
     - [x] style check
       - [x] `PKGBUILD`: by [namcap](https://wiki.archlinux.org/title/Namcap)
 - [x] [Document Formatting](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_formatting):
   - [x] sort variables
   - [x] sort values
 - [x] [Document Link](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_documentLink):
   - [x] `build.sh`: <https://github.com/termux/termux-packages/tree/master/packages/package_name/build.sh>
-  - [x] `PKGBUILD`: <https://archlinux.org/packages/package_name>
+  - [x] `PKGBUILD`:
+    - [x] ArchLinux: <https://archlinux.org/packages/package_name>
+    - [x] Windows Msys2: <https://packages.msys2.org/base/package_name>
   - [ ] `ebuild`: <https://packages.gentoo.org/packages/package_name>
 - [x] [Hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_hover)
 - [x] [Completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_completion)
   - [x] builtin variables
   - [x] package names
     - [ ] `build.sh`
     - [x] `PKGBUILD`: by [pyalpm](https://github.com/ornitorrincos/pyalpm)
```

### Comparing `termux-language-server-0.0.8/src/termux_language_server.egg-info/SOURCES.txt` & `termux-language-server-0.0.9/src/termux_language_server.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -53,13 +53,14 @@
 src/termux_language_server/misc/pkgbuild.py
 src/termux_language_server/misc/termux.py
 src/termux_language_server/packages/__init__.py
 src/termux_language_server/packages/pkgbuild.py
 src/termux_language_server/tools/namcap.py
 templates/class.txt
 templates/def.txt
+templates/metainfo.py.j2
 templates/noarg.txt
 tests/PKGBUILD
 tests/build.sh
 tests/neovim-0.9.4.ebuild
 tests/test_schema.py
 tests/test_utils.py
```

### Comparing `termux-language-server-0.0.8/tests/PKGBUILD` & `termux-language-server-0.0.9/tests/PKGBUILD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # shellcheck shell=bash disable=SC2034,SC2154
 # Updated by https://github.com/Freed-Wu/pkgbuild-language-server/blob/main/.github/workflows/main.yml
 pkgname=pkgbuild-language-server
 pkgver=0.0.6
 pkgrel=1
 pkgdesc="Archlinux and Windows Msys2's PKGBUILD language server"
 arch=(any)
+mingw_arch=(wrong_arch)
 url=https://github.com/Freed-Wu/pkgbuild-language-server
 depends=(python-colorama python-jinja python-platformdirs python-pygls python-tree-sitter)
 optdepends=(python-pypandoc python-markdown-it-py pacman pyalpm namcap)
 makedepends=python-installer
 license=(GPL3)
 _py=py3
 source=("https://files.pythonhosted.org/packages/$_py/${pkgname::1}/${pkgname//-/_}/${pkgname//-/_}-$pkgver-$_py-none-any.whl")
```

### Comparing `termux-language-server-0.0.8/tests/build.sh` & `termux-language-server-0.0.9/tests/build.sh`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/tests/neovim-0.9.4.ebuild` & `termux-language-server-0.0.9/tests/neovim-0.9.4.ebuild`

 * *Files identical despite different names*

### Comparing `termux-language-server-0.0.8/tests/test_schema.py` & `termux-language-server-0.0.9/tests/test_schema.py`

 * *Files identical despite different names*

