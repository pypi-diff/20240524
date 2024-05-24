# Comparing `tmp/invenio-administration-2.2.1.tar.gz` & `tmp/invenio-administration-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-administration-2.2.1.tar", last modified: Wed May 15 14:56:28 2024, max compression
+gzip compressed data, was "dist/invenio-administration-2.2.2.tar", last modified: Thu May 23 09:26:13 2024, max compression
```

## Comparing `invenio-administration-2.2.1.tar` & `invenio-administration-2.2.2.tar`

### file list

```diff
@@ -1,501 +1,501 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/routes.js
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/routes.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBulkActionContext.js
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)   132884 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/marshmallow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/menu/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/menu/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    32571 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/static/images/dashboard.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/create.html
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/details.html
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/header/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/header/side_bar_toggle.html
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/macros.html
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/search.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-15 14:56:26.000000 invenio-administration-2.2.1/invenio_administration/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-15 14:56:26.000000 invenio-administration-2.2.1/invenio_administration/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 14:56:26.000000 invenio-administration-2.2.1/invenio_administration/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-15 14:56:26.000000 invenio-administration-2.2.1/invenio_administration/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-15 14:56:26.000000 invenio-administration-2.2.1/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration/views/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14010 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/views/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/invenio_administration/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/invenio_administration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 14:56:27.000000 invenio-administration-2.2.1/invenio_administration.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      829 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/run-js-linter.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      980 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/mock_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:28.000000 invenio-administration-2.2.1/tests/mock_module/administration/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/mock_module/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/mock_module/administration/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/mock_module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/mock_module/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/test_admin_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/test_details_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/test_invenio_administration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/test_list_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-15 14:56:20.000000 invenio-administration-2.2.1/tests/test_marshmallow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/routes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/routes.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBulkActionContext.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)   132884 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/marshmallow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/menu/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    32571 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/static/images/dashboard.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/create.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/header/
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/header/side_bar_toggle.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/search.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/views/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/invenio_administration/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/invenio_administration.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      829 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/run-js-linter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      980 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/mock_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:13.000000 invenio-administration-2.2.2/tests/mock_module/administration/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/mock_module/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/mock_module/administration/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/mock_module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/mock_module/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/test_admin_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/test_details_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/test_invenio_administration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/test_list_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-23 09:26:05.000000 invenio-administration-2.2.2/tests/test_marshmallow_utils.py
```

### Comparing `invenio-administration-2.2.1/.editorconfig` & `invenio-administration-2.2.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/.github/workflows/i18n-push.yml` & `invenio-administration-2.2.2/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/.github/workflows/pypi-publish.yml` & `invenio-administration-2.2.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/.github/workflows/tests.yml` & `invenio-administration-2.2.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/.tx/config` & `invenio-administration-2.2.2/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/CHANGES.rst` & `invenio-administration-2.2.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     invenio-administration is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 2.2.2 (released 2024-05-23)
+
+- views: allow list view to receive a pid_value
+
 Version 2.2.1 (released 2024-05-15)
 
 - remove implicit dependency on oai_pmh view
 
 Version 2.2.0 (released 2024-03-22)
 
 - fix: before_first_request deprecation (move to finalize app entry point)
```

### Comparing `invenio-administration-2.2.1/CONTRIBUTING.rst` & `invenio-administration-2.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/MANIFEST.in` & `invenio-administration-2.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/PKG-INFO` & `invenio-administration-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-administration
-Version: 2.2.1
+Version: 2.2.2
 Summary: Invenio module that adds administration panel to the system.
 Home-page: https://github.com/inveniosoftware/invenio-administration
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             invenio-administration is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 2.2.2 (released 2024-05-23)
+        
+        - views: allow list view to receive a pid_value
+        
         Version 2.2.1 (released 2024-05-15)
         
         - remove implicit dependency on oai_pmh view
         
         Version 2.2.0 (released 2024-03-22)
         
         - fix: before_first_request deprecation (move to finalize app entry point)
```

### Comparing `invenio-administration-2.2.1/README.rst` & `invenio-administration-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/docs/Makefile` & `invenio-administration-2.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/docs/conf.py` & `invenio-administration-2.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/docs/index.rst` & `invenio-administration-2.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/docs/make.bat` & `invenio-administration-2.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/admin.py` & `invenio-administration-2.2.2/invenio_administration/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBulkActionContext.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBulkActionContext.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_AT/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de_DE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_AT/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en_HU/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_CU/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es_MX/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa_IR/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_CI/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr_FR/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hi_IN/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu_HU/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ne/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv_SE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk_UA/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot` & `invenio-administration-2.2.2/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/config.py` & `invenio-administration-2.2.2/invenio_administration/config.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/errors.py` & `invenio-administration-2.2.2/invenio_administration/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/ext.py` & `invenio-administration-2.2.2/invenio_administration/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/generators.py` & `invenio-administration-2.2.2/invenio_administration/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/marshmallow_utils.py` & `invenio-administration-2.2.2/invenio_administration/marshmallow_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/menu/menu.py` & `invenio-administration-2.2.2/invenio_administration/menu/menu.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/static/images/dashboard.png` & `invenio-administration-2.2.2/invenio_administration/static/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/base.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/base.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/create.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/create.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/details.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/details.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/edit.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/edit.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/index.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/index.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/search.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/search.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html` & `invenio-administration-2.2.2/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/af/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/af/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ar/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ar/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/bg/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/bg/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ca/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ca/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/cs/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/cs/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/da/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/da/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/de/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/de/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/el/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/el/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/en/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/en/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/es/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/es/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/et/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/et/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fa/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fa/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fr/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fr/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/gl/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/gl/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/hr/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/hr/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/hu/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/hu/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/it/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/it/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ja/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ja/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ka/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ka/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/lt/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/lt/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/messages.pot` & `invenio-administration-2.2.2/invenio_administration/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ne/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ne/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/no/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/no/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/pl/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/pl/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/pt/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/pt/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ro/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ro/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ru/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/ru/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/rw/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/rw/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/sk/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/sk/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/sv/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/sv/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/tr/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/tr/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/uk/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/uk/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-administration-2.2.2/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-administration-2.2.2/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/views/base.py` & `invenio-administration-2.2.2/invenio_administration/views/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,40 +381,44 @@
 
     def get_available_facets(self):
         """Get search available facets."""
         if not self.available_facets:
             return self.resource.service.config.search.facets
         return self.available_facets
 
-    def get(self):
-        """GET view method."""
+    def get_context(self, **kwargs):
+        """Create details view context."""
         search_conf = self.init_search_config()
         schema = self.get_service_schema()
         serialized_schema = self._schema_to_json(schema)
-        return self.render(
-            **{
-                "search_config": search_conf,
-                "title": self.title,
-                "name": self.name,
-                "resource_schema": serialized_schema,
-                "fields": self.item_field_list,
-                "display_search": self.display_search,
-                "display_create": self.display_create,
-                "display_edit": self.display_edit,
-                "display_delete": self.display_delete,
-                "display_read": self.display_read,
-                "actions": self.serialize_actions(),
-                "pid_path": self.pid_path,
-                "create_ui_endpoint": self.get_create_view_endpoint(),
-                "list_ui_endpoint": self.get_list_view_endpoint(),
-                "resource_name": (
-                    self.resource_name if self.resource_name else self.pid_path
-                ),
-            }
-        )
+        pid_value = kwargs.get("pid_value", "")
+        return {
+            "search_config": search_conf,
+            "title": self.title,
+            "name": self.name,
+            "resource_schema": serialized_schema,
+            "fields": self.item_field_list,
+            "display_search": self.display_search,
+            "display_create": self.display_create,
+            "display_edit": self.display_edit,
+            "display_delete": self.display_delete,
+            "display_read": self.display_read,
+            "actions": self.serialize_actions(),
+            "pid_path": self.pid_path,
+            "pid_value": pid_value,
+            "create_ui_endpoint": self.get_create_view_endpoint(),
+            "list_ui_endpoint": self.get_list_view_endpoint(),
+            "resource_name": (
+                self.resource_name if self.resource_name else self.pid_path
+            ),
+        }
+
+    def get(self, **kwargs):
+        """GET view method."""
+        return self.render(**self.get_context(**kwargs))
 
 
 class AdminResourceViewSet:
     """View set based on resource.
 
     Provides a list view and a details view given the provided configuration.
     """
```

### Comparing `invenio-administration-2.2.1/invenio_administration/views/dashboard.py` & `invenio-administration-2.2.2/invenio_administration/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration/webpack.py` & `invenio-administration-2.2.2/invenio_administration/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration.egg-info/PKG-INFO` & `invenio-administration-2.2.2/invenio_administration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-administration
-Version: 2.2.1
+Version: 2.2.2
 Summary: Invenio module that adds administration panel to the system.
 Home-page: https://github.com/inveniosoftware/invenio-administration
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             invenio-administration is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 2.2.2 (released 2024-05-23)
+        
+        - views: allow list view to receive a pid_value
+        
         Version 2.2.1 (released 2024-05-15)
         
         - remove implicit dependency on oai_pmh view
         
         Version 2.2.0 (released 2024-03-22)
         
         - fix: before_first_request deprecation (move to finalize app entry point)
```

### Comparing `invenio-administration-2.2.1/invenio_administration.egg-info/SOURCES.txt` & `invenio-administration-2.2.2/invenio_administration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/invenio_administration.egg-info/requires.txt` & `invenio-administration-2.2.2/invenio_administration.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/run-js-linter.sh` & `invenio-administration-2.2.2/run-js-linter.sh`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/run-tests.sh` & `invenio-administration-2.2.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/setup.cfg` & `invenio-administration-2.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/tests/conftest.py` & `invenio-administration-2.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/tests/mock_module/administration/mock.py` & `invenio-administration-2.2.2/tests/mock_module/administration/mock.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/tests/mock_module/config.py` & `invenio-administration-2.2.2/tests/mock_module/config.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/tests/mock_module/ext.py` & `invenio-administration-2.2.2/tests/mock_module/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/tests/test_admin_menu.py` & `invenio-administration-2.2.2/tests/test_admin_menu.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/tests/test_base.py` & `invenio-administration-2.2.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/tests/test_invenio_administration.py` & `invenio-administration-2.2.2/tests/test_invenio_administration.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-2.2.1/tests/test_marshmallow_utils.py` & `invenio-administration-2.2.2/tests/test_marshmallow_utils.py`

 * *Files identical despite different names*

