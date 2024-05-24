# Comparing `tmp/c6t-0.0.6.tar.gz` & `tmp/c6t-0.0.7.tar.gz`

## Comparing `c6t-0.0.6.tar` & `c6t-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.6/.python-version
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 c6t-0.0.6/requirements-dev.lock
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 c6t-0.0.6/requirements.lock
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 c6t-0.0.6/.github/dependabot.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.6/.github/workflows/dump-env.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/__main__.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/api/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/api/agent_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/configure/__init__.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/configure/credentials.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/external/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/external/integrations/scw/__init__.py
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/external/integrations/scw/contrast_api.py
--rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/external/integrations/scw/contrast_scw.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/templates/contrast_security.yaml.j2
--rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 c6t-0.0.6/src/c6t/ui/auth.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.6/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 c6t-0.0.6/LICENSE
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 c6t-0.0.6/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 c6t-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 c6t-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.7/.python-version
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 c6t-0.0.7/requirements-dev.lock
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 c6t-0.0.7/requirements.lock
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 c6t-0.0.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.7/.github/workflows/dump-env.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/__main__.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/api/__init__.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/api/agent_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/configure/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/configure/credentials.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/external/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/external/integrations/scw/__init__.py
+-rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/external/integrations/scw/contrast_api.py
+-rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/external/integrations/scw/contrast_scw.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/templates/contrast_security.yaml.j2
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/templates/contrast_security_env.yaml.j2
+-rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 c6t-0.0.7/src/c6t/ui/auth.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 c6t-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 c6t-0.0.7/LICENSE
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 c6t-0.0.7/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 c6t-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 c6t-0.0.7/PKG-INFO
```

### Comparing `c6t-0.0.6/requirements-dev.lock` & `c6t-0.0.7/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `c6t-0.0.6/requirements.lock` & `c6t-0.0.7/requirements.lock`

 * *Files identical despite different names*

### Comparing `c6t-0.0.6/.github/dependabot.yml` & `c6t-0.0.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `c6t-0.0.6/src/c6t/cli.py` & `c6t-0.0.7/src/c6t/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from typing import Optional
+
 import typer
 import yaml
 from git.repo import Repo
-from jinja2 import Environment, PackageLoader, select_autoescape
+from git.exc import InvalidGitRepositoryError
+from jinja2 import Environment, PackageLoader
 
 from rich import print as rprint
 
 import questionary
 
 from c6t.configure.credentials import ContrastAPICredentials
 from c6t.ui.auth import ContrastUIAuthManager
@@ -75,73 +78,108 @@
     credentials.superadmin = typer.confirm("Contrast superadmin status")
     credentials.write_credentials_to_file()
 
 
 @app.command("agent-config")
 def agent_config(
     profile: str = "default",
-    path: str = "contrast_security.yaml",
+    type: str = "yaml",
+    path: Optional[str] = None,
+    application_name: Optional[str] = None,
+    environment: str = "dev",
     language: str = "JAVA",
+    include_credentials: bool = True,
 ) -> None:
     """
     Gets the Contrast Agent YAML config file from TeamServer
     and saves it to the current working directory.
     """
 
-    # Get initials from user input
-    initials = typer.prompt("Enter your initials")
-    environment = "dev"
+    branch_name: Optional[str] = None
+    commit_hash: Optional[str] = None
+    committer: Optional[str] = None
+    repository: Optional[str] = None
 
     # Attach to repo in current working directory
-    repo = Repo(".")
+    try:
+        repo = Repo(".")
+        branch_name = str(repo.active_branch)
+        commit_hash = str(repo.head.commit)
+        committer = str(repo.head.commit.author)
+        repository = str(repo.remotes.origin.url)
+    except InvalidGitRepositoryError:
+        rprint("This command must be run in a git repository.")
 
     # Get credentials from file
     rprint("Getting agent config from TeamServer...")
     agent_config = AgentConfig(profile=profile)
     raw_yaml_text = agent_config.get_agent_credentials(language=language)
     credentials = yaml.safe_load(raw_yaml_text).get("api")
 
     # Load Jinga2 template and render using YAML text
     rprint("Rendering agent config...")
-    # template_path = pathlib.Path("~/.c6t/templates").expanduser()
-    # template_loader = FileSystemLoader(searchpath=template_path)
     template_env = Environment(
-        loader=PackageLoader("c6t", "templates"), autoescape=select_autoescape(["yaml"])
+        loader=PackageLoader("c6t", "templates"),
+    )
+
+    yaml_template = template_env.get_template("contrast_security.yaml.j2")
+    env_template = template_env.get_template("contrast_security_env.yaml.j2")
+
+    rendered_yaml_text = yaml_template.render(
+        url=credentials.get("url"),
+        api_key=credentials.get("api_key"),
+        service_key=credentials.get("service_key"),
+        user_name=credentials.get("user_name"),
+        application_name=application_name,
+        branch_name=branch_name,
+        commit_hash=commit_hash,
+        committer=committer,
+        repository=repository,
+        environment=environment,
+        include_credentials=include_credentials,
     )
-    template = template_env.get_template("contrast_security.yaml.j2")
-    rendered_yaml_text = template.render(
+
+    rendered_env_text = env_template.render(
         url=credentials.get("url"),
         api_key=credentials.get("api_key"),
         service_key=credentials.get("service_key"),
         user_name=credentials.get("user_name"),
-        application_name=f"TerracottaBank-{initials}",
-        branch_name=repo.active_branch,
-        commit_hash=repo.head.commit,
-        committer=repo.head.commit.author,
-        repository=repo.remotes.origin.url,
+        application_name=application_name,
+        branch_name=branch_name,
+        commit_hash=commit_hash,
+        committer=committer,
+        repository=repository,
         environment=environment,
+        include_credentials=include_credentials,
     )
 
     rprint("Writing agent config to file...")
-    agent_config.write_agent_config_to_file(path=path, yaml_text=rendered_yaml_text)
+    if type == "yaml":
+        if path is None:
+            path = "contrast_security.yaml"
+        agent_config.write_agent_config_to_file(path=path, text=rendered_yaml_text)
+    elif type == "env":
+        if path is None:
+            path = "contrast.env"
+        agent_config.write_agent_config_to_file(path=path, text=rendered_env_text)
 
 
 @scw_integration_app.command("create")
 def scw(profile: str = "default") -> None:
     """
     Populate vulnerability references with Secure Code Warrior links.
     """
-    print("Creating SCW links...")
+    rprint("Creating SCW links...")
     scw_create(profile=profile)
 
 
 @scw_integration_app.command("delete")
 def scw_reset(profile: str = "default") -> None:
     """
     Delete vulnerability references and reset to the original Contrast links.
     """
-    print("Deleting SCW links...")
+    rprint("Deleting SCW links...")
     scw_delete(profile=profile)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `c6t-0.0.6/src/c6t/api/agent_config.py` & `c6t-0.0.7/src/c6t/api/agent_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,14 @@
         response = self.session.post(url)
         if response.status_code == 200:
             return response.text
         else:
             response.raise_for_status()
         return ""
 
-    def write_agent_config_to_file(self, yaml_text: str, path: str) -> None:
+    def write_agent_config_to_file(self, text: str, path: str) -> None:
         """
         Write the Agent Config to the file system
         """
         config_path = Path(path)
         with open(config_path, "w") as f:
-            f.write(yaml_text)
+            f.write(text)
```

### Comparing `c6t-0.0.6/src/c6t/configure/credentials.py` & `c6t-0.0.7/src/c6t/configure/credentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,23 +38,29 @@
     superadmin: bool
 
     def get_credentials_from_file(self, profile: str) -> None:
         """
         Get credentials from file in JSON format
         """
         credentials_file_path = Path("~/.c6t/credentials.json").expanduser()
-        with open(credentials_file_path, "r") as credentials_file:
-            credentials = json.load(credentials_file)
-        self.profile = profile
-        self.base_url = credentials.get(profile).get("url")
-        self.username = credentials.get(profile).get("user_name")
-        self.api_key = credentials.get(profile).get("api_key")
-        self.service_key = credentials.get(profile).get("service_key")
-        self.organization_uuid = credentials.get(profile).get("organization_id")
-        self.superadmin = credentials.get(profile).get("superadmin")
+        try:
+            with open(credentials_file_path, "r") as credentials_file:
+                credentials = json.load(credentials_file)
+            self.profile = profile
+            self.base_url = credentials.get(profile).get("url")
+            self.username = credentials.get(profile).get("user_name")
+            self.api_key = credentials.get(profile).get("api_key")
+            self.service_key = credentials.get(profile).get("service_key")
+            self.organization_uuid = credentials.get(profile).get("organization_id")
+            self.superadmin = credentials.get(profile).get("superadmin")
+        except FileNotFoundError:
+            typer.echo(
+                "Credentials file not found. Please run `c6t login` or `c6t configure`."
+            )
+            raise typer.Abort()  # Exit the program
 
     def write_credentials_to_file(self) -> None:
         """
         Write credentials to file in JSON format
         """
         credentials = {
             self.profile: {
```

### Comparing `c6t-0.0.6/src/c6t/external/integrations/scw/contrast_api.py` & `c6t-0.0.7/src/c6t/external/integrations/scw/contrast_api.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.6/src/c6t/external/integrations/scw/contrast_scw.py` & `c6t-0.0.7/src/c6t/external/integrations/scw/contrast_scw.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.6/src/c6t/ui/auth.py` & `c6t-0.0.7/src/c6t/ui/auth.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.6/.gitignore` & `c6t-0.0.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -165,8 +165,9 @@
 # Mac
 .DS_Store
 
 # Logs
 logs
 
 # Contrast Security
-contrast_security.yaml
+contrast_security.yaml
+*.env
```

### Comparing `c6t-0.0.6/LICENSE` & `c6t-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `c6t-0.0.6/README.md` & `c6t-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 ```shell
 $ c6t configure
 ```
 
 #### Get Agent Configuration File
 This will download the agent configuration file to your local machine.
 ```shell
-$ c6t get-agent-config
+$ c6t agent-config
 ```
```

### Comparing `c6t-0.0.6/pyproject.toml` & `c6t-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "c6t"
-version = "0.0.6"
+version = "0.0.7"
 description = "Unofficial Administrative Command Line Interface for Contrast Security"
 authors = [
     { name = "Jonathan Harper", email = "39912347+jharper-sec@users.noreply.github.com" },
 ]
 dependencies = [
     "requests>=2.32.0",
     "shellingham>=1.5.4",
```

### Comparing `c6t-0.0.6/PKG-INFO` & `c6t-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: c6t
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unofficial Administrative Command Line Interface for Contrast Security
 Project-URL: Homepage, https://github.com/jharper-sec/c6t
 Project-URL: Issues, https://github.com/jharper-sec/c6t/issues
 Project-URL: Documentation, https://github.com/jharper-sec/c6t/blob/main/README.md
 Author-email: Jonathan Harper <39912347+jharper-sec@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -252,9 +252,9 @@
 ```shell
 $ c6t configure
 ```
 
 #### Get Agent Configuration File
 This will download the agent configuration file to your local machine.
 ```shell
-$ c6t get-agent-config
+$ c6t agent-config
 ```
```

