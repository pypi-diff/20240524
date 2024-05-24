# Comparing `tmp/langchainhub-0.1.8.tar.gz` & `tmp/langchainhub-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchainhub-0.1.8.tar", max compression
+gzip compressed data, was "langchainhub-0.1.9.tar", max compression
```

## Comparing `langchainhub-0.1.8.tar` & `langchainhub-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-08-03 22:00:27.715972 langchainhub-0.1.8/README.md
--rw-r--r--   0        0        0       61 2023-08-03 21:10:04.137469 langchainhub-0.1.8/langchainhub/__init__.py
--rw-r--r--   0        0        0     7639 2023-08-24 23:50:30.763898 langchainhub-0.1.8/langchainhub/client.py
--rw-r--r--   0        0        0      748 2023-08-24 23:51:38.615365 langchainhub-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 langchainhub-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 22:00:27.715972 langchainhub-0.1.9/README.md
+-rw-r--r--   0        0        0       61 2023-08-03 21:10:04.137469 langchainhub-0.1.9/langchainhub/__init__.py
+-rw-r--r--   0        0        0     7758 2023-08-25 00:27:33.458353 langchainhub-0.1.9/langchainhub/client.py
+-rw-r--r--   0        0        0      748 2023-08-25 00:30:22.670376 langchainhub-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 langchainhub-0.1.9/PKG-INFO
```

### Comparing `langchainhub-0.1.8/langchainhub/client.py` & `langchainhub-0.1.9/langchainhub/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     if api_key is None or not api_key.strip():
         return None
     return api_key.strip().strip('"').strip("'") or None
 
 
 def _get_api_url(api_url: Optional[str], has_api_key: bool = False) -> str:
     default_api_url = (
-        "https://dev.api.hub.langchain.com"
+        "https://beta.api.hub.langchain.com"
         if has_api_key
-        else "https://dev.public.hub.langchain.com"
+        else "https://beta.public.hub.langchain.com"
     )
     _api_url = (
         api_url
         if api_url is not None
         else os.getenv(
             "LANGCHAIN_HUB_API_URL",
             default_api_url,
@@ -89,14 +89,16 @@
         return headers
 
     @property
     def _host_url(self) -> str:
         """The web host url."""
         if _is_localhost(self.api_url):
             link = "http://localhost"
+        elif "beta" in self.api_url.split(".", maxsplit=1)[0]:
+            link = "https://beta.smith.langchain.com"
         elif "dev" in self.api_url.split(".", maxsplit=1)[0]:
             link = "https://dev.smith.langchain.com"
         else:
             link = "https://smith.langchain.com"
         return link
 
     def get_settings(self):
```

### Comparing `langchainhub-0.1.8/pyproject.toml` & `langchainhub-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchainhub"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["LangChain <support@langchain.dev>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 requests = "^2"
```

