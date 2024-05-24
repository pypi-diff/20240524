# Comparing `tmp/authx-1.1.2.tar.gz` & `tmp/authx-1.1.3.tar.gz`

## Comparing `authx-1.1.2.tar` & `authx-1.1.3.tar`

### file list

```diff
@@ -1,115 +1,60 @@
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 authx-1.1.2/.all-contributorsrc
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 authx-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 authx-1.1.2/mkdocs.yml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 authx-1.1.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 authx-1.1.2/.github/SECURITY.md
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 authx-1.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 authx-1.1.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 authx-1.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 authx-1.1.2/authx/__init__.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 authx-1.1.2/authx/config.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 authx-1.1.2/authx/core.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 authx-1.1.2/authx/dependencies.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 authx-1.1.2/authx/exceptions.py
--rw-r--r--   0        0        0    25599 2020-02-02 00:00:00.000000 authx-1.1.2/authx/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.2/authx/py.typed
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 authx-1.1.2/authx/schema.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 authx-1.1.2/authx/token.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authx-1.1.2/authx/types.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/__init__.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_callback.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_error.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_logger.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_memory.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_signature.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 authx-1.1.2/authx/_internal/_utils.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 authx-1.1.2/docs/index.md
--rw-r--r--   0        0        0    51615 2020-02-02 00:00:00.000000 authx-1.1.2/docs/release.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/config.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/dependencies.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/exceptions.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/main.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/reference.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/request.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/token.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/cache.md
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/metrics.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/oauth2.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/profiler.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/extra/session.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/internal/callback.md
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/internal/errors.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/internal/memory.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 authx-1.1.2/docs/api/internal/signature.md
--rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 authx-1.1.2/docs/callbacks/token.md
--rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 authx-1.1.2/docs/callbacks/user.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 authx-1.1.2/docs/css/custom.css
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 authx-1.1.2/docs/css/termynal.css
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 authx-1.1.2/docs/dependencies/aliases.md
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 authx-1.1.2/docs/dependencies/bundle.md
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 authx-1.1.2/docs/dependencies/dependencies.md
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 authx-1.1.2/docs/dependencies/injection.md
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 authx-1.1.2/docs/development/contributing.md
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/Cache.md
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/Metrics.md
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/OAuth2.md
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/Sessions.md
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 authx-1.1.2/docs/extra/profiler.md
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 authx-1.1.2/docs/faq/code_of_conduct.md
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 authx-1.1.2/docs/faq/faq.md
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 authx-1.1.2/docs/faq/help.md
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 authx-1.1.2/docs/faq/license.md
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/basic-usage.md
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/installation.md
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/location.md
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/payload.md
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/refresh.md
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 authx-1.1.2/docs/get-started/token.md
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-1.1.2/docs/img/header.svg
--rw-r--r--   0        0        0   335246 2020-02-02 00:00:00.000000 authx-1.1.2/docs/img/icon.ico
--rw-r--r--   0        0        0   112430 2020-02-02 00:00:00.000000 authx-1.1.2/docs/img/logo.png
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 authx-1.1.2/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 authx-1.1.2/docs/js/termynal.js
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/all.txt
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/docs.in
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/docs.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/linting.in
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/linting.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/pyproject.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/testing.in
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 authx-1.1.2/requirements/testing.txt
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/clean.sh
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/docs_build.sh
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/docs_serve.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/format.sh
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/mypy.sh
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/requirements.sh
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/test.sh
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 authx-1.1.2/scripts/test_extra.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_authx.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_callback.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_config.py
--rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_core.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_dependencies.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_errors.py
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_schema.py
--rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 authx-1.1.2/tests/test_token.py
--rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 authx-1.1.2/tests/utils.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/conftest.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_access_location.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_blocklist_token.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_fresh_token.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_get_subject.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 authx-1.1.2/tests/app/test_token_protected_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/__init__.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/test_logger.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/test_memory.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/test_signature.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 authx-1.1.2/tests/internal/test_utils.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 authx-1.1.2/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx-1.1.2/LICENSE
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 authx-1.1.2/README.md
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 authx-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    12133 2020-02-02 00:00:00.000000 authx-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 authx-1.1.3/README.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 authx-1.1.3/authx/__init__.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 authx-1.1.3/authx/config.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 authx-1.1.3/authx/core.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 authx-1.1.3/authx/dependencies.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 authx-1.1.3/authx/exceptions.py
+-rw-r--r--   0        0        0    25603 2020-02-02 00:00:00.000000 authx-1.1.3/authx/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.3/authx/py.typed
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 authx-1.1.3/authx/schema.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 authx-1.1.3/authx/token.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authx-1.1.3/authx/types.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 authx-1.1.3/authx/_internal/__init__.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 authx-1.1.3/authx/_internal/_callback.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 authx-1.1.3/authx/_internal/_error.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 authx-1.1.3/authx/_internal/_logger.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 authx-1.1.3/authx/_internal/_memory.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 authx-1.1.3/authx/_internal/_signature.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 authx-1.1.3/authx/_internal/_utils.py
+-rw-r--r--   0        0        0    53081 2020-02-02 00:00:00.000000 authx-1.1.3/docs/release.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 authx-1.1.3/requirements/all.txt
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.1.3/requirements/docs.in
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 authx-1.1.3/requirements/docs.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 authx-1.1.3/requirements/linting.in
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 authx-1.1.3/requirements/linting.txt
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 authx-1.1.3/requirements/pyproject.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 authx-1.1.3/requirements/testing.in
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 authx-1.1.3/requirements/testing.txt
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 authx-1.1.3/scripts/clean.sh
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 authx-1.1.3/scripts/docs_build.sh
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 authx-1.1.3/scripts/docs_serve.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx-1.1.3/scripts/format.sh
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 authx-1.1.3/scripts/mypy.sh
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 authx-1.1.3/scripts/requirements.sh
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 authx-1.1.3/scripts/test.sh
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 authx-1.1.3/scripts/test_extra.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 authx-1.1.3/tests/test_authx.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 authx-1.1.3/tests/test_callback.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 authx-1.1.3/tests/test_config.py
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 authx-1.1.3/tests/test_core.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 authx-1.1.3/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 authx-1.1.3/tests/test_errors.py
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 authx-1.1.3/tests/test_schema.py
+-rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 authx-1.1.3/tests/test_token.py
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 authx-1.1.3/tests/utils.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 authx-1.1.3/tests/app/conftest.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 authx-1.1.3/tests/app/test_access_location.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 authx-1.1.3/tests/app/test_blocklist_token.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 authx-1.1.3/tests/app/test_fresh_token.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 authx-1.1.3/tests/app/test_get_subject.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 authx-1.1.3/tests/app/test_token_protected_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.3/tests/internal/__init__.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 authx-1.1.3/tests/internal/test_logger.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 authx-1.1.3/tests/internal/test_memory.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 authx-1.1.3/tests/internal/test_signature.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 authx-1.1.3/tests/internal/test_utils.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 authx-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 authx-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    31212 2020-02-02 00:00:00.000000 authx-1.1.3/PKG-INFO
```

### Comparing `authx-1.1.2/authx/config.py` & `authx-1.1.3/authx/config.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/core.py` & `authx-1.1.3/authx/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     return RequestToken(token=query_token, location="query")
 
 
 async def _get_token_from_json(
     request: Request, config: AuthXConfig, refresh: bool = False, **kwargs
 ) -> RequestToken:
-    if not (request.headers.get("content-type") == "application/json"):
+    if request.headers.get("content-type") != "application/json":
         raise MissingTokenError("Invalid content-type. Must be application/json")
 
     key = config.JWT_JSON_KEY
     token_type = "access"
     if refresh:
         token_type = "refresh"
         key = config.JWT_REFRESH_JSON_KEY
```

### Comparing `authx-1.1.2/authx/dependencies.py` & `authx-1.1.3/authx/dependencies.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/exceptions.py` & `authx-1.1.3/authx/exceptions.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/main.py` & `authx-1.1.3/authx/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,15 @@
         max_age: Optional[int] = None,
     ) -> None:
         """Add 'Set-Cookie' for access token in response header
 
         Args:
             token (str): Access token
             response (Response): response to set cookie on
-            max_age (Optional[int], optional): Max Age cookie paramater. Defaults to None.
+            max_age (Optional[int], optional): Max Age cookie parameter. Defaults to None.
         """
         self._set_cookies(
             token=token, type="access", response=response, max_age=max_age
         )
 
     def set_refresh_cookies(
         self,
@@ -458,15 +458,15 @@
         max_age: Optional[int] = None,
     ) -> None:
         """Add 'Set-Cookie' for refresh token in response header
 
         Args:
             token (str): Refresh token
             response (Response): response to set cookie on
-            max_age (Optional[int], optional): Max Age cookie paramater. Defaults to None.
+            max_age (Optional[int], optional): Max Age cookie parameter. Defaults to None.
         """
         self._set_cookies(
             token=token, type="refresh", response=response, max_age=max_age
         )
 
     def unset_access_cookies(
         self,
@@ -497,19 +497,19 @@
             response (Response): response to remove token cookies from
         """
         self.unset_access_cookies(response)
         self.unset_refresh_cookies(response)
 
     # Notes:
     # The AuthXDeps is a utility class, to enable quick token operations
-    # within the route logic. It provides methods to avoid addtional code
+    # within the route logic. It provides methods to avoid additional code
     # in your route that would be outside of the route logic
 
     # Such methods includes setting and unsetting cookies without the need
-    # to generate a response object beforhand.
+    # to generate a response object beforehand.
 
     @property
     def DEPENDENCY(self) -> AuthXDependency:
         """FastAPI Dependency to return an AuthX sub-object within the route context"""
         return Depends(self.get_dependency)
 
     @property
@@ -552,19 +552,19 @@
 
         Args:
             request (Request): Request context managed by FastAPI
             response (Response): Response context managed by FastAPI
 
         Note:
             The AuthXDeps is a utility class, to enable quick token operations
-            within the route logic. It provides methods to avoid addtional code
+            within the route logic. It provides methods to avoid additional code
             in your route that would be outside of the route logic
 
             Such methods includes setting and unsetting cookies without the need
-            to generate a response object beforhand
+            to generate a response object beforehand
 
         Returns:
             AuthXDeps: The contextful AuthX object
         """
         return AuthXDependency(self, request=request, response=response)
 
     def token_required(
```

### Comparing `authx-1.1.2/authx/schema.py` & `authx-1.1.3/authx/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,19 +117,21 @@
         )
 
     @classmethod
     def decode(
         cls,
         token: str,
         key: str,
-        algorithms: Sequence[AlgorithmType] = ["HS256"],
+        algorithms: Sequence[AlgorithmType] = None,
         audience: Optional[StringOrSequence] = None,
         issuer: Optional[str] = None,
         verify: bool = True,
     ) -> "TokenPayload":
+        if algorithms is None:  # pragma: no cover
+            algorithms = ["HS256"]  # pragma: no cover
         payload = decode_token(
             token=token,
             key=key,
             algorithms=algorithms,
             audience=audience,
             issuer=issuer,
             verify=verify,
@@ -142,22 +144,24 @@
     csrf: Optional[str] = None
     type: TokenType = "access"
     location: TokenLocation
 
     def verify(
         self,
         key: str,
-        algorithms: Sequence[AlgorithmType] = ["HS256"],
+        algorithms: Sequence[AlgorithmType] = None,
         audience: Optional[StringOrSequence] = None,
         issuer: Optional[str] = None,
         verify_jwt: bool = True,
         verify_type: bool = True,
         verify_csrf: bool = True,
         verify_fresh: bool = False,
     ) -> TokenPayload:
+        if algorithms is None:  # pragma: no cover
+            algorithms = ["HS256"]  # pragma: no cover
         # JWT Base Verification
         try:
             decoded_token = decode_token(
                 token=self.token,
                 key=key,
                 algorithms=algorithms,
                 verify=verify_jwt,
```

### Comparing `authx-1.1.2/authx/token.py` & `authx-1.1.3/authx/token.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,20 +79,22 @@
 
     return jwt.encode(payload=payload, key=key, algorithm=algorithm, headers=headers)
 
 
 def decode_token(
     token: str,
     key: str,
-    algorithms: Sequence[AlgorithmType] = ["HS256"],
+    algorithms: Sequence[AlgorithmType] = None,
     audience: Optional[StringOrSequence] = None,
     issuer: Optional[str] = None,
     verify: bool = True,
 ) -> Dict[str, Any]:
     """Decode a token"""
+    if algorithms is None:  # pragma: no cover
+        algorithms = ["HS256"]  # pragma: no cover
     try:
         return jwt.decode(
             jwt=token,
             key=key,
             algorithms=algorithms,
             audience=audience,
             issuer=issuer,
```

### Comparing `authx-1.1.2/authx/types.py` & `authx-1.1.3/authx/types.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/_internal/__init__.py` & `authx-1.1.3/authx/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/_internal/_callback.py` & `authx-1.1.3/authx/_internal/_callback.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/_internal/_error.py` & `authx-1.1.3/authx/_internal/_error.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/_internal/_logger.py` & `authx-1.1.3/authx/_internal/_logger.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/_internal/_memory.py` & `authx-1.1.3/authx/_internal/_memory.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/_internal/_signature.py` & `authx-1.1.3/authx/_internal/_signature.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/authx/_internal/_utils.py` & `authx-1.1.3/authx/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/docs/release.md` & `authx-1.1.3/docs/release.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,31 @@
----
-hide:
-  - navigation
----
+## Latest Changes
 
-# Release Notes
+### Internal
 
-## Latest Changes
+* 🔧 Separate CI of testing from Release one . PR [#593](https://github.com/yezz123/authx/pull/593) by [@yezz123](https://github.com/yezz123).
+
+## 1.1.3
+
+### Features
+
+* ♻️ Replaces use of default mutable arguments. PR [#589](https://github.com/yezz123/authx/pull/589) by [@yezz123](https://github.com/yezz123).
+
+### Upgrades
+
+* Bump requests from 2.31.0 to 2.32.2 in /requirements. PR [#592](https://github.com/yezz123/authx/pull/592) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ☔ [pre-commit.ci] pre-commit autoupdate. PR [#590](https://github.com/yezz123/authx/pull/590) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
+* ☔ [pre-commit.ci] pre-commit autoupdate. PR [#585](https://github.com/yezz123/authx/pull/585) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
+* ⬆️ Bump jinja2 from 3.1.3 to 3.1.4 in /requirements. PR [#584](https://github.com/yezz123/authx/pull/584) by [@dependabot[bot]](https://github.com/apps/dependabot).
+
+### Internal
+
+* 🔧 Update CI workflow, by adding release process. PR [#586](https://github.com/yezz123/authx/pull/586) by [@yezz123](https://github.com/yezz123).
+* 🔧 Update build targets & add `hatch-fancy-pypi-readme`. PR [#588](https://github.com/yezz123/authx/pull/588) by [@yezz123](https://github.com/yezz123).
+* 🔧 Add codespell hook for spell checking. PR [#587](https://github.com/yezz123/authx/pull/587) by [@yezz123](https://github.com/yezz123).
 
 ## 1.1.2
 
 ### Docs
 
 * 📝 Update badges and links in README. PR [#583](https://github.com/yezz123/authx/pull/583) by [@yezz123](https://github.com/yezz123).
 * 📝  Refactor route decorators to use `@app.get` instead of `@app.route`. PR [#576](https://github.com/yezz123/authx/pull/576) by [@yezz123](https://github.com/yezz123).
@@ -185,14 +201,16 @@
 * ⬆ Bump the python-packages group with 6 updates. PR [#541](https://github.com/yezz123/authx/pull/541) by @dependabot.
 
 ## 1.0.0b0
 
 !!! warning
     This is a beta release. Please do not use in production.
 
+<!-- package description limit -->
+
 ### Major Changes 🚑️
 
 * ➖ Remove Documentation Workflow. PR [#414](https://github.com/yezz123/authx/pull/414) by [@yezz123](https://github.com/yezz123).
 * ♻️ chore(revamp): AuthX Revamp - V1.0.0. PR [#446](https://github.com/yezz123/authx/pull/446) by [@yezz123](https://github.com/yezz123).
 * 🔧 Feat: Refactor & Rebuild Functionalities in authx. PR [#454](https://github.com/yezz123/authx/pull/454) by [@yezz123](https://github.com/yezz123).
 * 🐛 fix Continuous Integration Badge. [PR #455](https://github.com/yezz123/authx/pull/455) by [@yezz123](https://github.com/yezz123).
 * ♻️ use pip-tool to autogenerate dependencies[PR #478](https://github.com/yezz123/authx/pull/478) by [@yezz123](https://github.com/yezz123)
```

### Comparing `authx-1.1.2/docs/faq/license.md` & `authx-1.1.3/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-# License
+MIT License
 
-<p>
-     <img align="right" src="https://i0.wp.com/opensource.org/wp-content/uploads/2023/03/cropped-OSI-horizontal-large.png">
-</p>
-
-The class is licensed under the [MIT License](https://opensource.org/licenses/mit)
-
-Copyright &copy; 2021 to present [Yezz LLC.](https://yezz.me). and individual contributors.
+Copyright (c) 2021 to present Yezz LLC. and individual contributors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -21,9 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
----
```

### Comparing `authx-1.1.2/requirements/docs.txt` & `authx-1.1.3/requirements/docs.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile requirements/docs.in -o requirements/docs.txt
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   starlette
+    #   watchfiles
 async-timeout==4.0.3
     # via redis
-authx==1.1.1
+authx==1.1.2
     # via authx-extra
-authx-extra @ git+https://github.com/yezz123/authx-extra.git@9364049513e122f511e43a7bbd8ba0702b8d9fb8
-babel==2.14.0
+authx-extra @ git+https://github.com/yezz123/authx-extra.git@06ec79b130abc318a1409ad60e42e304016ea4f6
+babel==2.15.0
     # via mkdocs-material
 beautifulsoup4==4.12.3
     # via mkdocs-mermaid2-plugin
 cairocffi==1.7.0
     # via cairosvg
 cairosvg==2.7.1
 certifi==2024.2.2
@@ -30,51 +31,65 @@
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   mkdocs
     #   mkdocstrings
     #   typer
+    #   uvicorn
 colorama==0.4.6
     # via
     #   griffe
     #   mkdocs-material
-cryptography==42.0.5
+cryptography==42.0.7
     # via pyjwt
 cssselect2==0.7.0
     # via cairosvg
 cyclic==1.0.0
     # via mdx-include
 defusedxml==0.7.1
     # via cairosvg
+dnspython==2.6.1
+    # via email-validator
 ecdsa==0.19.0
     # via python-jose
 editorconfig==0.12.4
     # via jsbeautifier
-fastapi==0.110.3
+email-validator==2.1.1
+    # via fastapi
+fastapi==0.111.0
     # via authx
+fastapi-cli==0.0.4
+    # via fastapi
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.44.0
+griffe==0.45.1
     # via
     #   griffe-typingdoc
     #   mkdocstrings-python
 griffe-typingdoc==0.2.5
 h11==0.14.0
-    # via httpcore
+    # via
+    #   httpcore
+    #   uvicorn
 httpcore==1.0.5
     # via httpx
+httptools==0.6.1
+    # via uvicorn
 httpx==0.27.0
+    # via fastapi
 idna==3.7
     # via
     #   anyio
+    #   email-validator
     #   httpx
     #   requests
-jinja2==3.1.3
+jinja2==3.1.4
     # via
+    #   fastapi
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
 jsbeautifier==1.15.1
     # via mkdocs-mermaid2-plugin
 markdown==3.6
     # via
@@ -109,31 +124,33 @@
     #   mkdocs-mermaid2-plugin
     #   mkdocstrings
 mkdocs-autorefs==1.0.1
     # via mkdocstrings
 mkdocs-get-deps==0.2.0
     # via mkdocs
 mkdocs-markdownextradata-plugin==0.2.5
-mkdocs-material==9.5.20
+mkdocs-material==9.5.24
 mkdocs-material-extensions==1.3.1
     # via mkdocs-material
 mkdocs-mermaid2-plugin==1.1.1
-mkdocstrings==0.25.0
+mkdocstrings==0.25.1
     # via mkdocstrings-python
-mkdocstrings-python==1.10.0
+mkdocstrings-python==1.10.3
     # via mkdocstrings
+orjson==3.10.3
+    # via fastapi
 packaging==24.0
     # via mkdocs
 paginate==0.5.6
     # via mkdocs-material
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via cairosvg
-platformdirs==4.2.1
+platformdirs==4.2.2
     # via
     #   mkdocs-get-deps
     #   mkdocstrings
 prometheus-client==0.20.0
     # via authx-extra
 pyasn1==0.6.0
     # via
@@ -146,15 +163,15 @@
     #   authx
     #   fastapi
     #   pydantic-settings
 pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
     # via authx
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   mkdocs-material
     #   rich
 pyinstrument==4.6.2
     # via authx-extra
 pyjwt==2.8.0
     # via authx
@@ -164,43 +181,48 @@
     #   mkdocs-mermaid2-plugin
     #   mkdocstrings
 python-dateutil==2.9.0.post0
     # via
     #   authx
     #   ghp-import
 python-dotenv==1.0.1
-    # via pydantic-settings
+    # via
+    #   pydantic-settings
+    #   uvicorn
 python-jose==3.3.0
     # via authx
+python-multipart==0.0.9
+    # via fastapi
 pytz==2024.1
     # via authx
 pyyaml==6.0.1
     # via
     #   mkdocs
     #   mkdocs-get-deps
     #   mkdocs-markdownextradata-plugin
     #   pymdown-extensions
     #   pyyaml-env-tag
+    #   uvicorn
 pyyaml-env-tag==0.1
     # via mkdocs
 rcslice==1.1.0
     # via mdx-include
 redis==5.0.4
     # via authx-extra
-regex==2024.4.28
+regex==2024.5.15
     # via mkdocs-material
-requests==2.31.0
+requests==2.32.2
     # via
     #   mkdocs-material
     #   mkdocs-mermaid2-plugin
 rich==13.7.1
     # via typer
 rsa==4.9
     # via python-jose
-setuptools==69.5.1
+setuptools==70.0.0
     # via mkdocs-mermaid2-plugin
 shellingham==1.5.4
     # via typer
 six==1.16.0
     # via
     #   ecdsa
     #   jsbeautifier
@@ -214,24 +236,36 @@
 starlette==0.37.2
     # via fastapi
 tinycss2==1.3.0
     # via
     #   cairosvg
     #   cssselect2
 typer==0.12.3
-    # via typer-cli
+    # via
+    #   fastapi-cli
+    #   typer-cli
 typer-cli==0.12.3
 typing-extensions==4.11.0
     # via
     #   fastapi
     #   griffe-typingdoc
     #   pydantic
     #   pydantic-core
     #   typer
+ujson==5.10.0
+    # via fastapi
 urllib3==2.2.1
     # via requests
+uvicorn==0.29.0
+    # via fastapi
+uvloop==0.19.0
+    # via uvicorn
 watchdog==4.0.0
     # via mkdocs
+watchfiles==0.21.0
+    # via uvicorn
 webencodings==0.5.1
     # via
     #   cssselect2
     #   tinycss2
+websockets==12.0
+    # via uvicorn
```

### Comparing `authx-1.1.2/requirements/linting.txt` & `authx-1.1.3/requirements/linting.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile requirements/linting.in -o requirements/linting.txt
 black==24.4.2
 cfgv==3.4.0
     # via pre-commit
 click==8.1.7
     # via black
+codespell==2.2.6
 distlib==0.3.8
     # via virtualenv
 filelock==3.14.0
     # via virtualenv
 identify==2.5.36
     # via pre-commit
 mypy==1.10.0
@@ -18,24 +19,24 @@
     #   mypy
 nodeenv==1.8.0
     # via pre-commit
 packaging==24.0
     # via black
 pathspec==0.12.1
     # via black
-platformdirs==4.2.1
+platformdirs==4.2.2
     # via
     #   black
     #   virtualenv
-pre-commit==3.7.0
+pre-commit==3.7.1
 pyupgrade==3.15.2
 pyyaml==6.0.1
     # via pre-commit
-ruff==0.4.2
-setuptools==69.5.1
+ruff==0.4.4
+setuptools==70.0.0
     # via nodeenv
 tokenize-rt==5.2.0
     # via pyupgrade
 typing-extensions==4.11.0
     # via mypy
-virtualenv==20.26.1
+virtualenv==20.26.2
     # via pre-commit
```

### Comparing `authx-1.1.2/requirements/pyproject.txt` & `authx-1.1.3/requirements/pyproject.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile pyproject.toml -o requirements/pyproject.txt
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 anyio==4.3.0
     # via starlette
 cffi==1.16.0
     # via cryptography
-cryptography==42.0.5
+cryptography==42.0.7
     # via pyjwt
 ecdsa==0.19.0
     # via python-jose
-fastapi==0.110.3
+fastapi-slim==0.111.0
 idna==3.7
     # via anyio
 pyasn1==0.6.0
     # via
     #   python-jose
     #   rsa
 pycparser==2.22
     # via cffi
 pydantic==2.7.1
     # via
-    #   fastapi
+    #   fastapi-slim
     #   pydantic-settings
 pydantic-core==2.18.2
     # via pydantic
 pydantic-settings==2.2.1
 pyjwt==2.8.0
 python-dateutil==2.9.0.post0
 python-dotenv==1.0.1
@@ -37,13 +37,13 @@
 six==1.16.0
     # via
     #   ecdsa
     #   python-dateutil
 sniffio==1.3.1
     # via anyio
 starlette==0.37.2
-    # via fastapi
+    # via fastapi-slim
 typing-extensions==4.11.0
     # via
-    #   fastapi
+    #   fastapi-slim
     #   pydantic
     #   pydantic-core
```

### Comparing `authx-1.1.2/requirements/testing.txt` & `authx-1.1.3/requirements/testing.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 certifi==2024.2.2
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.3.2
     # via requests
-coverage==7.5.0
+coverage==7.5.1
     # via pytest-cov
-freezegun==1.5.0
+freezegun==1.5.1
 h11==0.14.0
     # via httpcore
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
 idna==3.7
     # via
@@ -25,28 +25,28 @@
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.2.0
 packaging==24.0
     # via pytest
 pluggy==1.5.0
     # via pytest
-pytest==8.2.0
+pytest==8.2.1
     # via
     #   pytest-asyncio
     #   pytest-cov
-pytest-asyncio==0.23.6
+pytest-asyncio==0.23.7
 pytest-cov==5.0.0
 python-dateutil==2.9.0.post0
     # via freezegun
-requests==2.31.0
+requests==2.32.2
 six==1.16.0
     # via python-dateutil
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
-sqlalchemy==2.0.29
+sqlalchemy==2.0.30
 typing-extensions==4.11.0
     # via sqlalchemy
 urllib3==2.2.1
     # via requests
 websockets==12.0
```

### Comparing `authx-1.1.2/scripts/clean.sh` & `authx-1.1.3/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/test_authx.py` & `authx-1.1.3/tests/test_authx.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/test_callback.py` & `authx-1.1.3/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/test_config.py` & `authx-1.1.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/test_core.py` & `authx-1.1.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/test_dependencies.py` & `authx-1.1.3/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/test_errors.py` & `authx-1.1.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/test_schema.py` & `authx-1.1.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/test_token.py` & `authx-1.1.3/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/utils.py` & `authx-1.1.3/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,18 +215,18 @@
         data: dict,
     ):
         if "subject" in data:
             RESOURCES.append(data)
             return {"resource": data}
         return {"message": "Subject not found", "data": data}
 
-    @app.get("/entitiy/subjects", dependencies=[security.CURRENT_SUBJECT])
+    @app.get("/entity/subjects", dependencies=[security.CURRENT_SUBJECT])
     async def _subjects_route():
         return {"subjects": list(USER_DB.values())}
 
-    @app.get("/entitiy/subject")
+    @app.get("/entity/subject")
     async def _subject_route(subject: dict = security.CURRENT_SUBJECT):
         return {"subject": subject}
 
     @app.get("/entity/subject/resources")
     async def _subject_resources_route(subject: dict = security.CURRENT_SUBJECT):
         return {"resources": [r for r in RESOURCES if subject["uid"] == r["subject"]]}
```

### Comparing `authx-1.1.2/tests/app/conftest.py` & `authx-1.1.3/tests/app/conftest.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/app/test_access_location.py` & `authx-1.1.3/tests/app/test_access_location.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/app/test_blocklist_token.py` & `authx-1.1.3/tests/app/test_blocklist_token.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/app/test_fresh_token.py` & `authx-1.1.3/tests/app/test_fresh_token.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/app/test_get_subject.py` & `authx-1.1.3/tests/app/test_get_subject.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import pytest
 
 import authx.exceptions as exc
 
 
 def test_no_authorization_get_subject(api):
     with pytest.raises(exc.MissingTokenError):
-        api.get("/entitiy/subject")
+        api.get("/entity/subject")
 
 
 def test_get_subject_access_token(api, access_token: str):
     response = api.get(
-        "/entitiy/subject", headers={"Authorization": f"Bearer {access_token}"}
+        "/entity/subject", headers={"Authorization": f"Bearer {access_token}"}
     )
     assert response.status_code == 200
 
 
 def test_get_subject_refresh_token(api, refresh_token: str):
     with pytest.raises(exc.AccessTokenRequiredError):
-        api.get(
-            "/entitiy/subject", headers={"Authorization": f"Bearer {refresh_token}"}
-        )
+        api.get("/entity/subject", headers={"Authorization": f"Bearer {refresh_token}"})
 
 
 def test_get_subject(api, access_token: str):
     response = api.get(
-        "/entitiy/subject", headers={"Authorization": f"Bearer {access_token}"}
+        "/entity/subject", headers={"Authorization": f"Bearer {access_token}"}
     )
     assert response.status_code == 200
     assert response.json()["subject"]["uid"] == "test"
     assert response.json()["subject"]["email"] == "test@test.com"
 
 
 def test_get_subject_resources(api, access_token: str):
```

### Comparing `authx-1.1.2/tests/app/test_token_protected_access.py` & `authx-1.1.3/tests/app/test_token_protected_access.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/internal/test_logger.py` & `authx-1.1.3/tests/internal/test_logger.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/internal/test_memory.py` & `authx-1.1.3/tests/internal/test_memory.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/internal/test_signature.py` & `authx-1.1.3/tests/internal/test_signature.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/tests/internal/test_utils.py` & `authx-1.1.3/tests/internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/.gitignore` & `authx-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/README.md` & `authx-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `authx-1.1.2/pyproject.toml` & `authx-1.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-fancy-pypi-readme>=22.5.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "authx"
 description = "Ready to use and customizable Authentications and Oauth2 management for FastAPI"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -42,15 +42,15 @@
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "fastapi >=0.100.0,<0.120.0",
+    "fastapi-slim >=0.111.0",
     "pyjwt[crypto] >=2.6.0,<3.0.0",
     "pydantic >=2.0.0,<3.0.0",
     "pydantic-settings >=2.1.0",
     "python-dateutil>=2.8,<3.0.0",
     "pytz>=2023.3,<2025.0",
     "python-jose>=3.3.0,<4.0.0",
 ]
@@ -60,19 +60,47 @@
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project.urls]
 Homepage = "https://github.com/yezz123/authx"
 Documentation = "https://authx.yezz.me/"
 Funding = 'https://github.com/sponsors/yezz123'
-
+Source = 'https://github.com/yezz123/authx'
+Changelog = 'https://authx.yezz.me/release/'
 
 [tool.hatch.version]
 path = "authx/__init__.py"
 
+[tool.hatch.build.targets.sdist]
+# limit which files are included in the sdist (.tar.gz) asset,
+# to exclude unnecessary files and directories from the distribution
+include = [
+    '/README.md',
+    '/docs/release.md',
+    '/scripts',
+    '/authx',
+    '/tests',
+    '/requirements',
+]
+
+[tool.hatch.metadata.hooks.fancy-pypi-readme]
+content-type = 'text/markdown'
+# construct the PyPI readme from README.md and HISTORY.md
+fragments = [
+    {path = "README.md"},
+    {text = "\n## Changelog\n\n"},
+    {path = "docs/release.md", pattern = "(.+?)<!-- package description limit -->"},
+    {text = "\n... see [here](https://authx.yezz.me/release/#100b0) for earlier changes.\n"},
+]
+# convert GitHuB issue/PR numbers and handles to links
+substitutions = [
+    {pattern = '(\s+)#(\d+)', replacement = '\1[#\2](https://github.com/yezz123/authx/issues/\2)'},
+    {pattern = '(\s+)@([\w\-]+)', replacement = '\1[@\2](https://github.com/\2)'},
+    {pattern = '@@', replacement = '@'},
+]
 
 [tool.ruff.lint]
 mccabe = { max-complexity = 14 }
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
@@ -132,7 +160,11 @@
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format= "%Y-%m-%d %H:%M:%S"
 asyncio_mode= "auto"
 filterwarnings = [
     'error',
     'ignore::DeprecationWarning',
 ]
+
+[tool.codespell]
+skip = '.git,env*,__pycache__,.venv'
+ignore-words-list = 'ines,ser'
```

