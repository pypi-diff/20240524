# Comparing `tmp/ludic-0.4.2.tar.gz` & `tmp/ludic-0.4.3.tar.gz`

## Comparing `ludic-0.4.2.tar` & `ludic-0.4.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.2/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.2/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/catalog.md
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/getting-started.md
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.2/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/README.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/bulk_update.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/click_to_edit.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/click_to_load.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/delete_row.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/edit_row.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/infinite_scroll.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.2/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/__init__.py
--rw-r--r--   0        0        0    16478 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/attrs.py
--rw-r--r--   0        0        0    10138 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/components.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/format.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/utils.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/forms.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/headers.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/items.py
--rw-r--r--   0        0        0     6627 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/layouts.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/lists.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/loaders.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/messages.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/pages.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/tables.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/typography.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/collect.py
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/themes.py
--rw-r--r--   0        0        0    24350 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/types.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/__init__.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/parsers.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/responses.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.4.2/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_components.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_exceptions.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_formatting.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/test_types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/styles/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/styles/test_styles.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/styles/test_themes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.2/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.2/LICENCE
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.2/README.md
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 ludic-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.3/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.3/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/catalog.md
+-rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/getting-started.md
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.3/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/README.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/click_to_load.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/infinite_scroll.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.3/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/__init__.py
+-rw-r--r--   0        0        0    16518 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/attrs.py
+-rw-r--r--   0        0        0    10138 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/components.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/format.py
+-rw-r--r--   0        0        0    12114 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/headers.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/items.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/messages.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/styles/collect.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/styles/themes.py
+-rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/styles/types.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/responses.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.4.3/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/test_components.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.3/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.3/LICENCE
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.3/README.md
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 ludic-0.4.3/PKG-INFO
```

### Comparing `ludic-0.4.2/.pre-commit-config.yaml` & `ludic-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/CONTRIBUTING.md` & `ludic-0.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/mkdocs.yaml` & `ludic-0.4.3/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/.github/workflows/publish.yaml` & `ludic-0.4.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/.github/workflows/test.yaml` & `ludic-0.4.3/.github/workflows/test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -52,10 +52,10 @@
         python -m pip install .[full,test]
 
     - name: Test with pytest
       run: |
         pytest --cov --cov-report xml:coverage.xml
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v4.3.0
+      uses: codecov/codecov-action@v4.4.1
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `ludic-0.4.2/docs/catalog.md` & `ludic-0.4.3/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/docs/components.md` & `ludic-0.4.3/docs/components.md`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
 ### Pre-defined Attributes
 
 The `ludic.attrs` module contains many attribute definition that you can reuse in your components, here are the most used ones:
 
 - `HtmlAttrs` - Global HTML attributes available in all elements
     - The `class` and `for` attributes have the aliases `class_` and `for_`
-- `EventAttrs` - Event HTML attributes like `onclick`, `onkey`, and so on.
+- `EventAttrs` - Event HTML attributes like `on_click`, `on_key`, and so on.
 - `HtmxAttrs` - All [HTMX attributes](https://htmx.org/reference/) available.
     - All HTMX attributes have aliases with underscore, e.g. `hx_target`
 - `GlobalAttrs` subclasses `HtmlAttrs`, `EventAttrs` and `HtmxAttrs`
 - `[HtmlElementName]Attrs` - e.g. `ButtonAttrs`, `TdAttrs`, and so on.
 
 ## HTML Elements
```

### Comparing `ludic-0.4.2/docs/getting-started.md` & `ludic-0.4.3/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/docs/htmx.md` & `ludic-0.4.3/docs/htmx.md`

 * *Files 0% similar despite different names*

```diff
@@ -104,10 +104,10 @@
 from your_app.server import app
 
 @app.get("/data")
 def data() -> div:
     return div(
         h2("Data"),
         table(...),
-        button("Click Here", onclick=JavaScript("alert('test')")),
+        button("Click Here", on_click=JavaScript("alert('test')")),
     )
 ```
```

### Comparing `ludic-0.4.2/docs/index.md` & `ludic-0.4.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/docs/styles.md` & `ludic-0.4.3/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/docs/web-framework.md` & `ludic-0.4.3/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/docs/assets/ludic.png` & `ludic-0.4.3/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/examples/README.md` & `ludic-0.4.3/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/examples/__init__.py` & `ludic-0.4.3/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/examples/bulk_update.py` & `ludic-0.4.3/examples/bulk_update.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/examples/click_to_edit.py` & `ludic-0.4.3/examples/click_to_edit.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/examples/click_to_load.py` & `ludic-0.4.3/examples/click_to_load.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/examples/delete_row.py` & `ludic-0.4.3/examples/delete_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     @classmethod
     def get(cls) -> Self:
         return cls(people=[person.dict() for person in db.people.values()])
 
     @override
     def render(self) -> Table[TableHead, PersonRow]:
-        return Table[TableHead, PersonRow](
+        return Table(
             TableHead("Name", "Email", "Active", ""),
             *(PersonRow(**person) for person in self.attrs["people"]),
             body_attrs=HtmxAttrs(
                 hx_confirm="Are you sure?",
                 hx_target="closest tr",
                 hx_swap="outerHTML swap:1s",
             ),
```

### Comparing `ludic-0.4.2/examples/edit_row.py` & `ludic-0.4.3/examples/edit_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/examples/infinite_scroll.py` & `ludic-0.4.3/examples/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/examples/lazy_loading.py` & `ludic-0.4.3/examples/lazy_loading.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/attrs.py` & `ludic-0.4.3/ludic/attrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,14 +510,15 @@
 
 
 class IframeAttrs(GlobalAttrs, total=False):
     allow: str
     allowfullscreen: bool
     allowpaymentrequest: bool
     height: int
+    frameborder: str
     loading: Literal["eager", "lazy"]
     name: str
     referrerpolicy: Literal[
         "no-referrer",
         "no-referrer-when-downgrade",
         "origin",
         "origin-when-cross-origin",
@@ -531,14 +532,15 @@
         "allow-popups",
         "allow-same-origin",
         "allow-scripts",
         "allow-top-navigation",
     ]
     src: str
     srcdoc: str
+    scrolling: str
     width: int
 
 
 class ColAttrs(GlobalAttrs, total=False):
     span: int
```

### Comparing `ludic-0.4.2/ludic/base.py` & `ludic-0.4.3/ludic/base.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/components.py` & `ludic-0.4.3/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/format.py` & `ludic-0.4.3/ludic/format.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/html.py` & `ludic-0.4.3/ludic/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,14 +428,15 @@
 
 class html(ElementStrict[head, body, HtmlTagAttrs]):
     html_header = "<!doctype html>"
     html_name = "html"
 
 
 class iframe(Element[NoChildren, IframeAttrs]):
+    always_pair = True
     html_name = "iframe"
 
 
 class article(Element[AnyChildren, GlobalAttrs]):
     html_name = "article"
```

### Comparing `ludic-0.4.2/ludic/types.py` & `ludic-0.4.3/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/utils.py` & `ludic-0.4.3/ludic/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/catalog/forms.py` & `ludic-0.4.3/ludic/catalog/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     classes = ["form-field"]
     styles = style.use(
         lambda theme: {
             ".form-field": {
                 "label": {
                     "display": "block",
                     "font-weight": "bold",
-                    "margin": f"{theme.sizes.xxxs} 0 {theme.sizes.xxs}",
+                    "margin-block-end": theme.sizes.xxs,
                 },
                 "input": {
                     "inline-size": "100%",
                     "padding": f"{theme.sizes.xxxs} {theme.sizes.xs}",
                     "border": f"1px solid {theme.colors.light.darken(2)}",
                     "border-radius": theme.rounding.normal,
                     "box-sizing": "border-box",
```

### Comparing `ludic-0.4.2/ludic/catalog/headers.py` & `ludic-0.4.3/ludic/catalog/headers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/catalog/items.py` & `ludic-0.4.3/ludic/catalog/items.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Iterable
 from typing import override
 
 from ludic.attrs import GlobalAttrs
-from ludic.html import dd, dl, dt, style
+from ludic.html import dd, dl, dt
 from ludic.types import Component, PrimitiveChildren
 
 from .utils import attr_to_camel
 
 
 class Key(Component[PrimitiveChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``dt`` element."""
@@ -51,23 +51,14 @@
     Or alternatively:
 
         Pairs(
             items={"name": "John", "age": 42}.items(),
         )
     """
 
-    classes = ["stack", "small"]
-    styles = style.use(
-        lambda theme: {
-            ".stack.small > dt + dd": {
-                "margin-block-start": theme.sizes.xxxxs,
-            },
-        }
-    )
-
     @override
     def render(self) -> dl:
         from_items: list[Key | Value] = []
 
         for key, value in self.attrs.get("items", ()):
             from_items.append(Key(attr_to_camel(key)))
             from_items.append(Value(value))
```

### Comparing `ludic-0.4.2/ludic/catalog/layouts.py` & `ludic-0.4.3/ludic/catalog/layouts.py`

 * *Files 18% similar despite different names*

```diff
@@ -69,17 +69,23 @@
         )
     """
 
     classes = ["box"]
     styles = style.use(
         lambda theme: {
             ".box": {
-                "padding": theme.sizes.xl,
+                "padding": theme.sizes.l,
                 "color": theme.colors.dark,
             },
+            ".box.small": {
+                "padding": theme.sizes.s,
+            },
+            ".box.large": {
+                "padding": theme.sizes.xxl,
+            },
             ".box:not(.transparent)": {
                 "border": (
                     f"{theme.borders.thin} solid {theme.colors.light.darken(1)}"
                 ),
                 "border-radius": theme.rounding.more,
                 "background-color": theme.colors.light,
             },
@@ -248,7 +254,106 @@
                 f".switcher > :nth-last-child(n+{theme.layouts.switcher.limit+1})",
                 f".switcher > :nth-last-child(n+{theme.layouts.switcher.limit+1}) ~ *",
             ): {
                 "flex-basis": "100%",
             },
         }
     )
+
+
+class Cover(div):
+    """A component which covers the whole viewport.
+
+    Example usage:
+
+        Cover(
+            div(...),
+        )
+    """
+
+    classes = ["cover"]
+    styles = style.use(
+        lambda theme: {
+            ".cover": {
+                "display": "flex",
+                "flex-direction": "column",
+                "min-block-size": theme.layouts.cover.min_height,
+                "padding": theme.sizes.xxl,
+            },
+            ".cover > *": {
+                "margin-block": theme.sizes.xxl,
+            },
+            f".cover > :first-child:not({theme.layouts.cover.element})": {
+                "margin-block-start": "0",
+            },
+            f".cover > :last-child:not({theme.layouts.cover.element})": {
+                "margin-block-end": "0",
+            },
+            f".cover > {theme.layouts.cover.element}": {
+                "margin-block": "auto",
+            },
+        }
+    )
+
+
+class Grid(div):
+    """A component which creates a grid layout.
+
+    Example usage:
+
+        Grid(
+            div(...),
+            div(...),
+        )
+    """
+
+    classes = ["grid"]
+    styles = style.use(
+        lambda theme: {
+            ".grid": {
+                "display": "grid",
+                "grid-gap": theme.sizes.xxl,
+            },
+            f"@supports (width: min({theme.layouts.grid.cell_size}, 100%))": {
+                ".grid": {
+                    "grid-template-columns": (
+                        "repeat("
+                        "auto-fit,"
+                        f"minmax(min({theme.layouts.grid.cell_size},"
+                        "100%"
+                        "), 1fr))"
+                    ),
+                },
+            },
+        }
+    )
+
+
+class Frame(div):
+    """A component which creates a frame layout.
+
+    Example usage:
+
+        Frame(
+            div(...),
+        )
+    """
+
+    classes = ["frame"]
+    styles = style.use(
+        lambda theme: {
+            ".frame": {
+                "aspect-ratio": (
+                    f"{theme.layouts.frame.numerator}/{theme.layouts.frame.denominator}"
+                ),
+                "overflow": "hidden",
+                "display": "flex",
+                "justify-content": "center",
+                "align-items": "center",
+            },
+            (".frame > img", ".frame > video"): {
+                "inline-size": "100%",
+                "block-size": "100%",
+                "object-fit": "cover",
+            },
+        }
+    )
```

### Comparing `ludic-0.4.2/ludic/catalog/lists.py` & `ludic-0.4.3/ludic/catalog/lists.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/catalog/loaders.py` & `ludic-0.4.3/ludic/catalog/loaders.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,22 +11,22 @@
         lambda theme: {
             ".loader": {
                 "text-align": "center",
             },
             ".lds-ellipsis": {
                 "display": "inline-block",
                 "position": "relative",
-                "width": "80px",
-                "height": "80px",
+                "width": theme.sizes.m * 5,
+                "height": theme.sizes.m,
+                "margin": theme.sizes.xl,
             },
             ".lds-ellipsis div": {
                 "position": "absolute",
-                "top": "33px",
-                "width": "13px",
-                "height": "13px",
+                "width": theme.sizes.m,
+                "height": theme.sizes.m,
                 "border-radius": "50%",
                 "background": theme.colors.dark,
                 "animation-timing-function": "cubic-bezier(0, 1, 1, 0)",
             },
             ".lds-ellipsis div:nth-child(1)": {
                 "left": "8px",
                 "animation": "lds-ellipsis1 0.6s infinite",
```

### Comparing `ludic-0.4.2/ludic/catalog/messages.py` & `ludic-0.4.3/ludic/catalog/messages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/catalog/pages.py` & `ludic-0.4.3/ludic/catalog/pages.py`

 * *Files 24% similar despite different names*

```diff
@@ -101,19 +101,19 @@
             },
             ("code", "pre", "pre *"): {
                 "font-family": theme.fonts.mono,
             },
             "dl": {
                 "margin-block": "0",
             },
-            "dl dt": {
-                "margin-block-start": theme.sizes.xxs,
+            "dl dd + dt": {
+                "margin-block-start": theme.sizes.xs,
             },
-            "dl dd": {
-                "margin-block-start": theme.sizes.xxxs,
+            "dl dt + dd": {
+                "margin-block-start": theme.sizes.xxxxs,
             },
             "dt": {
                 "font-weight": "bold",
             },
             "dd": {
                 "margin-left": "0",
             },
@@ -125,43 +125,76 @@
             },
             "ul > li::marker": {
                 "font-size": theme.fonts.size * 1.2,
             },
             ("img", "svg"): {
                 "width": "100%",
             },
-            "button": {
-                "line-height": 1,
-            },
             # utilities
             ".text-align-center": {
-                "text-align": "center",
+                "text-align": "center !important",  # type: ignore[typeddict-item]
             },
             ".text-align-right": {
-                "text-align": "right",
+                "text-align": "right !important",  # type: ignore[typeddict-item]
             },
             ".text-align-left": {
-                "text-align": "left",
+                "text-align": "left !important",  # type: ignore[typeddict-item]
             },
-            ".no-border": {
-                "border": "none !important",
-                "border-radius": "0 !important",
+            ".justify-space-between": {
+                "justify-content": "space-between !important",  # type: ignore[typeddict-item]
+            },
+            ".justify-space-around": {
+                "justify-content": "space-around !important",  # type: ignore[typeddict-item]
+            },
+            ".justify-space-evenly": {
+                "justify-content": "space-evenly !important",  # type: ignore[typeddict-item]
+            },
+            ".justify-center": {
+                "justify-content": "center !important",  # type: ignore[typeddict-item]
+            },
+            ".justify-end": {
+                "justify-content": "end !important",  # type: ignore[typeddict-item]
+            },
+            ".justify-start": {
+                "justify-content": "start !important",  # type: ignore[typeddict-item]
+            },
+            ".align-center": {
+                "align-items": "center !important",  # type: ignore[typeddict-item]
+            },
+            ".align-end": {
+                "align-items": "end !important",  # type: ignore[typeddict-item]
+            },
+            ".align-start": {
+                "align-items": "start !important",  # type: ignore[typeddict-item]
             },
             ".no-padding": {
                 "padding": "0 !important",
             },
             ".no-inline-padding": {
                 "padding-inline": "0 !important",
             },
             ".no-margin": {
                 "margin": "0 !important",
             },
             ".no-inline-margin": {
                 "margin-inline": "0 !important",
             },
+            ".no-block-margin": {
+                "margin-block": "0 !important",
+            },
+            ".no-block-padding": {
+                "padding-block": "0 !important",
+            },
+            ".no-border": {
+                "border": "none !important",
+                "border-radius": "0 !important",
+            },
+            ".no-border-radius": {
+                "border-radius": "0 !important",
+            },
         }
     )
 
     @override
     def render(self) -> html:
         return html(
             self.children[0].render(),
```

### Comparing `ludic-0.4.2/ludic/catalog/quotes.py` & `ludic-0.4.3/ludic/catalog/quotes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/catalog/tables.py` & `ludic-0.4.3/ludic/catalog/tables.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/catalog/typography.py` & `ludic-0.4.3/ludic/catalog/typography.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from pygments.formatters import HtmlFormatter
     from pygments.lexers import get_lexer_by_name
 
     pygments_loaded = True
 except ImportError:
     pygments_loaded = False
 
-from ludic.attrs import GlobalAttrs
+from ludic.attrs import GlobalAttrs, HyperlinkAttrs
 from ludic.html import a, code, p, pre, style
 from ludic.types import (
     AnyChildren,
     Attrs,
     Component,
     ComponentStrict,
     PrimitiveChildren,
@@ -22,14 +22,15 @@
 
 from .utils import remove_whitespaces
 
 
 class LinkAttrs(Attrs):
     to: str
     external: NotRequired[bool]
+    classes: NotRequired[list[str]]
 
 
 class Link(ComponentStrict[PrimitiveChildren, LinkAttrs]):
     """Simple component simulating a link.
 
     The main difference between :class:`Link` and :class:`a` is that this component
     automatically adds the ``target="_blank"`` attribute to the link if the link
@@ -42,23 +43,25 @@
     Example usage:
 
         Link("Hello, World!", to="https://example.com")
     """
 
     @override
     def render(self) -> a:
-        attrs = {"href": self.attrs["to"]}
+        attrs: HyperlinkAttrs = {"href": self.attrs.get("to", "#")}
+        if "classes" in self.attrs:
+            attrs["classes"] = self.attrs["classes"]
 
         match self.attrs.get("external", "auto"):
             case True:
                 attrs["target"] = "_blank"
             case False:
                 pass
             case "auto":
-                if self.attrs["to"].startswith("http"):
+                if str(attrs["href"]).startswith("http"):
                     attrs["target"] = "_blank"
 
         return a(self.children[0], **attrs)
 
 
 class Paragraph(Component[AnyChildren, GlobalAttrs]):
     """Simple component simulating a paragraph.
@@ -114,15 +117,16 @@
     """
 
     classes = ["code-block"]
     styles = style.use(
         lambda theme: {
             ".code-block": {
                 "background-color": theme.colors.light,
-                "padding": theme.sizes.l,
+                "padding-block": theme.sizes.l,
+                "padding-inline": theme.sizes.xxl,
                 "font-size": theme.fonts.size * 0.9,
             },
         }
     )
 
     @override
     def render(self) -> pre:
```

### Comparing `ludic-0.4.2/ludic/catalog/utils.py` & `ludic-0.4.3/ludic/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/styles/collect.py` & `ludic-0.4.3/ludic/styles/collect.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/styles/themes.py` & `ludic-0.4.3/ludic/styles/themes.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 @dataclass
 class Colors:
     """Colors for a theme."""
 
     primary: Color = ColorRange(["#276662", "#4ecdc4", "#dbf5f3"])
-    secondary: Color = ColorRange(["#f1f1f1", "#fefefe", "#fff"])
+    secondary: Color = ColorRange(["#212529", "#414549", "#616569"])
     success: Color = ColorRange(["#637a32", "#c7f464", "#eefbd0"])
     info: Color = ColorRange(["#978801", "#fce303", "#fef9cc"])
     warning: Color = ColorRange(["#7e4801", "#fc9003", "#fee8cc"])
     danger: Color = ColorRange(["#711414", "#e32929", "#f9d4d4"])
 
     light: Color = Color("#f8f8f8")
     dark: Color = Color("#414549")
@@ -120,19 +120,52 @@
     threshold: Size = Size(40, "rem")
 
     # The maximum number of elements allowed to appear in the horizontal configuration
     limit: int = 4
 
 
 @dataclass
+class Cover:
+    """Cover layout config for a theme."""
+
+    # The minimum height of the cover
+    min_height: Size = Size(100, "vh")
+
+    # The minimum space between and around the child elements
+    element: str = "h1"
+
+
+@dataclass
+class Grid:
+    """Grid layout config for a theme."""
+
+    # The size of the grid cells
+    cell_size: Size = Size(250, "px")
+
+
+@dataclass
+class Frame:
+    """Frame layout config for a theme."""
+
+    # The width of the frame
+    numerator: int = 16
+
+    # The height of the frame
+    denominator: int = 9
+
+
+@dataclass
 class Layouts:
     """Layout configuration for a theme."""
 
     sidebar: Sidebar = field(default_factory=Sidebar)
     switcher: Switcher = field(default_factory=Switcher)
+    cover: Cover = field(default_factory=Cover)
+    grid: Grid = field(default_factory=Grid)
+    frame: Frame = field(default_factory=Frame)
 
 
 @dataclass
 class Theme(metaclass=ABCMeta):
     """An abstract base class for theme configuration."""
 
     measure: Size = Size(110, "ch")
```

### Comparing `ludic-0.4.2/ludic/styles/types.py` & `ludic-0.4.3/ludic/styles/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,15 @@
         ],
         "animation-duration": str,
         "animation-fill-mode": Literal["none", "forwards", "backwards", "both"],
         "animation-iteration-count": float,
         "animation-name": str,
         "animation-play-state": Literal["paused", "running"],
         "animation-timing-function": str,
+        "aspect-ratio": str,
         # B
         "backdrop-filter": str,
         "backface-visibility": Literal["visible", "hidden"],
         "background": str,
         "background-attachment": Literal["scroll", "fixed", "local"],
         "background-blend-mode": str,
         "background-clip": Literal["border-box", "padding-box", "content-box", "text"],
```

### Comparing `ludic-0.4.2/ludic/styles/utils.py` & `ludic-0.4.3/ludic/styles/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/web/app.py` & `ludic-0.4.3/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/web/datastructures.py` & `ludic-0.4.3/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/web/endpoints.py` & `ludic-0.4.3/ludic/web/endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 from collections.abc import Callable
-from typing import Any, ClassVar, Protocol, cast
+from typing import Any, ClassVar, Protocol
 
 from starlette.datastructures import URL
 from starlette.endpoints import HTTPEndpoint as BaseEndpoint
 from starlette.routing import Route
 
 from ludic.catalog.loaders import LazyLoader
 from ludic.types import AnyChildren, Component, NoChildren, TAttrs
@@ -47,14 +47,19 @@
 
 
 class Endpoint(Component[NoChildren, TAttrs]):
     """Base class for Ludic endpoints."""
 
     route: ClassVar[Route]
 
+    @property
+    def request(self) -> Request | None:
+        """The current request."""
+        return self.context.get("request")
+
     def lazy_load(
         self,
         endpoint: type[RoutedProtocol],
         placeholder: AnyChildren = "Loading ...",
         **kwargs: Any,
     ) -> LazyLoader:
         """Lazy load an endpoint's content.
@@ -75,17 +80,15 @@
         Args:
             endpoint: The endpoint.
             **path_params: URL path parameters.
 
         Returns:
             The URL.
         """
-        request = self.context.get("request")
-
-        if request is None or not isinstance(request, Request):
+        if self.request is None or not isinstance(self.request, Request):
             raise RuntimeError(
                 f"{type(self).__name__} is not bound to a request, you can only use "
                 f"the {type(self).__name__}.url_for method in the context of a request."
             )
 
         if inspect.isclass(endpoint) and issubclass(endpoint, Endpoint):
             endpoint_generic_args = get_element_generic_args(endpoint)
@@ -98,8 +101,8 @@
             ):
                 path_params = {
                     key: value
                     for key, value in {**self.attrs, **path_params}.items()
                     if key in endpoint.route.param_convertors
                 }
 
-        return cast(URL, request.url_for(endpoint, **path_params))
+        return self.request.url_for(endpoint, **path_params)
```

### Comparing `ludic-0.4.2/ludic/web/exceptions.py` & `ludic-0.4.3/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/web/parsers.py` & `ludic-0.4.3/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/web/requests.py` & `ludic-0.4.3/ludic/web/requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,24 +43,24 @@
         if isinstance(endpoint, str):
             endpoint_name = endpoint
         elif (route := getattr(endpoint, "route", None)) and isinstance(route, Route):
             endpoint_name = route.name
         else:
             raise NoMatchFound(str(endpoint), path_params)
 
-        if partial_mount := self.scope.get("partial_mount"):
-            try:
+        try:
+            return router.url_path_for(endpoint_name, **path_params)
+        except NoMatchFound as e:
+            if partial_mount := self.scope.get("partial_mount"):
                 return router.url_path_for(
                     join_mounts(partial_mount, endpoint_name),
                     **path_params,
                 )
-            except NoMatchFound:
-                return router.url_path_for(endpoint_name, **path_params)
-        else:
-            return router.url_path_for(endpoint_name, **path_params)
+            else:
+                raise e
 
     def url_for(self, endpoint: str | Callable[..., Any], /, **path_params: Any) -> URL:
         """Get URL for an endpoint.
 
         Args:
             endpoint: The endpoint to get the URL for, can be name or a registered
                 endpoint class.
```

### Comparing `ludic-0.4.2/ludic/web/responses.py` & `ludic-0.4.3/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/ludic/web/routing.py` & `ludic-0.4.3/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/tests/test_components.py` & `ludic-0.4.3/tests/test_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,32 +51,32 @@
         NavItem("Home", to="/"),
         NavItem("About", to="/about"),
         id="nav",
     )
     assert navigation.to_html() == (
         '<nav id="nav" class="navigation">'
             '<ul class="stack small">'
-                '<li class="nav-item"><a href="/" class="small btn link">Home</a></li>'
+                '<li class="nav-item"><a href="/" class="btn">Home</a></li>'
                 '<li class="nav-item">'
-                    '<a href="/about" class="small btn link">About</a>'
+                    '<a href="/about" class="btn">About</a>'
                 '</li>'
             "</ul>"
         "</nav>"
     )  # fmt: skip
 
 
 def test_pairs() -> None:
     pairs = Pairs(
         Key("Name"),
         Value("John"),
         Key("Age"),
         Value(42),
     )
     assert pairs.to_html() == (
-        '<dl class="stack small">'
+        '<dl>'
             '<dt>Name</dt>'
             '<dd>John</dd>'
             '<dt>Age</dt>'
             '<dd>42</dd>'
         "</dl>"
     )  # fmt: skip
```

### Comparing `ludic-0.4.2/tests/test_elements.py` & `ludic-0.4.3/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/tests/test_examples.py` & `ludic-0.4.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/tests/test_exceptions.py` & `ludic-0.4.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/tests/test_formatting.py` & `ludic-0.4.3/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/tests/test_types.py` & `ludic-0.4.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/tests/styles/__init__.py` & `ludic-0.4.3/tests/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/tests/styles/test_styles.py` & `ludic-0.4.3/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/tests/styles/test_themes.py` & `ludic-0.4.3/tests/styles/test_themes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/.gitignore` & `ludic-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/LICENCE` & `ludic-0.4.3/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/README.md` & `ludic-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/pyproject.toml` & `ludic-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.2/PKG-INFO` & `ludic-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.4.2
+Version: 0.4.3
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
```

