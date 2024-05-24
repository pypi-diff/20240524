# Comparing `tmp/feincms3-4.6.0.tar.gz` & `tmp/feincms3-4.6.1.tar.gz`

## Comparing `feincms3-4.6.0.tar` & `feincms3-4.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/__init__.py
--rw-r--r--   0        0        0    18418 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/admin.py
--rw-r--r--   0        0        0    23996 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/applications.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/cleanse.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/embedding.py
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/inline_ckeditor.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/mixins.py
--rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/pages.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/regions.py
--rw-r--r--   0        0        0    13486 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/renderer.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/shortcuts.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/utils.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/plugins/__init__.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/plugins/external.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/plugins/html.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/plugins/image.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/plugins/old_richtext.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/plugins/richtext.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/plugins/snippet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/root/__init__.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/root/middleware.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/root/passthru.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/static/feincms3/box-drawing.css
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/static/feincms3/box-drawing.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/static/feincms3/inline-ckeditor-contents.css
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/static/feincms3/inline-ckeditor.css
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/static/feincms3/inline-ckeditor.js
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/static/feincms3/move-form.css
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/static/feincms3/plugin-ckeditor.css
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/static/feincms3/static-path-style.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/templatetags/__init__.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 feincms3-4.6.0/feincms3/templatetags/feincms3.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 feincms3-4.6.0/.gitignore
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 feincms3-4.6.0/LICENSE
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 feincms3-4.6.0/README.rst
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 feincms3-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 feincms3-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/__init__.py
+-rw-r--r--   0        0        0    18418 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/admin.py
+-rw-r--r--   0        0        0    23996 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/applications.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/cleanse.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/embedding.py
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/inline_ckeditor.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/mixins.py
+-rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/pages.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/regions.py
+-rw-r--r--   0        0        0    13486 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/renderer.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/shortcuts.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/utils.py
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/__init__.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/external.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/html.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/image.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/old_richtext.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/richtext.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/snippet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/root/__init__.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/root/middleware.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/root/passthru.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/box-drawing.css
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/box-drawing.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor-contents.css
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor.css
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor.js
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/move-form.css
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/plugin-ckeditor.css
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/static-path-style.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/templatetags/__init__.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/templatetags/feincms3.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 feincms3-4.6.1/.gitignore
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 feincms3-4.6.1/LICENSE
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 feincms3-4.6.1/README.rst
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 feincms3-4.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 feincms3-4.6.1/PKG-INFO
```

### Comparing `feincms3-4.6.0/feincms3/admin.py` & `feincms3-4.6.1/feincms3/admin.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/applications.py` & `feincms3-4.6.1/feincms3/applications.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/cleanse.py` & `feincms3-4.6.1/feincms3/cleanse.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/embedding.py` & `feincms3-4.6.1/feincms3/embedding.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/inline_ckeditor.py` & `feincms3-4.6.1/feincms3/inline_ckeditor.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/mixins.py` & `feincms3-4.6.1/feincms3/mixins.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/pages.py` & `feincms3-4.6.1/feincms3/pages.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/regions.py` & `feincms3-4.6.1/feincms3/regions.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/renderer.py` & `feincms3-4.6.1/feincms3/renderer.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/shortcuts.py` & `feincms3-4.6.1/feincms3/shortcuts.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/utils.py` & `feincms3-4.6.1/feincms3/utils.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/de/LC_MESSAGES/django.mo` & `feincms3-4.6.1/feincms3/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/de/LC_MESSAGES/django.po` & `feincms3-4.6.1/feincms3/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/en/LC_MESSAGES/django.po` & `feincms3-4.6.1/feincms3/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/fr/LC_MESSAGES/django.mo` & `feincms3-4.6.1/feincms3/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/fr/LC_MESSAGES/django.po` & `feincms3-4.6.1/feincms3/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/it/LC_MESSAGES/django.mo` & `feincms3-4.6.1/feincms3/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/it/LC_MESSAGES/django.po` & `feincms3-4.6.1/feincms3/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/nb_NO/LC_MESSAGES/django.mo` & `feincms3-4.6.1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/locale/nb_NO/LC_MESSAGES/django.po` & `feincms3-4.6.1/feincms3/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/plugins/__init__.py` & `feincms3-4.6.1/feincms3/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/plugins/external.py` & `feincms3-4.6.1/feincms3/plugins/external.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/plugins/html.py` & `feincms3-4.6.1/feincms3/plugins/html.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/plugins/image.py` & `feincms3-4.6.1/feincms3/plugins/image.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/plugins/old_richtext.py` & `feincms3-4.6.1/feincms3/plugins/old_richtext.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/plugins/richtext.py` & `feincms3-4.6.1/feincms3/plugins/richtext.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/plugins/snippet.py` & `feincms3-4.6.1/feincms3/plugins/snippet.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/root/middleware.py` & `feincms3-4.6.1/feincms3/root/middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,16 +44,39 @@
 from django.http import (
     HttpResponseNotFound,
     HttpResponsePermanentRedirect,
     HttpResponseRedirect,
 )
 
 
-class _UseRootMiddlewareResponse(HttpResponseNotFound):
-    """Used by feincms3.root.passthru to tell the middleware to do its thing"""
+class UseRootMiddlewareResponse(HttpResponseNotFound):
+    """
+    Used by feincms3.root.passthru to tell the middleware to do its thing
+
+    You can return this response from your own views as well if some view
+    cannot handle a request and you want to allow the root middleware to try
+    handling the current request. If you just raise ``Http404`` or return a
+    stock ``HttpResponseNotFound`` response the root middleware will do
+    nothing.
+
+    As an example, of ``get_object_or_404(Thing, pk=pk)`` you could do the
+    following if you want to fall back to the root middleware:
+
+    .. code-block:: python
+
+        from feincms3.root.middleware import UseRootMiddlewareResponse
+
+        def view(request, pk):
+            if thing := Thing.objects.filter(pk=pk).first():
+                return render(...)
+            return UseRootMiddlewareResponse()
+
+    This makes the root middleware check the pages for a match, and still
+    return the 404 if no page could be found.
+    """
 
 
 def create_page_if_404_middleware(*, queryset, handler, language_code_redirect=False):
     """
     Create a middleware for handling pages
 
     This utility is there for your convenience, you do not have to use it. The
@@ -77,18 +100,18 @@
     """
 
     def outer(get_response):
         def inner(request):
             response = get_response(request)
             if response.status_code != 404 or (
                 request.resolver_match
-                and not isinstance(response, _UseRootMiddlewareResponse)
+                and not isinstance(response, UseRootMiddlewareResponse)
             ):
                 # Response is not a 404 OR the 404 comes from a resolved view
-                # which also didn't return a _UseRootMiddlewareResponse.
+                # which also didn't return a UseRootMiddlewareResponse.
                 return response
             qs = queryset(request) if callable(queryset) else queryset._clone()
             if page := qs.filter(path=request.path_info).first():
                 return handler(request, page)
             if language_code_redirect and request.path_info == "/":
                 target = f"/{request.LANGUAGE_CODE}/"
                 if qs.filter(path=target).exists():
```

### Comparing `feincms3-4.6.0/feincms3/root/passthru.py` & `feincms3-4.6.1/feincms3/root/passthru.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 
 from functools import partial
 
 from django.urls import path
 from django.utils.functional import lazy
 
 from feincms3.applications import reverse_app
-from feincms3.root.middleware import _UseRootMiddlewareResponse
+from feincms3.root.middleware import UseRootMiddlewareResponse
 
 
 app_name = "passthru"
-urlpatterns = [path("", lambda request: _UseRootMiddlewareResponse(), name="passthru")]
+urlpatterns = [path("", lambda request: UseRootMiddlewareResponse(), name="passthru")]
 ignore_app_name_mismatch = True
 
 
 def reverse_passthru(namespace, **kwargs):
     """
     Reverse a passthru app URL
```

### Comparing `feincms3-4.6.0/feincms3/static/feincms3/box-drawing.css` & `feincms3-4.6.1/feincms3/static/feincms3/box-drawing.css`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/static/feincms3/box-drawing.js` & `feincms3-4.6.1/feincms3/static/feincms3/box-drawing.js`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/static/feincms3/inline-ckeditor.css` & `feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor.css`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/static/feincms3/inline-ckeditor.js` & `feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor.js`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/static/feincms3/move-form.css` & `feincms3-4.6.1/feincms3/static/feincms3/move-form.css`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/static/feincms3/static-path-style.js` & `feincms3-4.6.1/feincms3/static/feincms3/static-path-style.js`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/feincms3/templatetags/feincms3.py` & `feincms3-4.6.1/feincms3/templatetags/feincms3.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/LICENSE` & `feincms3-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/README.rst` & `feincms3-4.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/pyproject.toml` & `feincms3-4.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.0/PKG-INFO` & `feincms3-4.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: feincms3
-Version: 4.6.0
+Version: 4.6.1
 Summary: CMS-building toolkit for Django
 Project-URL: Homepage, https://github.com/matthiask/feincms3/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

