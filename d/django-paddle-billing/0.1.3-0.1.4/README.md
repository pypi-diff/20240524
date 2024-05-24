# Comparing `tmp/django_paddle_billing-0.1.3.tar.gz` & `tmp/django_paddle_billing-0.1.4.tar.gz`

## Comparing `django_paddle_billing-0.1.3.tar` & `django_paddle_billing-0.1.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.safety-policy.yml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/Makefile
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/requirements.txt
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/.stale.yml
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/release-drafter.yml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/.gitignore
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/dataSources.xml
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/django-paddle-billing.iml
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/__init__.py
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/manage.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/admin.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/apps.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/models.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/schema.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/tests.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/urls.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/views.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/api.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/asgi.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/settings.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/urls.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/wsgi.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/__init__.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/api.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/apps.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/encoders.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/exceptions.py
--rw-r--r--   0        0        0    25427 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/models.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/settings.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/signals.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/tests.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/urls.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/utils.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/views.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/management/commands/sync_from_paddle.py
--rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/0001_initial.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/0002_alter_subscription_status.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/tests/test_encoder.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/LICENSE
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/README.md
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.safety-policy.yml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/Makefile
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/.stale.yml
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/release-drafter.yml
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.idea/dataSources.xml
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.idea/django-paddle-billing.iml
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/__init__.py
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/manage.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/admin.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/apps.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/models.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/schema.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/tests.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/urls.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/views.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/billing/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/django_billing/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/django_billing/api.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/django_billing/asgi.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/django_billing/settings.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/django_billing/urls.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/example/django_billing/django_billing/wsgi.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/__init__.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/api.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/apps.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/encoders.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/exceptions.py
+-rw-r--r--   0        0        0    25427 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/models.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/settings.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/signals.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/tests.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/urls.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/utils.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/views.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/management/commands/sync_from_paddle.py
+-rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/migrations/0001_initial.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/migrations/0002_alter_subscription_status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/src/django_paddle_billing/migrations/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/tests/test_encoder.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/README.md
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.4/PKG-INFO
```

### Comparing `django_paddle_billing-0.1.3/.safety-policy.yml` & `django_paddle_billing-0.1.4/.safety-policy.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/CODE_OF_CONDUCT.md` & `django_paddle_billing-0.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/CONTRIBUTING.md` & `django_paddle_billing-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/Makefile` & `django_paddle_billing-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/requirements.txt` & `django_paddle_billing-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/.stale.yml` & `django_paddle_billing-0.1.4/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/PULL_REQUEST_TEMPLATE.md` & `django_paddle_billing-0.1.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/dependabot.yml` & `django_paddle_billing-0.1.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/release-drafter.yml` & `django_paddle_billing-0.1.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `django_paddle_billing-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `django_paddle_billing-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/question.md` & `django_paddle_billing-0.1.4/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/workflows/build.yml` & `django_paddle_billing-0.1.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.github/workflows/test.yml` & `django_paddle_billing-0.1.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.idea/dataSources.xml` & `django_paddle_billing-0.1.4/.idea/dataSources.xml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.idea/django-paddle-billing.iml` & `django_paddle_billing-0.1.4/.idea/django-paddle-billing.iml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.idea/inspectionProfiles/Project_Default.xml` & `django_paddle_billing-0.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/example/django_billing/manage.py` & `django_paddle_billing-0.1.4/example/django_billing/manage.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/example/django_billing/billing/schema.py` & `django_paddle_billing-0.1.4/example/django_billing/billing/schema.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/example/django_billing/billing/views.py` & `django_paddle_billing-0.1.4/example/django_billing/billing/views.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/example/django_billing/billing/migrations/0001_initial.py` & `django_paddle_billing-0.1.4/example/django_billing/billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/example/django_billing/django_billing/api.py` & `django_paddle_billing-0.1.4/example/django_billing/django_billing/api.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/example/django_billing/django_billing/settings.py` & `django_paddle_billing-0.1.4/example/django_billing/django_billing/settings.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/example/django_billing/django_billing/urls.py` & `django_paddle_billing-0.1.4/example/django_billing/django_billing/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 Class-based views
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
+from django_paddle_billing.urls import urlpatterns as paddle_billing_urls
 from billing.urls import urlpatterns as billing_urls
 from django.contrib import admin
 from django.urls import path
 
 from .api import api
 
 urlpatterns = [
     path("admin/", admin.site.urls),
     path("api/", api.urls),
 ]
 urlpatterns += billing_urls
+urlpatterns += paddle_billing_urls
+
```

### Comparing `django_paddle_billing-0.1.3/src/django_paddle_billing/admin.py` & `django_paddle_billing-0.1.4/src/django_paddle_billing/admin.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/src/django_paddle_billing/models.py` & `django_paddle_billing-0.1.4/src/django_paddle_billing/models.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/src/django_paddle_billing/settings.py` & `django_paddle_billing-0.1.4/src/django_paddle_billing/settings.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/src/django_paddle_billing/signals.py` & `django_paddle_billing-0.1.4/src/django_paddle_billing/signals.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/src/django_paddle_billing/views.py` & `django_paddle_billing-0.1.4/src/django_paddle_billing/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,21 +73,21 @@
         """
         handle paddle webhook requests by
         - validating the payload signature
         - sending a django signal for each of the SUPPORTED_WEBHOOKS
         """
         payload = request.body.decode("utf-8")
         paddle_ip = request.META.get("HTTP_X_FORWARDED_FOR", "")
-        if app_settings["PADDLE_SANDBOX"] and paddle_ip not in app_settings["PADDLE_SANDBOX_IPS"]:
+        if app_settings.PADDLE_SANDBOX and paddle_ip not in app_settings.PADDLE_SANDBOX_IPS:
             return HttpResponseBadRequest("IP not allowed")
-        elif not app_settings["PADDLE_SANDBOX"] and paddle_ip not in app_settings["PADDLE_IPS"]:
+        elif not app_settings.PADDLE_SANDBOX and paddle_ip not in app_settings.PADDLE_IPS:
             return HttpResponseBadRequest("IP not allowed")
 
         is_valid = validate_webhook_signature(
-            request.META.get("HTTP_PADDLE_SIGNATURE", ""), request.body, app_settings["PADDLE_SECRET_KEY"]
+            request.META.get("HTTP_PADDLE_SIGNATURE", ""), request.body, app_settings.PADDLE_SECRET_KEY
         )
 
         if not is_valid:
             return HttpResponseBadRequest("Invalid signature")
         notification = NotificationPayload.model_validate(json.loads(payload))
 
         if not notification.event_type:
```

### Comparing `django_paddle_billing-0.1.3/src/django_paddle_billing/management/commands/sync_from_paddle.py` & `django_paddle_billing-0.1.4/src/django_paddle_billing/management/commands/sync_from_paddle.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/0001_initial.py` & `django_paddle_billing-0.1.4/src/django_paddle_billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/0002_alter_subscription_status.py` & `django_paddle_billing-0.1.4/src/django_paddle_billing/migrations/0002_alter_subscription_status.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/tests/test_encoder.py` & `django_paddle_billing-0.1.4/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/.gitignore` & `django_paddle_billing-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/LICENSE` & `django_paddle_billing-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/README.md` & `django_paddle_billing-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/pyproject.toml` & `django_paddle_billing-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.3/PKG-INFO` & `django_paddle_billing-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-paddle-billing
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django + Paddle Billing Integration
 Project-URL: Documentation, https://github.com/websideproject/django-paddle-billing#readme
 Project-URL: Issues, https://github.com/websideproject/django-paddle-billing/issues
 Project-URL: Source, https://github.com/websideproject/django-paddle-billing
 Author-email: Benjamin Gervan <benjamin@websideproject.com>
 License-Expression: MIT
 License-File: LICENSE
```

