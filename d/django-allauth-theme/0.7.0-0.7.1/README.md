# Comparing `tmp/django_allauth_theme-0.7.0.tar.gz` & `tmp/django_allauth_theme-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allauth_theme-0.7.0.tar", last modified: Fri May 24 14:08:03 2024, max compression
+gzip compressed data, was "django_allauth_theme-0.7.1.tar", last modified: Fri May 24 15:09:22 2024, max compression
```

## Comparing `django_allauth_theme-0.7.0.tar` & `django_allauth_theme-0.7.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1074 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/LICENSE
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      197 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/MANIFEST.in
--rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/PKG-INFO
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1994 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/README.md
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.709406 django_allauth_theme-0.7.0/allauth_theme/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      142 2024-05-24 14:07:32.000000 django_allauth_theme-0.7.0/allauth_theme/__init__.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1234 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.0/allauth_theme/app_settings.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      624 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.0/allauth_theme/context_processors.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      492 2024-05-24 13:46:59.000000 django_allauth_theme-0.7.0/allauth_theme/forms.py
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.709406 django_allauth_theme-0.7.0/allauth_theme/static/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/static/css/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)    12018 2024-05-24 13:45:30.000000 django_allauth_theme-0.7.0/allauth_theme/static/css/signup.css
--rw-rw-r--   0 ledil     (1000) ledil     (1000)    21356 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.0/allauth_theme/static/css/tailwind.css
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/static/img/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     4099 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.0/allauth_theme/static/img/google.png
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.709406 django_allauth_theme-0.7.0/allauth_theme/templates/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.709406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/account_inactive.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2453 2024-05-24 13:47:39.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2609 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/email.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1035 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/email_confirm.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1958 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/login.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      562 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/logout.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      623 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_change.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      867 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      550 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_done.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      875 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_from_key.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_from_key_done.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      485 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_set.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      793 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/signup.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      294 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/signup_closed.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      582 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/verification_sent.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1007 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/verified_email_required.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/openid/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       48 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/openid/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      473 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/openid/login.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      332 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/authentication_error.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       42 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1480 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/connections.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      861 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/login.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      495 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/login_cancelled.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      835 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/signup.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/snippets/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      786 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2150 2024-05-24 13:46:02.000000 django_allauth_theme-0.7.0/allauth_theme/urls.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2604 2024-05-24 13:46:40.000000 django_allauth_theme-0.7.0/allauth_theme/views.py
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/
--rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/PKG-INFO
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2028 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)        1 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       63 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/requires.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       14 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/top_level.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       38 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/setup.cfg
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1902 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/setup.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.507824 django_allauth_theme-0.7.1/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1074 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/LICENSE
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      197 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/MANIFEST.in
+-rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 15:09:22.507824 django_allauth_theme-0.7.1/PKG-INFO
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1994 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/README.md
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.487824 django_allauth_theme-0.7.1/allauth_theme/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      142 2024-05-24 15:08:55.000000 django_allauth_theme-0.7.1/allauth_theme/__init__.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1234 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.1/allauth_theme/app_settings.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      624 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.1/allauth_theme/context_processors.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      492 2024-05-24 13:46:59.000000 django_allauth_theme-0.7.1/allauth_theme/forms.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.483824 django_allauth_theme-0.7.1/allauth_theme/static/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.487824 django_allauth_theme-0.7.1/allauth_theme/static/css/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)    11785 2024-05-24 15:08:44.000000 django_allauth_theme-0.7.1/allauth_theme/static/css/signup.css
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)    21356 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.1/allauth_theme/static/css/tailwind.css
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.487824 django_allauth_theme-0.7.1/allauth_theme/static/img/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     4099 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.1/allauth_theme/static/img/google.png
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.483824 django_allauth_theme-0.7.1/allauth_theme/templates/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.483824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.499824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/account_inactive.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2453 2024-05-24 13:47:39.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2609 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/email.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1035 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/email_confirm.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1958 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/login.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      562 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/logout.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      623 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_change.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      867 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      550 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_done.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      875 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_from_key.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_from_key_done.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      485 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_set.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      793 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/signup.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      294 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/signup_closed.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      582 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/verification_sent.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1007 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/verified_email_required.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.499824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/openid/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       48 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/openid/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      473 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/openid/login.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.503824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      332 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/authentication_error.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       42 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1480 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/connections.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      861 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/login.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      495 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/login_cancelled.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      835 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/signup.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.503824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/snippets/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      786 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2150 2024-05-24 13:46:02.000000 django_allauth_theme-0.7.1/allauth_theme/urls.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2604 2024-05-24 13:46:40.000000 django_allauth_theme-0.7.1/allauth_theme/views.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.507824 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/
+-rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/PKG-INFO
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2028 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/SOURCES.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)        1 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/dependency_links.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       63 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/requires.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       14 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/top_level.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       38 2024-05-24 15:09:22.507824 django_allauth_theme-0.7.1/setup.cfg
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1902 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/setup.py
```

### Comparing `django_allauth_theme-0.7.0/LICENSE` & `django_allauth_theme-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/PKG-INFO` & `django_allauth_theme-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-theme
-Version: 0.7.0
+Version: 0.7.1
 Summary: An awesome and responsive django-allauth theme based on tailwind
 Home-page: http://pypi.python.org/pypi/django-allauth-theme/
 Author: Leonardo Di Lella
 Author-email: leonardo.dilella@mobileapart.com
 License: LICENSE
 Keywords: django auth account social openid twitter facebook oauth registration theme tailwindcss
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_allauth_theme-0.7.0/README.md` & `django_allauth_theme-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/app_settings.py` & `django_allauth_theme-0.7.1/allauth_theme/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/context_processors.py` & `django_allauth_theme-0.7.1/allauth_theme/context_processors.py`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/static/css/signup.css` & `django_allauth_theme-0.7.1/allauth_theme/static/css/signup.css`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,14 @@
     float: left;
 }
 
 .sign_up_menu li:first-child {
     margin-right: 25px;
 }
 
-.sign_in_up_modal .checkboxinput {
-    position: absolute;
-    left: 0;
-    top: 2px;
-}
-
 .h-screen {
     height: 100vh;
 }
 
 @media (min-width: 1024px) {
     .lg\:flex-row {
         flex-direction: row !important;
@@ -94,22 +88,14 @@
     background-color: rgb(249 250 251);
     padding: 0.625rem;
     font-size: .875rem;
     line-height: 1.25rem;
     color: rgb(17 24 39);
 }
 
-.sign_up_form label {
-    font-size: .875rem;
-    line-height: 1.25rem;
-    margin-bottom: 0.5rem;
-    display: block;
-    font-weight: 500;
-}
-
 .sign_up_form div.control-group {
     margin-bottom: 1rem;
 }
 
 .sign_up_form form {
     margin-top: 1rem;
 }
```

### Comparing `django_allauth_theme-0.7.0/allauth_theme/static/css/tailwind.css` & `django_allauth_theme-0.7.1/allauth_theme/static/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/static/img/google.png` & `django_allauth_theme-0.7.1/allauth_theme/static/img/google.png`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/base.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/base.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/email.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/email.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/email_confirm.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/login.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/logout.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/logout.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_change.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_change.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_done.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_from_key.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/signup.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/signup.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/verification_sent.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/verified_email_required.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/connections.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/login.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/signup.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html` & `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/urls.py` & `django_allauth_theme-0.7.1/allauth_theme/urls.py`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/allauth_theme/views.py` & `django_allauth_theme-0.7.1/allauth_theme/views.py`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/django_allauth_theme.egg-info/PKG-INFO` & `django_allauth_theme-0.7.1/django_allauth_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-theme
-Version: 0.7.0
+Version: 0.7.1
 Summary: An awesome and responsive django-allauth theme based on tailwind
 Home-page: http://pypi.python.org/pypi/django-allauth-theme/
 Author: Leonardo Di Lella
 Author-email: leonardo.dilella@mobileapart.com
 License: LICENSE
 Keywords: django auth account social openid twitter facebook oauth registration theme tailwindcss
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_allauth_theme-0.7.0/django_allauth_theme.egg-info/SOURCES.txt` & `django_allauth_theme-0.7.1/django_allauth_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.0/setup.py` & `django_allauth_theme-0.7.1/setup.py`

 * *Files identical despite different names*

