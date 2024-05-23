# Comparing `tmp/Flask-Mail-0.9.0.tar.gz` & `tmp/Flask-Mail-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Mail-0.9.0.tar", last modified: Fri Jun 14 17:00:55 2013, max compression
+gzip compressed data, was "dist/Flask-Mail-0.9.1.tar", last modified: Sun Sep 28 23:35:18 2014, max compression
```

## Comparing `Flask-Mail-0.9.0.tar` & `Flask-Mail-0.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/docs/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/docs/_static/
--rw-r--r--   0 matt       (501) staff       (20)     5851 2012-11-20 17:13:53.000000 Flask-Mail-0.9.0/docs/_static/flask-mail.jpg
--rw-r--r--   0 matt       (501) staff       (20)    15659 2012-11-20 17:13:53.000000 Flask-Mail-0.9.0/docs/_static/flask-mail.png
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/docs/_themes/
--rw-r--r--   0 matt       (501) staff       (20)       40 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/.git
--rw-r--r--   0 matt       (501) staff       (20)       22 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/.gitignore
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/docs/_themes/flask/
--rw-r--r--   0 matt       (501) staff       (20)      750 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask/layout.html
--rw-r--r--   0 matt       (501) staff       (20)      590 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask/relations.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/docs/_themes/flask/static/
--rw-r--r--   0 matt       (501) staff       (20)     6436 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 matt       (501) staff       (20)      976 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask/static/small_flask.css
--rw-r--r--   0 matt       (501) staff       (20)      164 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/docs/_themes/flask_small/
--rw-r--r--   0 matt       (501) staff       (20)      683 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/docs/_themes/flask_small/static/
--rw-r--r--   0 matt       (501) staff       (20)     4609 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask_small/static/flasky.css_t
--rw-r--r--   0 matt       (501) staff       (20)      184 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask_small/theme.conf
--rw-r--r--   0 matt       (501) staff       (20)     4875 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/flask_theme_support.py
--rw-r--r--   0 matt       (501) staff       (20)     1789 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     1093 2012-11-20 17:14:28.000000 Flask-Mail-0.9.0/docs/_themes/README
--rw-r--r--   0 matt       (501) staff       (20)       23 2012-11-20 17:13:53.000000 Flask-Mail-0.9.0/docs/changelog.rst
--rw-r--r--   0 matt       (501) staff       (20)     6521 2013-06-14 17:00:50.000000 Flask-Mail-0.9.0/docs/conf.py
--rw-r--r--   0 matt       (501) staff       (20)     6928 2013-04-03 20:10:22.000000 Flask-Mail-0.9.0/docs/index.rst
--rw-r--r--   0 matt       (501) staff       (20)     3079 2012-11-20 17:13:53.000000 Flask-Mail-0.9.0/docs/make.bat
--rw-r--r--   0 matt       (501) staff       (20)     3134 2012-11-20 17:13:53.000000 Flask-Mail-0.9.0/docs/Makefile
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/Flask_Mail.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)        1 2013-06-14 17:00:54.000000 Flask-Mail-0.9.0/Flask_Mail.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2012-11-20 17:15:41.000000 Flask-Mail-0.9.0/Flask_Mail.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)      943 2013-06-14 17:00:54.000000 Flask-Mail-0.9.0/Flask_Mail.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)       13 2013-06-14 17:00:54.000000 Flask-Mail-0.9.0/Flask_Mail.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)      818 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/Flask_Mail.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)       11 2013-06-14 17:00:54.000000 Flask-Mail-0.9.0/Flask_Mail.egg-info/top_level.txt
--rw-r--r--   0 matt       (501) staff       (20)    14667 2013-06-14 17:00:50.000000 Flask-Mail-0.9.0/flask_mail.py
--rw-r--r--   0 matt       (501) staff       (20)     1449 2012-11-20 17:13:53.000000 Flask-Mail-0.9.0/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)      150 2012-11-20 17:13:53.000000 Flask-Mail-0.9.0/MANIFEST.in
--rw-r--r--   0 matt       (501) staff       (20)      943 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      235 2013-04-03 18:43:29.000000 Flask-Mail-0.9.0/README.rst
--rw-r--r--   0 matt       (501) staff       (20)      165 2013-06-14 17:00:55.000000 Flask-Mail-0.9.0/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)     1248 2013-06-14 17:00:50.000000 Flask-Mail-0.9.0/setup.py
--rw-r--r--   0 matt       (501) staff       (20)    17580 2013-06-14 16:58:29.000000 Flask-Mail-0.9.0/tests.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/docs/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/docs/_static/
+-rw-r--r--   0 matt       (501) staff       (20)     5851 2012-11-20 17:13:53.000000 Flask-Mail-0.9.1/docs/_static/flask-mail.jpg
+-rw-r--r--   0 matt       (501) staff       (20)    15659 2012-11-20 17:13:53.000000 Flask-Mail-0.9.1/docs/_static/flask-mail.png
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/docs/_themes/
+-rw-r--r--   0 matt       (501) staff       (20)       40 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/.git
+-rw-r--r--   0 matt       (501) staff       (20)       22 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/.gitignore
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/docs/_themes/flask/
+-rw-r--r--   0 matt       (501) staff       (20)      750 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask/layout.html
+-rw-r--r--   0 matt       (501) staff       (20)      590 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask/relations.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/docs/_themes/flask/static/
+-rw-r--r--   0 matt       (501) staff       (20)     6436 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 matt       (501) staff       (20)      976 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask/static/small_flask.css
+-rw-r--r--   0 matt       (501) staff       (20)      164 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/docs/_themes/flask_small/
+-rw-r--r--   0 matt       (501) staff       (20)      683 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask_small/layout.html
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/docs/_themes/flask_small/static/
+-rw-r--r--   0 matt       (501) staff       (20)     4609 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask_small/static/flasky.css_t
+-rw-r--r--   0 matt       (501) staff       (20)      184 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask_small/theme.conf
+-rw-r--r--   0 matt       (501) staff       (20)     4875 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 matt       (501) staff       (20)     1789 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     1093 2012-11-20 17:14:28.000000 Flask-Mail-0.9.1/docs/_themes/README
+-rw-r--r--   0 matt       (501) staff       (20)       23 2012-11-20 17:13:53.000000 Flask-Mail-0.9.1/docs/changelog.rst
+-rw-r--r--   0 matt       (501) staff       (20)     6521 2014-09-28 23:35:16.000000 Flask-Mail-0.9.1/docs/conf.py
+-rw-r--r--   0 matt       (501) staff       (20)     7536 2014-09-28 23:27:04.000000 Flask-Mail-0.9.1/docs/index.rst
+-rw-r--r--   0 matt       (501) staff       (20)     3079 2012-11-20 17:13:53.000000 Flask-Mail-0.9.1/docs/make.bat
+-rw-r--r--   0 matt       (501) staff       (20)     3134 2012-11-20 17:13:53.000000 Flask-Mail-0.9.1/docs/Makefile
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/Flask_Mail.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)        1 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/Flask_Mail.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2012-11-20 17:15:41.000000 Flask-Mail-0.9.1/Flask_Mail.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (501) staff       (20)      943 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/Flask_Mail.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)       13 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/Flask_Mail.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)      818 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/Flask_Mail.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)       11 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/Flask_Mail.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)    17950 2014-09-28 23:35:16.000000 Flask-Mail-0.9.1/flask_mail.py
+-rw-r--r--   0 matt       (501) staff       (20)     1449 2012-11-20 17:13:53.000000 Flask-Mail-0.9.1/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)      150 2012-11-20 17:13:53.000000 Flask-Mail-0.9.1/MANIFEST.in
+-rw-r--r--   0 matt       (501) staff       (20)      943 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      235 2013-04-03 18:43:29.000000 Flask-Mail-0.9.1/README.rst
+-rw-r--r--   0 matt       (501) staff       (20)      165 2014-09-28 23:35:18.000000 Flask-Mail-0.9.1/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)     1286 2014-09-28 23:35:16.000000 Flask-Mail-0.9.1/setup.py
+-rw-r--r--   0 matt       (501) staff       (20)    27955 2014-09-28 23:27:04.000000 Flask-Mail-0.9.1/tests.py
```

### Comparing `Flask-Mail-0.9.0/docs/_static/flask-mail.jpg` & `Flask-Mail-0.9.1/docs/_static/flask-mail.jpg`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_static/flask-mail.png` & `Flask-Mail-0.9.1/docs/_static/flask-mail.png`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/flask/layout.html` & `Flask-Mail-0.9.1/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/flask/relations.html` & `Flask-Mail-0.9.1/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/flask/static/flasky.css_t` & `Flask-Mail-0.9.1/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/flask/static/small_flask.css` & `Flask-Mail-0.9.1/docs/_themes/flask/static/small_flask.css`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/flask_small/layout.html` & `Flask-Mail-0.9.1/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/flask_small/static/flasky.css_t` & `Flask-Mail-0.9.1/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/flask_theme_support.py` & `Flask-Mail-0.9.1/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/LICENSE` & `Flask-Mail-0.9.1/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/_themes/README` & `Flask-Mail-0.9.1/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/conf.py` & `Flask-Mail-0.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 copyright = u'2010, Dan Jacob'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.9.0'
+version = '0.9.1'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `Flask-Mail-0.9.0/docs/index.rst` & `Flask-Mail-0.9.1/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 
 * **MAIL_DEFAULT_SENDER** : default **None**
 
 * **MAIL_MAX_EMAILS** : default **None**
 
 * **MAIL_SUPPRESS_SEND** : default **app.testing**
 
+* **MAIL_ASCII_ATTACHMENTS** : default **False**
+
 In addition the standard Flask ``TESTING`` configuration option is used by **Flask-Mail**
 in unit tests (see below).
 
 Emails are managed through a ``Mail`` instance::
 
     from flask import Flask
     from flask_mail import Mail
@@ -159,14 +161,23 @@
 Adding attachments is straightforward::
 
     with app.open_resource("image.png") as fp:
         msg.attach("image.png", "image/png", fp.read())
 
 See the `API`_ for details.
 
+If ``MAIL_ASCII_ATTACHMENTS`` is set to **True**, filenames will be converted to
+an ASCII equivalent. This can be useful when using a mail relay that modify mail
+content and mess up Content-Disposition specification when filenames are UTF-8
+encoded. The conversion to ASCII is a basic removal of non-ASCII characters. It
+should be fine for any unicode character that can be decomposed by NFKD into one
+or more ASCII characters. If you need romanization/transliteration (i.e `ß` →
+`ss`) then your application should do it and pass a proper ASCII string.
+
+
 Unit tests and suppressing emails
 ---------------------------------
 
 When you are sending messages inside of unit tests, or in a development
 environment, it's useful to be able to suppress email sending.
 
 If the setting ``TESTING`` is set to ``True``, emails will be
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Flask-Mail-0.9.0/docs/make.bat` & `Flask-Mail-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/docs/Makefile` & `Flask-Mail-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/Flask_Mail.egg-info/PKG-INFO` & `Flask-Mail-0.9.1/Flask_Mail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.1
 Name: Flask-Mail
-Version: 0.9.0
+Version: 0.9.1
 Summary: Flask extension for sending email
 Home-page: https://github.com/rduplain/flask-mail
 Author: Ron DuPlain
 Author-email: ron.duplain@gmail.com
 License: BSD
 Description: 
         Flask-Mail
```

### Comparing `Flask-Mail-0.9.0/Flask_Mail.egg-info/SOURCES.txt` & `Flask-Mail-0.9.1/Flask_Mail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/flask_mail.py` & `Flask-Mail-0.9.1/flask_mail.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,40 +7,47 @@
 
     :copyright: (c) 2010 by Dan Jacob.
     :license: BSD, see LICENSE for more details.
 """
 
 from __future__ import with_statement
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
+import re
 import blinker
 import smtplib
 import sys
 import time
+import unicodedata
 
 from email import charset
 from email.encoders import encode_base64
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.header import Header
 from email.utils import formatdate, formataddr, make_msgid, parseaddr
 from contextlib import contextmanager
 
 from flask import current_app
 
 PY3 = sys.version_info[0] == 3
 
+PY34 = PY3 and sys.version_info[1] >= 4
+
 if PY3:
     string_types = str,
     text_type = str
+    from email import policy
+    message_policy = policy.SMTP
 else:
     string_types = basestring,
     text_type = unicode
+    message_policy = None
 
 charset.add_charset('utf-8', charset.SHORTEST, None, 'utf-8')
 
 
 class FlaskMailUnicodeDecodeError(UnicodeDecodeError):
     def __init__(self, obj, *args):
         self.obj = obj
@@ -59,34 +66,42 @@
     If strings_only is True, don't convert (some) non-string-like objects.
     """
     if isinstance(s, text_type):
         return s
 
     try:
         if not isinstance(s, string_types):
-            if hasattr(s, '__unicode__'):
+            if PY3:
+                if isinstance(s, bytes):
+                    s = text_type(s, encoding, errors)
+                else:
+                    s = text_type(s)
+            elif hasattr(s, '__unicode__'):
                 s = s.__unicode__()
             else:
-                if PY3:
-                    if isinstance(s, bytes):
-                        s = text_type(s, encoding, errors)
-                    else:
-                        s = text_type(s)
-                else:
-                    s = text_type(bytes(s), encoding, errors)
+                s = text_type(bytes(s), encoding, errors)
         else:
             s = s.decode(encoding, errors)
     except UnicodeDecodeError as e:
         if not isinstance(s, Exception):
             raise FlaskMailUnicodeDecodeError(s, *e.args)
         else:
             s = ' '.join([force_text(arg, encoding, strings_only,
                     errors) for arg in s])
     return s
 
+def sanitize_subject(subject, encoding='utf-8'):
+    try:
+        subject.encode('ascii')
+    except UnicodeEncodeError:
+        try:
+            subject = Header(subject, encoding).encode()
+        except UnicodeEncodeError:
+            subject = Header(subject, 'utf-8').encode()
+    return subject
 
 def sanitize_address(addr, encoding='utf-8'):
     if isinstance(addr, string_types):
         addr = parseaddr(force_text(addr))
     nm, addr = addr
 
     try:
@@ -102,17 +117,23 @@
             domain = domain.encode('idna').decode('ascii')
             addr = '@'.join([localpart, domain])
         else:
             addr = Header(addr, encoding).encode()
     return formataddr((nm, addr))
 
 
-def sanitize_addresses(addresses):
-    return map(lambda e: sanitize_address(e), addresses)
+def sanitize_addresses(addresses, encoding='utf-8'):
+    return map(lambda e: sanitize_address(e, encoding), addresses)
+
 
+def _has_newline(line):
+    """Used by has_bad_header to check for \\r or \\n"""
+    if line and ('\r' in line or '\n' in line):
+        return True
+    return False
 
 class Connection(object):
     """Handles connection to host."""
 
     def __init__(self, mail):
         self.mail = mail
 
@@ -141,35 +162,38 @@
         if self.mail.use_tls:
             host.starttls()
         if self.mail.username and self.mail.password:
             host.login(self.mail.username, self.mail.password)
 
         return host
 
-    def send(self, message):
+    def send(self, message, envelope_from=None):
         """Verifies and sends message.
 
         :param message: Message instance.
+        :param envelope_from: Email address to be used in MAIL FROM command.
         """
-        assert message.recipients, "No recipients have been added"
+        assert message.send_to, "No recipients have been added"
 
         assert message.sender, (
                 "The message does not specify a sender and a default sender "
                 "has not been configured")
 
         if message.has_bad_headers():
             raise BadHeaderError
 
         if message.date is None:
             message.date = time.time()
 
         if self.host:
-            self.host.sendmail(message.sender,
-                               message.send_to,
-                               message.as_string())
+            self.host.sendmail(sanitize_address(envelope_from or message.sender),
+                               list(sanitize_addresses(message.send_to)),
+                               message.as_bytes() if PY3 else message.as_string(),
+                               message.mail_options,
+                               message.rcpt_options)
 
         email_dispatched.send(message, app=current_app._get_current_object())
 
         self.num_emails += 1
 
         if self.num_emails == self.mail.max_emails:
             self.num_emails = 0
@@ -223,61 +247,69 @@
     :param cc: CC list
     :param bcc: BCC list
     :param attachments: list of Attachment instances
     :param reply_to: reply-to address
     :param date: send date
     :param charset: message character set
     :param extra_headers: A dictionary of additional headers for the message
+    :param mail_options: A list of ESMTP options to be used in MAIL FROM command
+    :param rcpt_options:  A list of ESMTP options to be used in RCPT commands
     """
 
-    def __init__(self, subject=None,
+    def __init__(self, subject='',
                  recipients=None,
                  body=None,
                  html=None,
                  sender=None,
                  cc=None,
                  bcc=None,
                  attachments=None,
                  reply_to=None,
                  date=None,
                  charset=None,
-                 extra_headers=None):
+                 extra_headers=None,
+                 mail_options=None,
+                 rcpt_options=None):
 
-        sender = sender
+        sender = sender or current_app.extensions['mail'].default_sender
 
         if isinstance(sender, tuple):
             sender = "%s <%s>" % sender
 
         self.recipients = recipients or []
         self.subject = subject
-        self.sender = sender or current_app.extensions['mail'].default_sender
+        self.sender = sender
         self.reply_to = reply_to
         self.cc = cc or []
         self.bcc = bcc or []
         self.body = body
         self.html = html
         self.date = date
         self.msgId = make_msgid()
         self.charset = charset
         self.extra_headers = extra_headers
+        self.mail_options = mail_options or []
+        self.rcpt_options = rcpt_options or []
         self.attachments = attachments or []
 
     @property
     def send_to(self):
         return set(self.recipients) | set(self.bcc or ()) | set(self.cc or ())
 
     def _mimetext(self, text, subtype='plain'):
         """Creates a MIMEText object with the given subtype (default: 'plain')
         If the text is unicode, the utf-8 charset is used.
         """
         charset = self.charset or 'utf-8'
         return MIMEText(text, _subtype=subtype, _charset=charset)
 
-    def as_string(self):
+    def _message(self):
         """Creates the email"""
+        ascii_attachments = current_app.extensions['mail'].ascii_attachments
+        encoding = self.charset or 'utf-8'
 
         attachments = self.attachments or []
 
         if len(attachments) == 0 and not self.html:
             # No html content and zero attachments means plain text
             msg = self._mimetext(self.body)
         elif len(attachments) > 0 and not self.html:
@@ -288,59 +320,103 @@
             # Anything else
             msg = MIMEMultipart()
             alternative = MIMEMultipart('alternative')
             alternative.attach(self._mimetext(self.body, 'plain'))
             alternative.attach(self._mimetext(self.html, 'html'))
             msg.attach(alternative)
 
-        msg['Subject'] = self.subject
-        msg['From'] = sanitize_address(self.sender)
-        msg['To'] = ', '.join(list(set(sanitize_addresses(self.recipients))))
+        if self.subject:
+            msg['Subject'] = sanitize_subject(force_text(self.subject), encoding)
+
+        msg['From'] = sanitize_address(self.sender, encoding)
+        msg['To'] = ', '.join(list(set(sanitize_addresses(self.recipients, encoding))))
 
         msg['Date'] = formatdate(self.date, localtime=True)
         # see RFC 5322 section 3.6.4.
         msg['Message-ID'] = self.msgId
 
         if self.cc:
-            msg['Cc'] = ', '.join(list(set(sanitize_addresses(self.cc))))
+            msg['Cc'] = ', '.join(list(set(sanitize_addresses(self.cc, encoding))))
 
         if self.reply_to:
-            msg['Reply-To'] = sanitize_address(self.reply_to)
+            msg['Reply-To'] = sanitize_address(self.reply_to, encoding)
 
         if self.extra_headers:
             for k, v in self.extra_headers.items():
                 msg[k] = v
 
+        SPACES = re.compile(r'[\s]+', re.UNICODE)
         for attachment in attachments:
             f = MIMEBase(*attachment.content_type.split('/'))
             f.set_payload(attachment.data)
             encode_base64(f)
 
-            f.add_header('Content-Disposition', '%s;filename=%s' %
-                         (attachment.disposition, attachment.filename))
+            filename = attachment.filename
+            if filename and ascii_attachments:
+                # force filename to ascii
+                filename = unicodedata.normalize('NFKD', filename)
+                filename = filename.encode('ascii', 'ignore').decode('ascii')
+                filename = SPACES.sub(u' ', filename).strip()
+
+            try:
+                filename and filename.encode('ascii')
+            except UnicodeEncodeError:
+                if not PY3:
+                    filename = filename.encode('utf8')
+                filename = ('UTF8', '', filename)
+
+            f.add_header('Content-Disposition',
+                         attachment.disposition,
+                         filename=filename)
 
             for key, value in attachment.headers:
                 f.add_header(key, value)
 
             msg.attach(f)
+        if message_policy:
+            msg.policy = message_policy
+
+        return msg
+
+    def as_string(self):
+        return self._message().as_string()
 
-        return msg.as_string()
+    def as_bytes(self):
+        if PY34:
+            return self._message().as_bytes()
+        else: # fallback for old Python (3) versions
+            return self._message().as_string().encode(self.charset or 'utf-8')
 
     def __str__(self):
         return self.as_string()
 
+    def __bytes__(self):
+        return self.as_bytes()
+
     def has_bad_headers(self):
         """Checks for bad headers i.e. newlines in subject, sender or recipients.
+        RFC5322: Allows multiline CRLF with trailing whitespace (FWS) in headers
         """
 
-        reply_to = self.reply_to or ''
-        for val in [self.subject, self.sender, reply_to] + self.recipients:
-            for c in '\r\n':
-                if c in val:
-                    return True
+        headers = [self.sender, self.reply_to] + self.recipients
+        for header in headers:
+            if _has_newline(header):
+                return True
+
+        if self.subject:
+            if _has_newline(self.subject):
+                for linenum, line in enumerate(self.subject.split('\r\n')):
+                    if not line:
+                        return True
+                    if linenum > 0 and line[0] not in '\t ':
+                        return True
+                    if _has_newline(line):
+                        return True
+                    if len(line.strip()) == 0:
+                        return True
         return False
 
     def is_bad_headers(self):
         from warnings import warn
         msg = 'is_bad_headers is deprecated, use the new has_bad_headers method instead.'
         warn(DeprecationWarning(msg), stacklevel=1)
         return self.has_bad_headers()
@@ -432,58 +508,66 @@
             return Connection(app.extensions['mail'])
         except KeyError:
             raise RuntimeError("The curent application was not configured with Flask-Mail")
 
 
 class _Mail(_MailMixin):
     def __init__(self, server, username, password, port, use_tls, use_ssl,
-                 default_sender, debug, max_emails, suppress):
+                 default_sender, debug, max_emails, suppress,
+                 ascii_attachments=False):
         self.server = server
         self.username = username
         self.password = password
         self.port = port
         self.use_tls = use_tls
         self.use_ssl = use_ssl
         self.default_sender = default_sender
         self.debug = debug
         self.max_emails = max_emails
         self.suppress = suppress
+        self.ascii_attachments = ascii_attachments
 
 
 class Mail(_MailMixin):
     """Manages email messaging
 
     :param app: Flask instance
     """
 
     def __init__(self, app=None):
         self.app = app
         if app is not None:
             self.state = self.init_app(app)
+        else:
+            self.state = None
+
+    def init_mail(self, config, debug=False, testing=False):
+        return _Mail(
+            config.get('MAIL_SERVER', '127.0.0.1'),
+            config.get('MAIL_USERNAME'),
+            config.get('MAIL_PASSWORD'),
+            config.get('MAIL_PORT', 25),
+            config.get('MAIL_USE_TLS', False),
+            config.get('MAIL_USE_SSL', False),
+            config.get('MAIL_DEFAULT_SENDER'),
+            int(config.get('MAIL_DEBUG', debug)),
+            config.get('MAIL_MAX_EMAILS'),
+            config.get('MAIL_SUPPRESS_SEND', testing),
+            config.get('MAIL_ASCII_ATTACHMENTS', False)
+        )
 
     def init_app(self, app):
         """Initializes your mail settings from the application settings.
 
         You can use this if you want to set up your Mail instance
         at configuration time.
 
         :param app: Flask application instance
         """
-
-        state = _Mail(
-            app.config.get('MAIL_SERVER', '127.0.0.1'),
-            app.config.get('MAIL_USERNAME'),
-            app.config.get('MAIL_PASSWORD'),
-            app.config.get('MAIL_PORT', 25),
-            app.config.get('MAIL_USE_TLS', False),
-            app.config.get('MAIL_USE_SSL', False),
-            app.config.get('MAIL_DEFAULT_SENDER'),
-            int(app.config.get('MAIL_DEBUG', app.debug)),
-            app.config.get('MAIL_MAX_EMAILS'),
-            app.config.get('MAIL_SUPPRESS_SEND', app.testing))
+        state = self.init_mail(app.config, app.debug, app.testing)
 
         # register extension with app
         app.extensions = getattr(app, 'extensions', {})
         app.extensions['mail'] = state
         return state
 
     def __getattr__(self, name):
```

### Comparing `Flask-Mail-0.9.0/LICENSE` & `Flask-Mail-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Mail-0.9.0/PKG-INFO` & `Flask-Mail-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.1
 Name: Flask-Mail
-Version: 0.9.0
+Version: 0.9.1
 Summary: Flask extension for sending email
 Home-page: https://github.com/rduplain/flask-mail
 Author: Ron DuPlain
 Author-email: ron.duplain@gmail.com
 License: BSD
 Description: 
         Flask-Mail
```

### Comparing `Flask-Mail-0.9.0/setup.py` & `Flask-Mail-0.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * `documentation <http://packages.python.org/Flask-Mail>`_
 """
 from setuptools import setup
 
 
 setup(
     name='Flask-Mail',
-    version='0.9.0',
+    version='0.9.1',
     url='https://github.com/rduplain/flask-mail',
     license='BSD',
     author='Dan Jacob',
     author_email='danjac354@gmail.com',
     maintainer='Ron DuPlain',
     maintainer_email='ron.duplain@gmail.com',
     description='Flask extension for sending email',
@@ -34,14 +34,16 @@
     install_requires=[
         'Flask',
         'blinker',
     ],
     tests_require=[
         'nose',
         'blinker',
+        'speaklater',
+        'mock',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
```

### Comparing `Flask-Mail-0.9.0/tests.py` & `Flask-Mail-0.9.1/tests.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 from __future__ import with_statement
 
 import base64
 import email
 import unittest
 import time
 import re
+import mock
+from contextlib import contextmanager
 
 from email.header import Header
+from email import charset
 
 from flask import Flask
-from flask_mail import Mail, Message, BadHeaderError, sanitize_address
+from flask_mail import Mail, Message, BadHeaderError, sanitize_address, PY3
+from speaklater import make_lazy_string
 
 
 class TestCase(unittest.TestCase):
 
     TESTING = True
     MAIL_DEFAULT_SENDER = "support@mysite.com"
 
@@ -26,14 +30,32 @@
         self.mail = Mail(self.app)
         self.ctx = self.app.test_request_context()
         self.ctx.push()
 
     def tearDown(self):
         self.ctx.pop()
 
+    @contextmanager
+    def mail_config(self, **settings):
+        """
+        Context manager to alter mail config during a test and restore it after,
+        even in case of a failure.
+        """
+        original = {}
+        state = self.mail.state
+        for key in settings:
+            assert hasattr(state, key)
+            original[key] = getattr(state, key)
+            setattr(state, key, settings[key])
+
+        yield
+        # restore
+        for k, v in original.items():
+            setattr(state, k, v)
+
     def assertIn(self, member, container, msg=None):
         if hasattr(unittest.TestCase, 'assertIn'):
             return unittest.TestCase.assertIn(self, member, container, msg)
         return self.assertTrue(member in container)
 
     def assertNotIn(self, member, container, msg=None):
         if hasattr(unittest.TestCase, 'assertNotIn'):
@@ -47,14 +69,26 @@
 
     def assertIsNotNone(self, obj, msg=None):
         if hasattr(unittest.TestCase, 'assertIsNotNone'):
             return unittest.TestCase.assertIsNotNone(self, obj, msg)
         return self.assertTrue(obj is not None)
 
 
+class TestInitialization(TestCase):
+
+    def test_init_mail(self):
+        mail = self.mail.init_mail(
+            self.app.config,
+            self.app.debug,
+            self.app.testing
+        )
+
+        self.assertEquals(self.mail.state.__dict__, mail.__dict__)
+
+
 class TestMessage(TestCase):
 
     def test_initialize(self):
         msg = Message(subject="subject",
                       recipients=["to@example.com"])
         self.assertEqual(msg.sender, self.app.extensions['mail'].default_sender)
         self.assertEqual(msg.recipients, ["to@example.com"])
@@ -62,14 +96,25 @@
     def test_recipients_properly_initialized(self):
         msg = Message(subject="subject")
         self.assertEqual(msg.recipients, [])
         msg2 = Message(subject="subject")
         msg2.add_recipient("somebody@here.com")
         self.assertEqual(len(msg2.recipients), 1)
 
+    def test_esmtp_options_properly_initialized(self):
+        msg = Message(subject="subject")
+        self.assertEqual(msg.mail_options, [])
+        self.assertEqual(msg.rcpt_options, [])
+
+        msg = Message(subject="subject", mail_options=['BODY=8BITMIME'])
+        self.assertEqual(msg.mail_options, ['BODY=8BITMIME'])
+
+        msg2 = Message(subject="subject", rcpt_options=['NOTIFY=SUCCESS'])
+        self.assertEqual(msg2.rcpt_options, ['NOTIFY=SUCCESS'])
+
     def test_sendto_properly_set(self):
         msg = Message(subject="subject", recipients=["somebody@here.com"],
                       cc=["cc@example.com"], bcc=["bcc@example.com"])
         self.assertEqual(len(msg.send_to), 3)
         msg.add_recipient("cc@example.com")
         self.assertEqual(len(msg.send_to), 3)
 
@@ -79,14 +124,19 @@
         self.assertEqual(msg.recipients, ["to@example.com"])
 
     def test_sender_as_tuple(self):
         msg = Message(subject="testing",
                       sender=("tester", "tester@example.com"))
         self.assertEqual('tester <tester@example.com>', msg.sender)
 
+    def test_default_sender_as_tuple(self):
+        self.app.extensions['mail'].default_sender = ('tester', 'tester@example.com')
+        msg = Message(subject="testing")
+        self.assertEqual('tester <tester@example.com>', msg.sender)
+
     def test_reply_to(self):
         msg = Message(subject="testing",
                       recipients=["to@example.com"],
                       sender="spammer <spammer@example.com>",
                       reply_to="somebody <somebody@example.com>",
                       body="testing")
         response = msg.as_string()
@@ -132,32 +182,61 @@
         a = msg.attachments[0]
         self.assertIsNone(a.filename)
         self.assertEqual(a.disposition, 'attachment')
         self.assertEqual(a.content_type, "text/plain")
         self.assertEqual(a.data, b"this is a test")
 
     def test_bad_header_subject(self):
-        msg = Message(subject="testing\n\r",
+        msg = Message(subject="testing\r\n",
+                      sender="from@example.com",
+                      body="testing",
+                      recipients=["to@example.com"])
+        self.assertRaises(BadHeaderError, self.mail.send, msg)
+
+    def test_multiline_subject(self):
+        msg = Message(subject="testing\r\n testing\r\n testing \r\n \ttesting",
+                      sender="from@example.com",
+                      body="testing",
+                      recipients=["to@example.com"])
+        self.mail.send(msg)
+        response = msg.as_string()
+        self.assertIn("From: from@example.com", str(response))
+        self.assertIn("testing\r\n testing\r\n testing \r\n \ttesting", str(response))
+
+    def test_bad_multiline_subject(self):
+        msg = Message(subject="testing\r\n testing\r\n ",
+                      sender="from@example.com",
+                      body="testing",
+                      recipients=["to@example.com"])
+        self.assertRaises(BadHeaderError, self.mail.send, msg)
+
+        msg = Message(subject="testing\r\n testing\r\n\t",
+                      sender="from@example.com",
+                      body="testing",
+                      recipients=["to@example.com"])
+        self.assertRaises(BadHeaderError, self.mail.send, msg)
+
+        msg = Message(subject="testing\r\n testing\r\n\n",
                       sender="from@example.com",
                       body="testing",
                       recipients=["to@example.com"])
         self.assertRaises(BadHeaderError, self.mail.send, msg)
 
     def test_bad_header_sender(self):
         msg = Message(subject="testing",
-                      sender="from@example.com\n\r",
+                      sender="from@example.com\r\n",
                       recipients=["to@example.com"],
                       body="testing")
 
         self.assertIn('From: from@example.com', msg.as_string())
 
     def test_bad_header_reply_to(self):
         msg = Message(subject="testing",
                       sender="from@example.com",
-                      reply_to="evil@example.com\n\r",
+                      reply_to="evil@example.com\r",
                       recipients=["to@example.com"],
                       body="testing")
 
         self.assertIn('From: from@example.com', msg.as_string())
         self.assertIn('To: to@example.com', msg.as_string())
         self.assertIn('Reply-To: evil@example.com', msg.as_string())
 
@@ -165,15 +244,15 @@
         msg = Message(subject="testing",
                       sender="from@example.com",
                       recipients=[
                           "to@example.com",
                           "to\r\n@example.com"],
                       body="testing")
 
-        self.assertIn('To: to@example.com\n', msg.as_string())
+        self.assertIn('To: to@example.com', msg.as_string())
 
     def test_emails_are_sanitized(self):
         msg = Message(subject="testing",
                       sender="sender\r\n@example.com",
                       reply_to="reply_to\r\n@example.com",
                       recipients=["recipient\r\n@example.com"])
         self.assertIn('sender@example.com', msg.as_string())
@@ -203,14 +282,56 @@
                       body="hello")
 
         msg.attach(data=b"this is a test",
                    content_type="text/plain")
 
         self.assertIn('Content-Type: multipart/mixed', msg.as_string())
 
+    def test_plain_message_with_ascii_attachment(self):
+        msg = Message(subject="subject",
+                      recipients=["to@example.com"],
+                      body="hello")
+
+        msg.attach(data=b"this is a test",
+                   content_type="text/plain",
+                   filename='test doc.txt')
+
+        self.assertIn('Content-Disposition: attachment; filename="test doc.txt"', msg.as_string())
+
+    def test_plain_message_with_unicode_attachment(self):
+        msg = Message(subject="subject",
+                      recipients=["to@example.com"],
+                      body="hello")
+
+        msg.attach(data=b"this is a test",
+                   content_type="text/plain",
+                   filename=u'ünicöde ←→ ✓.txt')
+
+        parsed = email.message_from_string(msg.as_string())
+
+        self.assertIn(re.sub(r'\s+', ' ', parsed.get_payload()[1].get('Content-Disposition')), [
+            'attachment; filename*="UTF8\'\'%C3%BCnic%C3%B6de%20%E2%86%90%E2%86%92%20%E2%9C%93.txt"',
+            'attachment; filename*=UTF8\'\'%C3%BCnic%C3%B6de%20%E2%86%90%E2%86%92%20%E2%9C%93.txt'
+            ])
+
+    def test_plain_message_with_ascii_converted_attachment(self):
+        with self.mail_config(ascii_attachments=True):
+            msg = Message(subject="subject",
+                          recipients=["to@example.com"],
+                          body="hello")
+
+            msg.attach(data=b"this is a test",
+                       content_type="text/plain",
+                       filename=u'ünicödeß ←.→ ✓.txt')
+
+            parsed = email.message_from_string(msg.as_string())
+            self.assertIn(
+                'Content-Disposition: attachment; filename="unicode . .txt"',
+                msg.as_string())
+
     def test_html_message(self):
         html_text = "<p>Hello World</p>"
         msg = Message(sender="from@example.com",
                       subject="subject",
                       recipients=["to@example.com"],
                       html=html_text)
 
@@ -299,14 +420,20 @@
             self.assertIn(h1_a.encode(), response)
         except AssertionError:
             self.assertIn(h1_b.encode(), response)
 
         self.assertIn(h2.encode(), response)
         self.assertIn(h3.encode(), response)
 
+    def test_unicode_subject(self):
+        msg = Message(subject=make_lazy_string(lambda a: a, u"sübject"),
+                      sender='from@example.com',
+                      recipients=["to@example.com"])
+        self.assertIn('=?utf-8?q?s=C3=BCbject?=', msg.as_string())
+
     def test_extra_headers(self):
         msg = Message(sender="from@example.com",
                       subject="subject",
                       recipients=["to@example.com"],
                       body="hello",
                       extra_headers={'X-Extra-Header': 'Yes'})
         self.assertIn('X-Extra-Header: Yes', msg.as_string())
@@ -349,14 +476,70 @@
         msg = Message(sender="from@example.com",
                       subject="subject",
                       recipients=["foo@bar.com"])
         msg.html = None
         msg.attach(data=b"foobar", content_type='text/csv')
         self.assertIn('Content-Type: text/plain; charset="utf-8"', msg.as_string())
 
+        # unicode sender as tuple
+        msg = Message(sender=(u"送信者", "from@example.com"),
+                      subject=u"表題",
+                      recipients=["foo@bar.com"],
+                      reply_to=u"返信先 <somebody@example.com>",
+                      charset='shift_jis')  # japanese
+        msg.body = u'内容'
+        self.assertIn('From: =?iso-2022-jp?', msg.as_string())
+        self.assertNotIn('From: =?utf-8?', msg.as_string())
+        self.assertIn('Subject: =?iso-2022-jp?', msg.as_string())
+        self.assertNotIn('Subject: =?utf-8?', msg.as_string())
+        self.assertIn('Reply-To: =?iso-2022-jp?', msg.as_string())
+        self.assertNotIn('Reply-To: =?utf-8?', msg.as_string())
+        self.assertIn('Content-Type: text/plain; charset="iso-2022-jp"', msg.as_string())
+
+        # unicode subject sjis
+        msg = Message(sender="from@example.com",
+                      subject=u"表題",
+                      recipients=["foo@bar.com"],
+                      charset='shift_jis')  # japanese
+        msg.body = u'内容'
+        self.assertIn('Subject: =?iso-2022-jp?', msg.as_string())
+        self.assertIn('Content-Type: text/plain; charset="iso-2022-jp"', msg.as_string())
+
+        # unicode subject utf-8
+        msg = Message(sender="from@example.com",
+                      subject="subject",
+                      recipients=["foo@bar.com"],
+                      charset='utf-8')
+        msg.body = u'内容'
+        self.assertIn('Subject: subject', msg.as_string())
+        self.assertIn('Content-Type: text/plain; charset="utf-8"', msg.as_string())
+
+        # ascii subject
+        msg = Message(sender="from@example.com",
+                      subject="subject",
+                      recipients=["foo@bar.com"],
+                      charset='us-ascii')
+        msg.body = "normal ascii text"
+        self.assertNotIn('Subject: =?us-ascii?', msg.as_string())
+        self.assertIn('Content-Type: text/plain; charset="us-ascii"', msg.as_string())
+
+        # default charset
+        msg = Message(sender="from@example.com",
+                      subject="subject",
+                      recipients=["foo@bar.com"])
+        msg.body = "normal ascii text"
+        self.assertNotIn('Subject: =?', msg.as_string())
+        self.assertIn('Content-Type: text/plain; charset="utf-8"', msg.as_string())
+
+    def test_empty_subject_header(self):
+        msg = Message(sender="from@example.com",
+                      recipients=["foo@bar.com"])
+        msg.body = "normal ascii text"
+        self.mail.send(msg)
+        self.assertNotIn('Subject:', msg.as_string())
 
 class TestMail(TestCase):
 
     def test_send(self):
 
         with self.mail.record_messages() as outbox:
             msg = Message(subject="testing",
@@ -435,7 +618,76 @@
 
     def test_bad_header_subject(self):
         msg = Message(subject="testing\n\r",
                       body="testing",
                       recipients=["to@example.com"])
         with self.mail.connect() as conn:
             self.assertRaises(BadHeaderError, conn.send, msg)
+
+    def test_sendmail_with_ascii_recipient(self):
+        with self.mail.connect() as conn:
+            with mock.patch.object(conn, 'host') as host:
+                msg = Message(subject="testing",
+                              sender="from@example.com",
+                              recipients=["to@example.com"],
+                              body="testing")
+                conn.send(msg)
+
+                host.sendmail.assert_called_once_with(
+                    "from@example.com",
+                    ["to@example.com"],
+                    msg.as_bytes() if PY3 else msg.as_string(),
+                    msg.mail_options,
+                    msg.rcpt_options
+                )
+
+    def test_sendmail_with_non_ascii_recipient(self):
+        with self.mail.connect() as conn:
+            with mock.patch.object(conn, 'host') as host:
+                msg = Message(subject="testing",
+                              sender="from@example.com",
+                              recipients=[u'ÄÜÖ → ✓ <to@example.com>'],
+                              body="testing")
+                conn.send(msg)
+
+                host.sendmail.assert_called_once_with(
+                    "from@example.com",
+                    ["=?utf-8?b?w4TDnMOWIOKGkiDinJM=?= <to@example.com>"],
+                    msg.as_bytes() if PY3 else msg.as_string(),
+                    msg.mail_options,
+                    msg.rcpt_options
+                )
+
+    def test_sendmail_with_ascii_body(self):
+        with self.mail.connect() as conn:
+            with mock.patch.object(conn, 'host') as host:
+                msg = Message(subject="testing",
+                              sender="from@example.com",
+                              recipients=["to@example.com"],
+                              body="body")
+                conn.send(msg)
+
+                host.sendmail.assert_called_once_with(
+                    "from@example.com",
+                    ["to@example.com"],
+                    msg.as_bytes() if PY3 else msg.as_string(),
+                    msg.mail_options,
+                    msg.rcpt_options
+                )
+
+    def test_sendmail_with_non_ascii_body(self):
+        with self.mail.connect() as conn:
+            with mock.patch.object(conn, 'host') as host:
+                msg = Message(subject="testing",
+                              sender="from@example.com",
+                              recipients=["to@example.com"],
+                              body=u"Öö")
+
+                conn.send(msg)
+
+                host.sendmail.assert_called_once_with(
+                    "from@example.com",
+                    ["to@example.com"],
+                    msg.as_bytes() if PY3 else msg.as_string(),
+                    msg.mail_options,
+                    msg.rcpt_options
+                )
```

