# Comparing `tmp/st_diff_viewer-1.0.3.tar.gz` & `tmp/st_diff_viewer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_diff_viewer-1.0.3.tar", max compression
+gzip compressed data, was "st_diff_viewer-1.0.4.tar", max compression
```

## Comparing `st_diff_viewer-1.0.3.tar` & `st_diff_viewer-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1063 2024-05-17 07:07:34.851441 st_diff_viewer-1.0.3/LICENSE
--rw-r--r--   0        0        0      735 2024-05-17 12:26:32.281665 st_diff_viewer-1.0.3/README.md
--rw-r--r--   0        0        0    10730 2024-05-17 10:20:33.150645 st_diff_viewer-1.0.3/docs/head.png
--rw-r--r--   0        0        0    37586 2024-05-17 09:21:13.808831 st_diff_viewer-1.0.3/docs/img.png
--rw-r--r--   0        0        0      699 2024-05-17 12:27:10.945701 st_diff_viewer-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2470 2024-05-17 12:21:04.651220 st_diff_viewer-1.0.3/st_diff_viewer/__init__.py
--rw-r--r--   0        0        0     2626 2024-05-17 12:27:08.021802 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/404.html
--rw-r--r--   0        0        0   233887 2024-05-17 12:27:07.664157 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js
--rw-r--r--   0        0        0   140973 2024-05-17 12:27:07.664280 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js
--rw-r--r--   0        0        0    95990 2024-05-17 12:27:07.664418 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/main-49701d22161bf8f9.js
--rw-r--r--   0        0        0      442 2024-05-17 12:27:07.665217 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/pages/_app-2ddf65715eee6393.js
--rw-r--r--   0        0        0      247 2024-05-17 12:27:07.665441 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
--rw-r--r--   0        0        0     1085 2024-05-17 12:27:07.665652 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js
--rw-r--r--   0        0        0    91381 2024-05-17 12:27:07.665179 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0        0        0     1485 2024-05-17 12:27:07.664694 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/webpack-88e841e08c00aeb1.js
--rw-r--r--   0        0        0     4386 2024-05-17 12:27:07.664845 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/css/34e82990737d7da2.css
--rw-r--r--   0        0        0      321 2024-05-17 12:27:07.664951 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/eevQmOyAWWKyTH0eX_1RU/_buildManifest.js
--rw-r--r--   0        0        0       77 2024-05-17 12:27:07.665232 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/eevQmOyAWWKyTH0eX_1RU/_ssgManifest.js
--rw-r--r--   0        0        0    25931 2024-05-17 12:27:07.667905 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/favicon.ico
--rw-r--r--   0        0        0     1986 2024-05-17 12:27:07.953071 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/index.html
--rw-r--r--   0        0        0     1101 2024-05-17 12:27:07.667296 st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/vercel.svg
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 st_diff_viewer-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 07:07:34.851441 st_diff_viewer-1.0.4/LICENSE
+-rw-r--r--   0        0        0      675 2024-05-23 17:22:40.512885 st_diff_viewer-1.0.4/README.md
+-rw-r--r--   0        0        0     6142 2024-05-23 17:21:45.626693 st_diff_viewer-1.0.4/docs/head.png
+-rw-r--r--   0        0        0    29458 2024-05-23 17:21:45.655564 st_diff_viewer-1.0.4/docs/img.png
+-rw-r--r--   0        0        0      699 2024-05-24 02:04:06.442333 st_diff_viewer-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2533 2024-05-23 17:25:36.175010 st_diff_viewer-1.0.4/st_diff_viewer/__init__.py
+-rw-r--r--   0        0        0     2626 2024-05-24 02:04:04.050732 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/404.html
+-rw-r--r--   0        0        0   233887 2024-05-24 02:04:03.728577 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js
+-rw-r--r--   0        0        0   140973 2024-05-24 02:04:03.728664 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js
+-rw-r--r--   0        0        0    95990 2024-05-24 02:04:03.728673 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/main-49701d22161bf8f9.js
+-rw-r--r--   0        0        0      442 2024-05-24 02:04:03.729725 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/pages/_app-2ddf65715eee6393.js
+-rw-r--r--   0        0        0      247 2024-05-24 02:04:03.729949 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+-rw-r--r--   0        0        0     1085 2024-05-24 02:04:03.730149 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js
+-rw-r--r--   0        0        0    91381 2024-05-24 02:04:03.729192 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0        0        0     1485 2024-05-24 02:04:03.729220 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/webpack-88e841e08c00aeb1.js
+-rw-r--r--   0        0        0     4386 2024-05-24 02:04:03.729524 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/css/34e82990737d7da2.css
+-rw-r--r--   0        0        0      321 2024-05-24 02:04:03.729512 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/ftCWcu7KKXq4NEPlC1nzp/_buildManifest.js
+-rw-r--r--   0        0        0       77 2024-05-24 02:04:03.729828 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/ftCWcu7KKXq4NEPlC1nzp/_ssgManifest.js
+-rw-r--r--   0        0        0    25931 2024-05-24 02:04:03.732819 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/favicon.ico
+-rw-r--r--   0        0        0     1986 2024-05-24 02:04:03.999548 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/index.html
+-rw-r--r--   0        0        0     1090 2024-05-24 02:04:03.732827 st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/vercel.svg
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 st_diff_viewer-1.0.4/PKG-INFO
```

### Comparing `st_diff_viewer-1.0.3/LICENSE` & `st_diff_viewer-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/README.md` & `st_diff_viewer-1.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# [streamlit-diff-viewer](https://github.com/LinXueyuanStdio/streamlit-diff-viewer)
+# streamlit-diff-viewer
 git-like diff viewer for streamlit webapp
 
 ![](docs/head.png)
 
 ## Installation
 
 ```bash
```

### Comparing `st_diff_viewer-1.0.3/pyproject.toml` & `st_diff_viewer-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "st-diff-viewer"
-version = "1.0.3"
+version = "1.0.4"
 description = "A Streamlit component to display diff betoween two strings"
 authors = ["Xueyuan Lin <linxy59@mail2.sysu.eud.cn>"]
 readme = "README.md"
 packages = [{ include = "st_diff_viewer"}]
 
 license = "MIT"
```

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/__init__.py` & `st_diff_viewer-1.0.4/st_diff_viewer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     disabled_word_diff: Optional[bool] = False,
     left_title: Optional[str] = None,
     right_title: Optional[str] = None,
     use_dark_theme: Optional[bool] = False,
     extra_lines_surrounding_diff: Optional[int] = 3,
     hide_line_numbers: Optional[bool] = False,
     highlight_lines: Optional[List[str]] = [],
+    key=None,
+    **kwargs,
 ):
     """
     Creates a new instance of streamlit-diff-viewer component
 
     Parameters
     ----------
     old_text: str
@@ -68,8 +70,10 @@
         disabledWordDiff=disabled_word_diff,
         leftTitle=left_title,
         rightTitle=right_title,
         useDarkTheme=use_dark_theme,
         extraLinesSurroundingDiff=extra_lines_surrounding_diff,
         hideLineNumbers=hide_line_numbers,
         highlightLines=highlight_lines,
+        key=key,
+        **kwargs,
     )
```

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/404.html` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/404.html`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/webpack-88e841e08c00aeb1.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/main-49701d22161bf8f9.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/eevQmOyAWWKyTH0eX_1RU/_buildManifest.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/eevQmOyAWWKyTH0eX_1RU/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"eevQmOyAWWKyTH0eX_1RU","assetPrefix":"/component/st_diff_viewer.st_diff_viewer","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/webpack-88e841e08c00aeb1.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/main-49701d22161bf8f9.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/ftCWcu7KKXq4NEPlC1nzp/_buildManifest.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/ftCWcu7KKXq4NEPlC1nzp/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"ftCWcu7KKXq4NEPlC1nzp","assetPrefix":"/component/st_diff_viewer.st_diff_viewer","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/92-bf787e1cee9c20db.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/framework-c0663f0e1a0e4372.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/main-49701d22161bf8f9.js` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/main-49701d22161bf8f9.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/pages/index-08087b43971404a5.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/chunks/webpack-88e841e08c00aeb1.js` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/chunks/webpack-88e841e08c00aeb1.js`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/_next/static/css/34e82990737d7da2.css` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/_next/static/css/34e82990737d7da2.css`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/favicon.ico` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/favicon.ico`

 * *Files identical despite different names*

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/index.html` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Create Next App</title><meta name="description" content="Generated by create next app"/><link rel="icon" href="/favicon.ico"/><meta name="next-head-count" content="5"/><link rel="preload" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/webpack-88e841e08c00aeb1.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/main-49701d22161bf8f9.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/92-bf787e1cee9c20db.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/index-08087b43971404a5.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/eevQmOyAWWKyTH0eX_1RU/_buildManifest.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/eevQmOyAWWKyTH0eX_1RU/_ssgManifest.js" defer=""></script></head><body><div id="__next"></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"eevQmOyAWWKyTH0eX_1RU","assetPrefix":"/component/st_diff_viewer.st_diff_viewer","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Create Next App</title><meta name="description" content="Generated by create next app"/><link rel="icon" href="/favicon.ico"/><meta name="next-head-count" content="5"/><link rel="preload" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" as="style"/><link rel="stylesheet" href="/component/st_diff_viewer.st_diff_viewer/_next/static/css/34e82990737d7da2.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/webpack-88e841e08c00aeb1.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/framework-c0663f0e1a0e4372.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/main-49701d22161bf8f9.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/_app-2ddf65715eee6393.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/92-bf787e1cee9c20db.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/chunks/pages/index-08087b43971404a5.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/ftCWcu7KKXq4NEPlC1nzp/_buildManifest.js" defer=""></script><script src="/component/st_diff_viewer.st_diff_viewer/_next/static/ftCWcu7KKXq4NEPlC1nzp/_ssgManifest.js" defer=""></script></head><body><div id="__next"></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"ftCWcu7KKXq4NEPlC1nzp","assetPrefix":"/component/st_diff_viewer.st_diff_viewer","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `st_diff_viewer-1.0.3/st_diff_viewer/frontend/out/vercel.svg` & `st_diff_viewer-1.0.4/st_diff_viewer/frontend/out/vercel.svg`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-00000000: 3c73 7667 2077 6964 7468 3d22 3238 3322  <svg width="283"
-00000010: 2068 6569 6768 743d 2236 3422 2076 6965   height="64" vie
-00000020: 7742 6f78 3d22 3020 3020 3238 3320 3634  wBox="0 0 283 64
-00000030: 2220 6669 6c6c 3d22 6e6f 6e65 2220 0a20  " fill="none" . 
-00000040: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
-00000050: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
-00000060: 2f73 7667 223e 0a20 2020 203c 7061 7468  /svg">.    <path
-00000070: 2064 3d22 4d31 3431 2e30 3420 3136 632d   d="M141.04 16c-
-00000080: 3131 2e30 3420 302d 3139 2037 2e32 2d31  11.04 0-19 7.2-1
-00000090: 3920 3138 7338 2e39 3620 3138 2032 3020  9 18s8.96 18 20 
-000000a0: 3138 6336 2e36 3720 3020 3132 2e35 352d  18c6.67 0 12.55-
-000000b0: 322e 3634 2031 362e 3139 2d37 2e30 396c  2.64 16.19-7.09l
-000000c0: 2d37 2e36 352d 342e 3432 632d 322e 3032  -7.65-4.42c-2.02
-000000d0: 2032 2e32 312d 352e 3039 2033 2e35 2d38   2.21-5.09 3.5-8
-000000e0: 2e35 3420 332e 352d 342e 3739 2030 2d38  .54 3.5-4.79 0-8
-000000f0: 2e38 362d 322e 352d 3130 2e33 372d 362e  .86-2.5-10.37-6.
-00000100: 3568 3238 2e30 3263 2e32 322d 312e 3132  5h28.02c.22-1.12
-00000110: 2e33 352d 322e 3238 2e33 352d 332e 3520  .35-2.28.35-3.5 
-00000120: 302d 3130 2e37 392d 372e 3936 2d31 372e  0-10.79-7.96-17.
-00000130: 3939 2d31 392d 3137 2e39 397a 6d2d 392e  99-19-17.99zm-9.
-00000140: 3436 2031 342e 3563 312e 3235 2d33 2e39  46 14.5c1.25-3.9
-00000150: 3920 342e 3637 2d36 2e35 2039 2e34 352d  9 4.67-6.5 9.45-
-00000160: 362e 3520 342e 3739 2030 2038 2e32 3120  6.5 4.79 0 8.21 
-00000170: 322e 3531 2039 2e34 3520 362e 3568 2d31  2.51 9.45 6.5h-1
-00000180: 382e 397a 4d32 3438 2e37 3220 3136 632d  8.9zM248.72 16c-
-00000190: 3131 2e30 3420 302d 3139 2037 2e32 2d31  11.04 0-19 7.2-1
-000001a0: 3920 3138 7338 2e39 3620 3138 2032 3020  9 18s8.96 18 20 
-000001b0: 3138 6336 2e36 3720 3020 3132 2e35 352d  18c6.67 0 12.55-
-000001c0: 322e 3634 2031 362e 3139 2d37 2e30 396c  2.64 16.19-7.09l
-000001d0: 2d37 2e36 352d 342e 3432 632d 322e 3032  -7.65-4.42c-2.02
-000001e0: 2032 2e32 312d 352e 3039 2033 2e35 2d38   2.21-5.09 3.5-8
-000001f0: 2e35 3420 332e 352d 342e 3739 2030 2d38  .54 3.5-4.79 0-8
-00000200: 2e38 362d 322e 352d 3130 2e33 372d 362e  .86-2.5-10.37-6.
-00000210: 3568 3238 2e30 3263 2e32 322d 312e 3132  5h28.02c.22-1.12
-00000220: 2e33 352d 322e 3238 2e33 352d 332e 3520  .35-2.28.35-3.5 
-00000230: 302d 3130 2e37 392d 372e 3936 2d31 372e  0-10.79-7.96-17.
-00000240: 3939 2d31 392d 3137 2e39 397a 6d2d 392e  99-19-17.99zm-9.
-00000250: 3435 2031 342e 3563 312e 3235 2d33 2e39  45 14.5c1.25-3.9
-00000260: 3920 342e 3637 2d36 2e35 2039 2e34 352d  9 4.67-6.5 9.45-
-00000270: 362e 3520 342e 3739 2030 2038 2e32 3120  6.5 4.79 0 8.21 
-00000280: 322e 3531 2039 2e34 3520 362e 3568 2d31  2.51 9.45 6.5h-1
-00000290: 382e 397a 4d32 3030 2e32 3420 3334 6330  8.9zM200.24 34c0
-000002a0: 2036 2033 2e39 3220 3130 2031 3020 3130   6 3.92 10 10 10
-000002b0: 2034 2e31 3220 3020 372e 3231 2d31 2e38   4.12 0 7.21-1.8
-000002c0: 3720 382e 382d 342e 3932 6c37 2e36 3820  7 8.8-4.92l7.68 
-000002d0: 342e 3433 632d 332e 3138 2035 2e33 2d39  4.43c-3.18 5.3-9
-000002e0: 2e31 3420 382e 3439 2d31 362e 3438 2038  .14 8.49-16.48 8
-000002f0: 2e34 392d 3131 2e30 3520 302d 3139 2d37  .49-11.05 0-19-7
-00000300: 2e32 2d31 392d 3138 7337 2e39 362d 3138  .2-19-18s7.96-18
-00000310: 2031 392d 3138 6337 2e33 3420 3020 3133   19-18c7.34 0 13
-00000320: 2e32 3920 332e 3139 2031 362e 3438 2038  .29 3.19 16.48 8
-00000330: 2e34 396c 2d37 2e36 3820 342e 3433 632d  .49l-7.68 4.43c-
-00000340: 312e 3539 2d33 2e30 352d 342e 3638 2d34  1.59-3.05-4.68-4
-00000350: 2e39 322d 382e 382d 342e 3932 2d36 2e30  .92-8.8-4.92-6.0
-00000360: 3720 302d 3130 2034 2d31 3020 3130 7a6d  7 0-10 4-10 10zm
-00000370: 3832 2e34 382d 3239 7634 3668 2d39 5635  82.48-29v46h-9V5
-00000380: 6839 7a4d 3336 2e39 3520 304c 3733 2e39  h9zM36.95 0L73.9
-00000390: 2036 3448 304c 3336 2e39 3520 307a 6d39   64H0L36.95 0zm9
-000003a0: 322e 3338 2035 6c2d 3237 2e37 3120 3438  2.38 5l-27.71 48
-000003b0: 4c37 332e 3931 2035 4838 342e 336c 3137  L73.91 5H84.3l17
-000003c0: 2e33 3220 3330 2031 372e 3332 2d33 3068  .32 30 17.32-30h
-000003d0: 3130 2e33 397a 6d35 382e 3931 2031 3276  10.39zm58.91 12v
-000003e0: 392e 3639 632d 312d 2e32 392d 322e 3036  9.69c-1-.29-2.06
-000003f0: 2d2e 3439 2d33 2e32 2d2e 3439 2d35 2e38  -.49-3.2-.49-5.8
-00000400: 3120 302d 3130 2034 2d31 3020 3130 5635  1 0-10 4-10 10V5
-00000410: 3168 2d39 5631 3768 3976 392e 3263 302d  1h-9V17h9v9.2c0-
-00000420: 352e 3038 2035 2e39 312d 392e 3220 3133  5.08 5.91-9.2 13
-00000430: 2e32 2d39 2e32 7a22 2066 696c 6c3d 2223  .2-9.2z" fill="#
-00000440: 3030 3022 2f3e 0a3c 2f73 7667 3e         000"/>.</svg>
+00000000: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
+00000010: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00000020: 3030 2f73 7667 2220 7769 6474 683d 2232  00/svg" width="2
+00000030: 3833 2220 6865 6967 6874 3d22 3634 2220  83" height="64" 
+00000040: 6669 6c6c 3d22 6e6f 6e65 2220 7669 6577  fill="none" view
+00000050: 426f 783d 2230 2030 2032 3833 2036 3422  Box="0 0 283 64"
+00000060: 3e3c 7061 7468 2066 696c 6c3d 2223 3030  ><path fill="#00
+00000070: 3022 2064 3d22 4d31 3431 2e30 3420 3136  0" d="M141.04 16
+00000080: 632d 3131 2e30 3420 302d 3139 2037 2e32  c-11.04 0-19 7.2
+00000090: 2d31 3920 3138 7338 2e39 3620 3138 2032  -19 18s8.96 18 2
+000000a0: 3020 3138 6336 2e36 3720 3020 3132 2e35  0 18c6.67 0 12.5
+000000b0: 352d 322e 3634 2031 362e 3139 2d37 2e30  5-2.64 16.19-7.0
+000000c0: 396c 2d37 2e36 352d 342e 3432 632d 322e  9l-7.65-4.42c-2.
+000000d0: 3032 2032 2e32 312d 352e 3039 2033 2e35  02 2.21-5.09 3.5
+000000e0: 2d38 2e35 3420 332e 352d 342e 3739 2030  -8.54 3.5-4.79 0
+000000f0: 2d38 2e38 362d 322e 352d 3130 2e33 372d  -8.86-2.5-10.37-
+00000100: 362e 3568 3238 2e30 3263 2e32 322d 312e  6.5h28.02c.22-1.
+00000110: 3132 2e33 352d 322e 3238 2e33 352d 332e  12.35-2.28.35-3.
+00000120: 3520 302d 3130 2e37 392d 372e 3936 2d31  5 0-10.79-7.96-1
+00000130: 372e 3939 2d31 392d 3137 2e39 397a 6d2d  7.99-19-17.99zm-
+00000140: 392e 3436 2031 342e 3563 312e 3235 2d33  9.46 14.5c1.25-3
+00000150: 2e39 3920 342e 3637 2d36 2e35 2039 2e34  .99 4.67-6.5 9.4
+00000160: 352d 362e 3520 342e 3739 2030 2038 2e32  5-6.5 4.79 0 8.2
+00000170: 3120 322e 3531 2039 2e34 3520 362e 3568  1 2.51 9.45 6.5h
+00000180: 2d31 382e 397a 4d32 3438 2e37 3220 3136  -18.9zM248.72 16
+00000190: 632d 3131 2e30 3420 302d 3139 2037 2e32  c-11.04 0-19 7.2
+000001a0: 2d31 3920 3138 7338 2e39 3620 3138 2032  -19 18s8.96 18 2
+000001b0: 3020 3138 6336 2e36 3720 3020 3132 2e35  0 18c6.67 0 12.5
+000001c0: 352d 322e 3634 2031 362e 3139 2d37 2e30  5-2.64 16.19-7.0
+000001d0: 396c 2d37 2e36 352d 342e 3432 632d 322e  9l-7.65-4.42c-2.
+000001e0: 3032 2032 2e32 312d 352e 3039 2033 2e35  02 2.21-5.09 3.5
+000001f0: 2d38 2e35 3420 332e 352d 342e 3739 2030  -8.54 3.5-4.79 0
+00000200: 2d38 2e38 362d 322e 352d 3130 2e33 372d  -8.86-2.5-10.37-
+00000210: 362e 3568 3238 2e30 3263 2e32 322d 312e  6.5h28.02c.22-1.
+00000220: 3132 2e33 352d 322e 3238 2e33 352d 332e  12.35-2.28.35-3.
+00000230: 3520 302d 3130 2e37 392d 372e 3936 2d31  5 0-10.79-7.96-1
+00000240: 372e 3939 2d31 392d 3137 2e39 397a 6d2d  7.99-19-17.99zm-
+00000250: 392e 3435 2031 342e 3563 312e 3235 2d33  9.45 14.5c1.25-3
+00000260: 2e39 3920 342e 3637 2d36 2e35 2039 2e34  .99 4.67-6.5 9.4
+00000270: 352d 362e 3520 342e 3739 2030 2038 2e32  5-6.5 4.79 0 8.2
+00000280: 3120 322e 3531 2039 2e34 3520 362e 3568  1 2.51 9.45 6.5h
+00000290: 2d31 382e 397a 4d32 3030 2e32 3420 3334  -18.9zM200.24 34
+000002a0: 6330 2036 2033 2e39 3220 3130 2031 3020  c0 6 3.92 10 10 
+000002b0: 3130 2034 2e31 3220 3020 372e 3231 2d31  10 4.12 0 7.21-1
+000002c0: 2e38 3720 382e 382d 342e 3932 6c37 2e36  .87 8.8-4.92l7.6
+000002d0: 3820 342e 3433 632d 332e 3138 2035 2e33  8 4.43c-3.18 5.3
+000002e0: 2d39 2e31 3420 382e 3439 2d31 362e 3438  -9.14 8.49-16.48
+000002f0: 2038 2e34 392d 3131 2e30 3520 302d 3139   8.49-11.05 0-19
+00000300: 2d37 2e32 2d31 392d 3138 7337 2e39 362d  -7.2-19-18s7.96-
+00000310: 3138 2031 392d 3138 6337 2e33 3420 3020  18 19-18c7.34 0 
+00000320: 3133 2e32 3920 332e 3139 2031 362e 3438  13.29 3.19 16.48
+00000330: 2038 2e34 396c 2d37 2e36 3820 342e 3433   8.49l-7.68 4.43
+00000340: 632d 312e 3539 2d33 2e30 352d 342e 3638  c-1.59-3.05-4.68
+00000350: 2d34 2e39 322d 382e 382d 342e 3932 2d36  -4.92-8.8-4.92-6
+00000360: 2e30 3720 302d 3130 2034 2d31 3020 3130  .07 0-10 4-10 10
+00000370: 7a6d 3832 2e34 382d 3239 7634 3668 2d39  zm82.48-29v46h-9
+00000380: 5635 6839 7a4d 3336 2e39 3520 304c 3733  V5h9zM36.95 0L73
+00000390: 2e39 2036 3448 304c 3336 2e39 3520 307a  .9 64H0L36.95 0z
+000003a0: 6d39 322e 3338 2035 6c2d 3237 2e37 3120  m92.38 5l-27.71 
+000003b0: 3438 4c37 332e 3931 2035 4838 342e 336c  48L73.91 5H84.3l
+000003c0: 3137 2e33 3220 3330 2031 372e 3332 2d33  17.32 30 17.32-3
+000003d0: 3068 3130 2e33 397a 6d35 382e 3931 2031  0h10.39zm58.91 1
+000003e0: 3276 392e 3639 632d 312d 2e32 392d 322e  2v9.69c-1-.29-2.
+000003f0: 3036 2d2e 3439 2d33 2e32 2d2e 3439 2d35  06-.49-3.2-.49-5
+00000400: 2e38 3120 302d 3130 2034 2d31 3020 3130  .81 0-10 4-10 10
+00000410: 5635 3168 2d39 5631 3768 3976 392e 3263  V51h-9V17h9v9.2c
+00000420: 302d 352e 3038 2035 2e39 312d 392e 3220  0-5.08 5.91-9.2 
+00000430: 3133 2e32 2d39 2e32 7a22 2f3e 3c2f 7376  13.2-9.2z"/></sv
+00000440: 673e                                     g>
```

### Comparing `st_diff_viewer-1.0.3/PKG-INFO` & `st_diff_viewer-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-diff-viewer
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Streamlit component to display diff betoween two strings
 License: MIT
 Author: Xueyuan Lin
 Author-email: linxy59@mail2.sysu.eud.cn
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: streamlit (>=0.63)
 Description-Content-Type: text/markdown
 
-# [streamlit-diff-viewer](https://github.com/LinXueyuanStdio/streamlit-diff-viewer)
+# streamlit-diff-viewer
 git-like diff viewer for streamlit webapp
 
 ![](docs/head.png)
 
 ## Installation
 
 ```bash
```

