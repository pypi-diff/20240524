# Comparing `tmp/c6t-0.0.5.tar.gz` & `tmp/c6t-0.0.6.tar.gz`

## Comparing `c6t-0.0.5.tar` & `c6t-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.5/.python-version
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 c6t-0.0.5/requirements-dev.lock
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 c6t-0.0.5/requirements.lock
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.5/.github/workflows/dump-env.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/__main__.py
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/api/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/api/agent_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/configure/__init__.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/configure/credentials.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/external/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/external/integrations/scw/__init__.py
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/external/integrations/scw/contrast_api.py
--rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/external/integrations/scw/contrast_scw.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/templates/contrast_security.yaml.j2
--rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 c6t-0.0.5/src/c6t/ui/auth.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.5/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 c6t-0.0.5/LICENSE
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 c6t-0.0.5/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 c6t-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 c6t-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.6/.python-version
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 c6t-0.0.6/requirements-dev.lock
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 c6t-0.0.6/requirements.lock
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 c6t-0.0.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.6/.github/workflows/dump-env.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/__main__.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/api/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/api/agent_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/configure/__init__.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/configure/credentials.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/external/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/external/integrations/scw/__init__.py
+-rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/external/integrations/scw/contrast_api.py
+-rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/external/integrations/scw/contrast_scw.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/templates/contrast_security.yaml.j2
+-rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/ui/auth.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 c6t-0.0.6/LICENSE
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 c6t-0.0.6/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 c6t-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 c6t-0.0.6/PKG-INFO
```

### Comparing `c6t-0.0.5/requirements-dev.lock` & `c6t-0.0.6/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/requirements.lock` & `c6t-0.0.6/requirements.lock`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/src/c6t/cli.py` & `c6t-0.0.6/src/c6t/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import typer
 import yaml
-import pathlib
 from git.repo import Repo
-from jinja2 import Environment, FileSystemLoader
+from jinja2 import Environment, PackageLoader, select_autoescape
 
 from rich import print as rprint
 
 import questionary
 
 from c6t.configure.credentials import ContrastAPICredentials
 from c6t.ui.auth import ContrastUIAuthManager
@@ -99,17 +98,19 @@
     rprint("Getting agent config from TeamServer...")
     agent_config = AgentConfig(profile=profile)
     raw_yaml_text = agent_config.get_agent_credentials(language=language)
     credentials = yaml.safe_load(raw_yaml_text).get("api")
 
     # Load Jinga2 template and render using YAML text
     rprint("Rendering agent config...")
-    template_path = pathlib.Path("~/.c6t/templates").expanduser()
-    template_loader = FileSystemLoader(searchpath=template_path)
-    template_env = Environment(loader=template_loader)
+    # template_path = pathlib.Path("~/.c6t/templates").expanduser()
+    # template_loader = FileSystemLoader(searchpath=template_path)
+    template_env = Environment(
+        loader=PackageLoader("c6t", "templates"), autoescape=select_autoescape(["yaml"])
+    )
     template = template_env.get_template("contrast_security.yaml.j2")
     rendered_yaml_text = template.render(
         url=credentials.get("url"),
         api_key=credentials.get("api_key"),
         service_key=credentials.get("service_key"),
         user_name=credentials.get("user_name"),
         application_name=f"TerracottaBank-{initials}",
@@ -120,15 +121,14 @@
         environment=environment,
     )
 
     rprint("Writing agent config to file...")
     agent_config.write_agent_config_to_file(path=path, yaml_text=rendered_yaml_text)
 
 
-# TODO: Add a command to populate vulnerability references with Secure Code Warrior links
 @scw_integration_app.command("create")
 def scw(profile: str = "default") -> None:
     """
     Populate vulnerability references with Secure Code Warrior links.
     """
     print("Creating SCW links...")
     scw_create(profile=profile)
```

### Comparing `c6t-0.0.5/src/c6t/api/agent_config.py` & `c6t-0.0.6/src/c6t/api/agent_config.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/src/c6t/configure/credentials.py` & `c6t-0.0.6/src/c6t/configure/credentials.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/src/c6t/external/integrations/scw/contrast_api.py` & `c6t-0.0.6/src/c6t/external/integrations/scw/contrast_api.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/src/c6t/external/integrations/scw/contrast_scw.py` & `c6t-0.0.6/src/c6t/external/integrations/scw/contrast_scw.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/src/c6t/ui/auth.py` & `c6t-0.0.6/src/c6t/ui/auth.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/.gitignore` & `c6t-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/README.md` & `c6t-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `c6t-0.0.5/pyproject.toml` & `c6t-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "c6t"
-version = "0.0.5"
+version = "0.0.6"
 description = "Unofficial Administrative Command Line Interface for Contrast Security"
 authors = [
     { name = "Jonathan Harper", email = "39912347+jharper-sec@users.noreply.github.com" },
 ]
 dependencies = [
     "requests>=2.32.0",
     "shellingham>=1.5.4",
```

