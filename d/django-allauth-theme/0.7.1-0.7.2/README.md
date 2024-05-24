# Comparing `tmp/django_allauth_theme-0.7.1.tar.gz` & `tmp/django_allauth_theme-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allauth_theme-0.7.1.tar", last modified: Fri May 24 15:09:22 2024, max compression
+gzip compressed data, was "django_allauth_theme-0.7.2.tar", last modified: Fri May 24 15:41:55 2024, max compression
```

## Comparing `django_allauth_theme-0.7.1.tar` & `django_allauth_theme-0.7.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.507824 django_allauth_theme-0.7.1/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1074 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/LICENSE
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      197 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/MANIFEST.in
--rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 15:09:22.507824 django_allauth_theme-0.7.1/PKG-INFO
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1994 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/README.md
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.487824 django_allauth_theme-0.7.1/allauth_theme/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      142 2024-05-24 15:08:55.000000 django_allauth_theme-0.7.1/allauth_theme/__init__.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1234 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.1/allauth_theme/app_settings.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      624 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.1/allauth_theme/context_processors.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      492 2024-05-24 13:46:59.000000 django_allauth_theme-0.7.1/allauth_theme/forms.py
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.483824 django_allauth_theme-0.7.1/allauth_theme/static/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.487824 django_allauth_theme-0.7.1/allauth_theme/static/css/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)    11785 2024-05-24 15:08:44.000000 django_allauth_theme-0.7.1/allauth_theme/static/css/signup.css
--rw-rw-r--   0 ledil     (1000) ledil     (1000)    21356 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.1/allauth_theme/static/css/tailwind.css
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.487824 django_allauth_theme-0.7.1/allauth_theme/static/img/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     4099 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.1/allauth_theme/static/img/google.png
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.483824 django_allauth_theme-0.7.1/allauth_theme/templates/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.483824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.499824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/account_inactive.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2453 2024-05-24 13:47:39.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2609 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/email.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1035 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/email_confirm.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1958 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/login.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      562 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/logout.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      623 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_change.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      867 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      550 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_done.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      875 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_from_key.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_from_key_done.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      485 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_set.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      793 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/signup.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      294 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/signup_closed.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      582 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/verification_sent.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1007 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/verified_email_required.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.499824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/openid/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       48 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/openid/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      473 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/openid/login.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.503824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      332 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/authentication_error.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       42 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1480 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/connections.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      861 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/login.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      495 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/login_cancelled.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      835 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/signup.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.503824 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/snippets/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      786 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2150 2024-05-24 13:46:02.000000 django_allauth_theme-0.7.1/allauth_theme/urls.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2604 2024-05-24 13:46:40.000000 django_allauth_theme-0.7.1/allauth_theme/views.py
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:09:22.507824 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/
--rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/PKG-INFO
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2028 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)        1 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       63 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/requires.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       14 2024-05-24 15:09:22.000000 django_allauth_theme-0.7.1/django_allauth_theme.egg-info/top_level.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       38 2024-05-24 15:09:22.507824 django_allauth_theme-0.7.1/setup.cfg
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1902 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.1/setup.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.886231 django_allauth_theme-0.7.2/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1074 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.2/LICENSE
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      197 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.2/MANIFEST.in
+-rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 15:41:55.886231 django_allauth_theme-0.7.2/PKG-INFO
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1994 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.2/README.md
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.882231 django_allauth_theme-0.7.2/allauth_theme/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      142 2024-05-24 15:37:44.000000 django_allauth_theme-0.7.2/allauth_theme/__init__.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1234 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/app_settings.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      624 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/context_processors.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      492 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/forms.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.878231 django_allauth_theme-0.7.2/allauth_theme/static/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.882231 django_allauth_theme-0.7.2/allauth_theme/static/css/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     9417 2024-05-24 15:41:17.000000 django_allauth_theme-0.7.2/allauth_theme/static/css/signup.css
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)    21659 2024-05-24 15:41:22.000000 django_allauth_theme-0.7.2/allauth_theme/static/css/tailwind.css
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.882231 django_allauth_theme-0.7.2/allauth_theme/static/img/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     4099 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/static/img/google.png
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.878231 django_allauth_theme-0.7.2/allauth_theme/templates/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.878231 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.882231 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/account_inactive.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2579 2024-05-24 15:39:19.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2609 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/email.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1035 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/email_confirm.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1963 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/login.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      562 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/logout.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      623 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_change.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      867 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_reset.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      550 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_reset_done.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      875 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_reset_from_key.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_reset_from_key_done.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      485 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_set.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      793 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/signup.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      294 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/signup_closed.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      582 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/verification_sent.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1007 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/verified_email_required.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.882231 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/openid/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       48 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/openid/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      473 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/openid/login.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.882231 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      332 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/authentication_error.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       42 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1480 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/connections.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      861 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/login.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      495 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/login_cancelled.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      835 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/signup.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.882231 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/snippets/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      786 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2150 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/urls.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2604 2024-05-24 15:37:22.000000 django_allauth_theme-0.7.2/allauth_theme/views.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 15:41:55.886231 django_allauth_theme-0.7.2/django_allauth_theme.egg-info/
+-rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 15:41:55.000000 django_allauth_theme-0.7.2/django_allauth_theme.egg-info/PKG-INFO
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2028 2024-05-24 15:41:55.000000 django_allauth_theme-0.7.2/django_allauth_theme.egg-info/SOURCES.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)        1 2024-05-24 15:41:55.000000 django_allauth_theme-0.7.2/django_allauth_theme.egg-info/dependency_links.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       63 2024-05-24 15:41:55.000000 django_allauth_theme-0.7.2/django_allauth_theme.egg-info/requires.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       14 2024-05-24 15:41:55.000000 django_allauth_theme-0.7.2/django_allauth_theme.egg-info/top_level.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       38 2024-05-24 15:41:55.886231 django_allauth_theme-0.7.2/setup.cfg
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1902 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.2/setup.py
```

### Comparing `django_allauth_theme-0.7.1/LICENSE` & `django_allauth_theme-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/PKG-INFO` & `django_allauth_theme-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-theme
-Version: 0.7.1
+Version: 0.7.2
 Summary: An awesome and responsive django-allauth theme based on tailwind
 Home-page: http://pypi.python.org/pypi/django-allauth-theme/
 Author: Leonardo Di Lella
 Author-email: leonardo.dilella@mobileapart.com
 License: LICENSE
 Keywords: django auth account social openid twitter facebook oauth registration theme tailwindcss
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_allauth_theme-0.7.1/README.md` & `django_allauth_theme-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/app_settings.py` & `django_allauth_theme-0.7.2/allauth_theme/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/context_processors.py` & `django_allauth_theme-0.7.2/allauth_theme/context_processors.py`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/static/css/tailwind.css` & `django_allauth_theme-0.7.2/allauth_theme/static/css/tailwind.css`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 body {
   margin: 0;
   /* 1 */
   line-height: inherit;
   /* 2 */
 }
 
+.h-screen {
+    height: 100vh;
+}
+
 /*
 1. Add the correct height in Firefox.
 2. Correct the inheritance of border color in Firefox. (https://bugzilla.mozilla.org/show_bug.cgi?id=190655)
 3. Ensure horizontal rules are visible by default.
 */
 
 hr {
@@ -171,14 +175,31 @@
   /* 1 */
   border-color: inherit;
   /* 2 */
   border-collapse: collapse;
   /* 3 */
 }
 
+.gap-x-3 {
+  -moz-column-gap: 0.75rem;
+       column-gap: 0.75rem;
+}
+
+.h-full {
+  height: 100%;
+}
+
+.top-\[25px\] {
+  top: 25px;
+}
+
+.right-\[25px\] {
+  right: 25px;
+}
+
 /*
 1. Change the font styles in all browsers.
 2. Remove the margin in Firefox and Safari.
 3. Remove default padding in all browsers.
 */
 
 button,
@@ -737,14 +758,26 @@
   margin: -1px;
   overflow: hidden;
   clip: rect(0, 0, 0, 0);
   white-space: nowrap;
   border-width: 0;
 }
 
+.float-left {
+  float:left;
+}
+
+.pt-5 {
+  padding-top: 1.25rem;
+}
+
+.mr-5 {
+  margin-right: 1.25rem;
+}
+
 .pointer-events-none {
   pointer-events: none;
 }
 
 .static {
   position: static;
 }
```

### Comparing `django_allauth_theme-0.7.1/allauth_theme/static/img/google.png` & `django_allauth_theme-0.7.2/allauth_theme/static/img/google.png`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/base.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -18,30 +18,30 @@
      data-auto_prompt="true">
 </div>
 <script src="https://accounts.google.com/gsi/client" async defer></script>
 {% endif %}
 {% block body %}
     <div class="flex lg:flex-row h-screen flex-col">
         <div class="lg:basis-1/2 basis-1 bg_svg lg:pt-0 pt-20">
-            <div class="sign_up_welcome_box lg:ml-20p lg:mr-100 lg:justify-end justify-center">
+            <div class="sign_up_welcome_box flex items-center h-full lg:ml-20p lg:mr-100 lg:justify-end justify-center">
                 <div class="px-10">
                     <h4 class="lg:block hidden text-2xl font-bold dark:text-white pb-2">{{ DAT_WELCOME_TITLE }}</h4>
                     <h3 class="lg:hidden text-2xl font-bold dark:text-white pb-2">{{ DAT_WELCOME_TITLE_MOBILE }}</h3>
                     <p class="lg:block hidden">{{ DAT_WELCOME_TEXT }}</p>
                 </div>
             </div>
         </div>
         <div class="basis-1/2 lg:mt-0 mt-12 lg:mb-0 mb-12 pl-10">
         {% if not request.user.is_authenticated %}
-            <ul class="sign_up_menu">
-                <li><a class="link" href="{% url 'account_login' %}">{% trans "Sign In" %}</a></li>
-                <li><a class="primaryAction" href="{% url 'account_signup' %}">{% trans "Sign Up" %}</a></li>
+            <ul class="sign_up_menu absolute top-[25px] right-[25px]">
+                <li class="float-left mr-5"><a class="link" href="{% url 'account_login' %}">{% trans "Sign In" %}</a></li>
+                <li class="float-left"><a class="primaryAction" href="{% url 'account_signup' %}">{% trans "Sign Up" %}</a></li>
             </ul>
         {% endif %}
-            <div class="sign_up_form lg:justify-start justify-center lg:ml-100 ml-0">
+            <div class="sign_up_form flex h-full items-center lg:justify-start justify-center lg:ml-100 ml-0">
                 <div>
                     {% if messages %}
                         <div class="bg-orange-100 border-l-4 border-orange-500 text-orange-700 p-4 mb-4" role="alert">
                             {% for message in messages %}
                                 <p>{{ message }}</p>
                             {% endfor %}
                         </div>
```

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/email.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/email.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/email_confirm.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/login.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/login.html`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             </div>
 
         {% else %}
             <p>{% blocktrans %}If you have not created an account yet, then please
                 <strong><a class="link" href="{{ signup_url }}">sign up</a></strong> first.{% endblocktrans %}</p>
         {% endif %}
 
-        <form class="login" method="POST" action="{% url 'account_login' %}">
+        <form class="login pt-5" method="POST" action="{% url 'account_login' %}">
             {% csrf_token %}
             {{ form|crispy }}
             {% if redirect_field_value %}
                 <input type="hidden" name="{{ redirect_field_name }}"
                        value="{{ redirect_field_value }}"/>
             {% endif %}
```

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/logout.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/logout.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_change.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_change.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_done.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/password_reset_from_key.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/signup.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/signup.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/verification_sent.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/account/verified_email_required.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/connections.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/login.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/signup.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html` & `django_allauth_theme-0.7.2/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/urls.py` & `django_allauth_theme-0.7.2/allauth_theme/urls.py`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/allauth_theme/views.py` & `django_allauth_theme-0.7.2/allauth_theme/views.py`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/django_allauth_theme.egg-info/PKG-INFO` & `django_allauth_theme-0.7.2/django_allauth_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-theme
-Version: 0.7.1
+Version: 0.7.2
 Summary: An awesome and responsive django-allauth theme based on tailwind
 Home-page: http://pypi.python.org/pypi/django-allauth-theme/
 Author: Leonardo Di Lella
 Author-email: leonardo.dilella@mobileapart.com
 License: LICENSE
 Keywords: django auth account social openid twitter facebook oauth registration theme tailwindcss
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_allauth_theme-0.7.1/django_allauth_theme.egg-info/SOURCES.txt` & `django_allauth_theme-0.7.2/django_allauth_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_allauth_theme-0.7.1/setup.py` & `django_allauth_theme-0.7.2/setup.py`

 * *Files identical despite different names*

