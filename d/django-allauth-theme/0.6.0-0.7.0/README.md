# Comparing `tmp/django-allauth-theme-0.6.0.tar.gz` & `tmp/django_allauth_theme-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-allauth-theme-0.6.0.tar", last modified: Thu Feb  2 15:35:38 2023, max compression
+gzip compressed data, was "django_allauth_theme-0.7.0.tar", last modified: Fri May 24 14:08:03 2024, max compression
```

## Comparing `django-allauth-theme-0.6.0.tar` & `django_allauth_theme-0.7.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.746825 django-allauth-theme-0.6.0/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1074 2023-01-27 09:22:54.000000 django-allauth-theme-0.6.0/LICENSE
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      197 2023-02-02 15:35:13.000000 django-allauth-theme-0.6.0/MANIFEST.in
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     3547 2023-02-02 15:35:38.746825 django-allauth-theme-0.6.0/PKG-INFO
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1994 2023-02-02 12:58:28.000000 django-allauth-theme-0.6.0/README.md
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.742811 django-allauth-theme-0.6.0/allauth_theme/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      143 2023-02-02 15:35:26.000000 django-allauth-theme-0.6.0/allauth_theme/__init__.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1019 2023-01-30 08:30:53.000000 django-allauth-theme-0.6.0/allauth_theme/app_settings.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      486 2023-01-30 08:30:53.000000 django-allauth-theme-0.6.0/allauth_theme/context_processors.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      492 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/forms.py
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.742811 django-allauth-theme-0.6.0/allauth_theme/static/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.742811 django-allauth-theme-0.6.0/allauth_theme/static/css/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)    12018 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/static/css/signup.css
--rw-rw-r--   0 ledil     (1000) ledil     (1000)    21356 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/static/css/tailwind.css
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.742811 django-allauth-theme-0.6.0/allauth_theme/static/img/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     4099 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/static/img/google.png
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.742811 django-allauth-theme-0.6.0/allauth_theme/templates/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.742811 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.746825 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/account_inactive.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2383 2023-01-30 08:30:53.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2609 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/email.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1035 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/email_confirm.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1958 2023-02-02 15:32:15.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/login.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      562 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/logout.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      623 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_change.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      867 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_reset.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      550 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_reset_done.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      875 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_reset_from_key.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_reset_from_key_done.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      485 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_set.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      793 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/signup.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      294 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/signup_closed.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      582 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/verification_sent.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1007 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/verified_email_required.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.746825 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/openid/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       48 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/openid/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      473 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/openid/login.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.746825 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      332 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/authentication_error.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       42 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/base.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1480 2023-02-02 15:26:57.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/connections.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      861 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/login.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      495 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/login_cancelled.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      835 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/signup.html
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.746825 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/snippets/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)      786 2023-01-27 09:23:11.000000 django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2150 2023-01-30 08:30:53.000000 django-allauth-theme-0.6.0/allauth_theme/urls.py
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2604 2023-01-30 08:30:53.000000 django-allauth-theme-0.6.0/allauth_theme/views.py
-drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2023-02-02 15:35:38.746825 django-allauth-theme-0.6.0/django_allauth_theme.egg-info/
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     3547 2023-02-02 15:35:38.000000 django-allauth-theme-0.6.0/django_allauth_theme.egg-info/PKG-INFO
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     2028 2023-02-02 15:35:38.000000 django-allauth-theme-0.6.0/django_allauth_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)        1 2023-02-02 15:35:38.000000 django-allauth-theme-0.6.0/django_allauth_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       63 2023-02-02 15:35:38.000000 django-allauth-theme-0.6.0/django_allauth_theme.egg-info/requires.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       14 2023-02-02 15:35:38.000000 django-allauth-theme-0.6.0/django_allauth_theme.egg-info/top_level.txt
--rw-rw-r--   0 ledil     (1000) ledil     (1000)       38 2023-02-02 15:35:38.746825 django-allauth-theme-0.6.0/setup.cfg
--rw-rw-r--   0 ledil     (1000) ledil     (1000)     1902 2023-02-02 12:54:07.000000 django-allauth-theme-0.6.0/setup.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1074 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/LICENSE
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      197 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/MANIFEST.in
+-rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/PKG-INFO
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1994 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/README.md
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.709406 django_allauth_theme-0.7.0/allauth_theme/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      142 2024-05-24 14:07:32.000000 django_allauth_theme-0.7.0/allauth_theme/__init__.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1234 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.0/allauth_theme/app_settings.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      624 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.0/allauth_theme/context_processors.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      492 2024-05-24 13:46:59.000000 django_allauth_theme-0.7.0/allauth_theme/forms.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.709406 django_allauth_theme-0.7.0/allauth_theme/static/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/static/css/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)    12018 2024-05-24 13:45:30.000000 django_allauth_theme-0.7.0/allauth_theme/static/css/signup.css
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)    21356 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.0/allauth_theme/static/css/tailwind.css
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/static/img/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     4099 2024-05-24 13:44:13.000000 django_allauth_theme-0.7.0/allauth_theme/static/img/google.png
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.709406 django_allauth_theme-0.7.0/allauth_theme/templates/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.709406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/account_inactive.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2453 2024-05-24 13:47:39.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2609 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/email.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1035 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/email_confirm.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1958 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/login.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      562 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/logout.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      623 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_change.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      867 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      550 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_done.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      875 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_from_key.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      273 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_from_key_done.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      485 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_set.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      793 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/signup.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      294 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/signup_closed.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      582 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/verification_sent.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1007 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/verified_email_required.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/openid/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       48 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/openid/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      473 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/openid/login.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      332 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/authentication_error.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       42 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/base.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1480 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/connections.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      861 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/login.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      495 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/login_cancelled.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      835 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/signup.html
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/snippets/
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)      786 2023-01-28 09:03:02.000000 django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2150 2024-05-24 13:46:02.000000 django_allauth_theme-0.7.0/allauth_theme/urls.py
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2604 2024-05-24 13:46:40.000000 django_allauth_theme-0.7.0/allauth_theme/views.py
+drwxrwxr-x   0 ledil     (1000) ledil     (1000)        0 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/
+-rw-r--r--   0 ledil     (1000) ledil     (1000)     3655 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/PKG-INFO
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     2028 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/SOURCES.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)        1 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/dependency_links.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       63 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/requires.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       14 2024-05-24 14:08:03.000000 django_allauth_theme-0.7.0/django_allauth_theme.egg-info/top_level.txt
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)       38 2024-05-24 14:08:03.713406 django_allauth_theme-0.7.0/setup.cfg
+-rw-rw-r--   0 ledil     (1000) ledil     (1000)     1902 2024-05-24 14:06:06.000000 django_allauth_theme-0.7.0/setup.py
```

### Comparing `django-allauth-theme-0.6.0/LICENSE` & `django_allauth_theme-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/PKG-INFO` & `django_allauth_theme-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-theme
-Version: 0.6.0
+Version: 0.7.0
 Summary: An awesome and responsive django-allauth theme based on tailwind
 Home-page: http://pypi.python.org/pypi/django-allauth-theme/
 Author: Leonardo Di Lella
 Author-email: leonardo.dilella@mobileapart.com
 License: LICENSE
 Keywords: django auth account social openid twitter facebook oauth registration theme tailwindcss
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,14 +30,17 @@
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=2.0
+Requires-Dist: django-allauth>=0.51.0
+Requires-Dist: django-crispy-forms>=1.14.0
 
 # django-allauth-theme
 
 An awesome and responsive django-allauth theme based on tailwind.
 
 ## Install
```

### Comparing `django-allauth-theme-0.6.0/README.md` & `django_allauth_theme-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/app_settings.py` & `django_allauth_theme-0.7.0/allauth_theme/app_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-# -*- coding: utf-8 -*-
 from django.conf import settings
 
 
-class AppSettings(object):
+class AppSettings:
     @property
     def DAT_WELCOME_TITLE(self):
         return getattr(settings, "DAT_WELCOME_TITLE", "Welcome")
 
     @property
+    def DAT_TAILWIND_CSS(self):
+        return getattr(settings, "DAT_TAILWIND_CSS", "css/tailwind.css")
+
+    @property
+    def DAT_SIGNUP_CSS(self):
+        return getattr(settings, "DAT_SIGNUP_CSS", "css/signup.css")
+
+    @property
     def DAT_WELCOME_TITLE_MOBILE(self):
         return getattr(settings, "DAT_WELCOME_TITLE_MOBILE", "Welcome mobile")
 
     @property
     def DAT_GOOGLE_ENABLE_ONETAP_LOGIN(self):
         return getattr(settings, "DAT_GOOGLE_ENABLE_ONETAP_LOGIN", False)
 
@@ -21,10 +28,13 @@
 
     @property
     def DAT_BASE_URL(self):
         return getattr(settings, "DAT_BASE_URL", "http://localhost:8000")
 
     @property
     def DAT_WELCOME_TEXT(self):
-        return getattr(settings, "DAT_WELCOME_TEXT",
-                       "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor"
-                       " invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua")
+        return getattr(
+            settings,
+            "DAT_WELCOME_TEXT",
+            "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor"
+            " invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua",
+        )
```

### Comparing `django-allauth-theme-0.6.0/allauth_theme/static/css/signup.css` & `django_allauth_theme-0.7.0/allauth_theme/static/css/signup.css`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/static/css/tailwind.css` & `django_allauth_theme-0.7.0/allauth_theme/static/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/static/img/google.png` & `django_allauth_theme-0.7.0/allauth_theme/static/img/google.png`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/base.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load static i18n %}
 <!DOCTYPE html>
 <html>
 <head>
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <title>{% block head_title %}{% endblock %}</title>
-    <link href="{% static "css/tailwind.css" %}" rel="stylesheet"/>
-    <link href="{% static "css/signup.css" %}" rel="stylesheet"/>
+    <link href="{{ DAT_TAILWIND_CSS }}" rel="stylesheet"/>
+    <link href="{{ DAT_SIGNUP_CSS }}" rel="stylesheet"/>
     {% block extra_head %}
     {% endblock %}
 </head>
 <body class="sign_in_up_modal">
 {% if DAT_GOOGLE_ENABLE_ONETAP_LOGIN %}
 <div id="g_id_onload"
      data-client_id="{{DAT_GOOGLE_CLIENT_ID}}"
@@ -19,22 +19,22 @@
 </div>
 <script src="https://accounts.google.com/gsi/client" async defer></script>
 {% endif %}
 {% block body %}
     <div class="flex lg:flex-row h-screen flex-col">
         <div class="lg:basis-1/2 basis-1 bg_svg lg:pt-0 pt-20">
             <div class="sign_up_welcome_box lg:ml-20p lg:mr-100 lg:justify-end justify-center">
-                <div>
-                    <h2 class="lg:block hidden title">{{ DAT_WELCOME_TITLE }}</h2>
-                    <h3 class="lg:hidden title">{{ DAT_WELCOME_TITLE_MOBILE }}</h3>
+                <div class="px-10">
+                    <h4 class="lg:block hidden text-2xl font-bold dark:text-white pb-2">{{ DAT_WELCOME_TITLE }}</h4>
+                    <h3 class="lg:hidden text-2xl font-bold dark:text-white pb-2">{{ DAT_WELCOME_TITLE_MOBILE }}</h3>
                     <p class="lg:block hidden">{{ DAT_WELCOME_TEXT }}</p>
                 </div>
             </div>
         </div>
-        <div class="basis-1/2 lg:mt-0 mt-12 lg:mb-0 mb-12">
+        <div class="basis-1/2 lg:mt-0 mt-12 lg:mb-0 mb-12 pl-10">
         {% if not request.user.is_authenticated %}
             <ul class="sign_up_menu">
                 <li><a class="link" href="{% url 'account_login' %}">{% trans "Sign In" %}</a></li>
                 <li><a class="primaryAction" href="{% url 'account_signup' %}">{% trans "Sign Up" %}</a></li>
             </ul>
         {% endif %}
             <div class="sign_up_form lg:justify-start justify-center lg:ml-100 ml-0">
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
 {% load static i18n %}
-}" rel="stylesheet"/>
-}" rel="stylesheet"/> {% block extra_head %} {% endblock %}
+{% block extra_head %} {% endblock %}
 {% if DAT_GOOGLE_ENABLE_ONETAP_LOGIN %}
 {% endif %} {% block body %}
-********** {{{{ DDAATT__WWEELLCCOOMMEE__TTIITTLLEE }}}} **********
+****** {{{{ DDAATT__WWEELLCCOOMMEE__TTIITTLLEE }}}} ******
 ******** {{{{ DDAATT__WWEELLCCOOMMEE__TTIITTLLEE__MMOOBBIILLEE }}}} ********
 {{ DAT_WELCOME_TEXT }}
 {% if not request.user.is_authenticated %}
     * _{_%_ _t_r_a_n_s_ _"_S_i_g_n_ _I_n_"_ _%_}
     * _{_%_ _t_r_a_n_s_ _"_S_i_g_n_ _U_p_"_ _%_}
 {% endif %}
 {% if messages %}
```

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/email.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/email.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/email_confirm.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/login.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/login.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/logout.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/logout.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_change.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_change.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_reset.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_reset_done.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/password_reset_from_key.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/signup.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/signup.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/verification_sent.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/account/verified_email_required.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/connections.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/login.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/signup.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html` & `django_allauth_theme-0.7.0/allauth_theme/templates/allauth/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/urls.py` & `django_allauth_theme-0.7.0/allauth_theme/urls.py`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/allauth_theme/views.py` & `django_allauth_theme-0.7.0/allauth_theme/views.py`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/django_allauth_theme.egg-info/PKG-INFO` & `django_allauth_theme-0.7.0/django_allauth_theme.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-theme
-Version: 0.6.0
+Version: 0.7.0
 Summary: An awesome and responsive django-allauth theme based on tailwind
 Home-page: http://pypi.python.org/pypi/django-allauth-theme/
 Author: Leonardo Di Lella
 Author-email: leonardo.dilella@mobileapart.com
 License: LICENSE
 Keywords: django auth account social openid twitter facebook oauth registration theme tailwindcss
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,14 +30,17 @@
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=2.0
+Requires-Dist: django-allauth>=0.51.0
+Requires-Dist: django-crispy-forms>=1.14.0
 
 # django-allauth-theme
 
 An awesome and responsive django-allauth theme based on tailwind.
 
 ## Install
```

### Comparing `django-allauth-theme-0.6.0/django_allauth_theme.egg-info/SOURCES.txt` & `django_allauth_theme-0.7.0/django_allauth_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-allauth-theme-0.6.0/setup.py` & `django_allauth_theme-0.7.0/setup.py`

 * *Files identical despite different names*

