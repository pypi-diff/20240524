# Comparing `tmp/gunshotmatch_cli-0.8.0.tar.gz` & `tmp/gunshotmatch_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunshotmatch_cli-0.8.0.tar", last modified: Wed Mar 27 15:42:14 2024, max compression
+gzip compressed data, was "gunshotmatch_cli-0.9.0.tar", last modified: Fri May 24 10:38:42 2024, max compression
```

## Comparing `gunshotmatch_cli-0.8.0.tar` & `gunshotmatch_cli-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-27 15:42:14.680218 gunshotmatch_cli-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-27 15:42:14.676218 gunshotmatch_cli-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-27 15:42:14.680218 gunshotmatch_cli-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-27 15:42:14.680218 gunshotmatch_cli-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-03-27 15:42:14.680218 gunshotmatch_cli-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-03-27 15:41:45.895778 gunshotmatch_cli-0.8.0/gunshotmatch_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-03-27 15:41:45.895778 gunshotmatch_cli-0.8.0/gunshotmatch_cli/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:45.895778 gunshotmatch_cli-0.8.0/gunshotmatch_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-27 15:41:45.895778 gunshotmatch_cli-0.8.0/gunshotmatch_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-24 10:38:42.684913 gunshotmatch_cli-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-24 10:38:42.684913 gunshotmatch_cli-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-24 10:38:42.684913 gunshotmatch_cli-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-24 10:38:42.684913 gunshotmatch_cli-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-24 10:38:42.680914 gunshotmatch_cli-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-24 10:38:17.540903 gunshotmatch_cli-0.9.0/gunshotmatch_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-24 10:38:17.540903 gunshotmatch_cli-0.9.0/gunshotmatch_cli/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-24 10:38:17.540903 gunshotmatch_cli-0.9.0/gunshotmatch_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:38:17.540903 gunshotmatch_cli-0.9.0/gunshotmatch_cli/py.typed
```

### Comparing `gunshotmatch_cli-0.8.0/README.rst` & `gunshotmatch_cli-0.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-cli
 	:target: https://github.com/GunShotMatch/gunshotmatch-cli/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-cli
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-cli/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-cli/v0.9.0
 	:target: https://github.com/GunShotMatch/gunshotmatch-cli/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-cli
 	:target: https://github.com/GunShotMatch/gunshotmatch-cli/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_cli-0.8.0/LICENSE` & `gunshotmatch_cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gunshotmatch_cli-0.8.0/pyproject.toml` & `gunshotmatch_cli-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "gunshotmatch-cli"
-version = "0.8.0"
+version = "0.9.0"
 description = "GunShotMatch Command-Line Interface."
 readme = "README.rst"
 keywords = []
 dynamic = []
 dependencies = [
     "click>=8.1.7",
     "consolekit>=1.5.2",
     "domdf-python-tools>=3.6.1",
     "gunshotmatch-pipeline>=0.8.1",
     "gunshotmatch-reports>=0.1.0",
-    "libgunshotmatch>=0.4.0",
+    "libgunshotmatch>=0.12.0",
     "libgunshotmatch-mpl>=0.1.0.post1",
     "numpy>=1.22",
     "scikit-learn>=1.3.2",
+    "sdjson>=0.4.0",
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
@@ -31,22 +32,21 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 
+[project.license]
+file = "LICENSE"
+
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
-
-[project.license]
-file = "LICENSE"
-
 [project.urls]
 Homepage = "https://github.com/GunShotMatch/gunshotmatch-cli"
 "Issue Tracker" = "https://github.com/GunShotMatch/gunshotmatch-cli/issues"
 "Source Code" = "https://github.com/GunShotMatch/gunshotmatch-cli"
 
 [project.scripts]
 gunshotmatch-cli = "gunshotmatch_cli.__main__:main"
@@ -69,24 +69,24 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
-[tool.dependency-dash."requirements.txt"]
-order = 10
-
-[tool.dep_checker.name_mapping]
-attrs = "attr"
-pymassspec = "pyms"
-scikit-learn = "sklearn"
-
 [tool.snippet-fmt.languages.python]
 reformat = true
 
 [tool.snippet-fmt.languages.TOML]
 reformat = true
 
 [tool.snippet-fmt.languages.ini]
 
 [tool.snippet-fmt.languages.json]
+
+[tool.dependency-dash."requirements.txt"]
+order = 10
+
+[tool.dep_checker.name_mapping]
+attrs = "attr"
+pymassspec = "pyms"
+scikit-learn = "sklearn"
```

### Comparing `gunshotmatch_cli-0.8.0/PKG-INFO` & `gunshotmatch_cli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.2
 Name: gunshotmatch-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: GunShotMatch Command-Line Interface.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Home-page: https://github.com/GunShotMatch/gunshotmatch-cli
 Project-URL: Issue Tracker, https://github.com/GunShotMatch/gunshotmatch-cli/issues
 Project-URL: Source Code, https://github.com/GunShotMatch/gunshotmatch-cli
 Platform: Windows
@@ -23,18 +23,19 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: click>=8.1.7
 Requires-Dist: consolekit>=1.5.2
 Requires-Dist: domdf-python-tools>=3.6.1
 Requires-Dist: gunshotmatch-pipeline>=0.8.1
 Requires-Dist: gunshotmatch-reports>=0.1.0
-Requires-Dist: libgunshotmatch>=0.4.0
+Requires-Dist: libgunshotmatch>=0.12.0
 Requires-Dist: libgunshotmatch-mpl>=0.1.0.post1
 Requires-Dist: numpy>=1.22
 Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: sdjson>=0.4.0
 Description-Content-Type: text/x-rst
 
 
 =================
 gunshotmatch-cli
 =================
 
@@ -109,15 +110,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-cli
 	:target: https://github.com/GunShotMatch/gunshotmatch-cli/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-cli
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-cli/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-cli/v0.9.0
 	:target: https://github.com/GunShotMatch/gunshotmatch-cli/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-cli
 	:target: https://github.com/GunShotMatch/gunshotmatch-cli/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_cli-0.8.0/gunshotmatch_cli/__main__.py` & `gunshotmatch_cli-0.9.0/gunshotmatch_cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,19 +96,21 @@
 @main.command()
 def projects(projects_toml: str = "projects.toml") -> None:
 	"""
 	Pipeline for creating projects from raw datafiles.
 	"""
 
 	# 3rd party
+	import gunshotmatch_pipeline.results
+	import sdjson
 	from domdf_python_tools.paths import PathPlus
-	from gunshotmatch_pipeline.exporters import verify_saved_project, write_combined_csv, write_matches_json
+	from gunshotmatch_pipeline.exporters import verify_saved_project, write_combined_csv
 	from gunshotmatch_pipeline.projects import Projects, process_projects
 	from gunshotmatch_pipeline.utils import project_plural
-	from libgunshotmatch.peak import write_alignment
+	from libgunshotmatch.peak import write_project_alignment
 	from libgunshotmatch.project import Project
 
 	projects = Projects.from_toml(PathPlus(projects_toml).read_text())
 	output_dir = PathPlus(projects.global_settings.output_directory).abspath()
 
 	print(f"Processing {len(projects)} {project_plural(len(projects))}:")
 	for project_name in projects.per_project_settings:
@@ -123,24 +125,41 @@
 		# 	datafile = repeat.datafile
 
 		# 	verify_saved_file = False
 		# 	if verify_saved_file:
 		# 		from_file = Datafile.from_file(datafile_export_filename)
 		# 		verify_saved_datafile(datafile, from_file)
 
-		write_alignment(project.alignment, project.name, output_dir)
+		write_project_alignment(project, output_dir)
 		for repeat in project.datafile_data.values():
 			write_combined_csv(repeat, output_dir)
 
 		# Matches Sheet
 		# MatchesCSVExporter(
 		# 		os.path.join(output_dir, project.name + "_MATCHES.csv"), project, minutes=True, n_hits=5
 		# 		)
 
-		write_matches_json(project, output_dir)
+		write_new_output = True
+		matches_json_filename = f"{project.name}.json"
+		matches_data = gunshotmatch_pipeline.results.matches(project)
+
+		if (output_dir / matches_json_filename).is_file():
+			existing_file_content = (output_dir / matches_json_filename).read_text().strip()
+			existing_matches_json = sdjson.loads(existing_file_content)
+			matches_data_with_old_mtime: Dict[str, Dict[str, Any]] = {
+					"metadata": dict(matches_data["metadata"]),
+					"compounds": matches_data["compounds"],
+					}
+			matches_data_with_old_mtime["metadata"]["created"] = existing_matches_json["metadata"]["created"]
+			if sdjson.dumps(matches_data_with_old_mtime, indent=2).strip() == existing_file_content:
+				# Unchanged
+				write_new_output = False
+
+		if write_new_output:
+			(output_dir / matches_json_filename).write_clean(sdjson.dumps(matches_data, indent=2))
 
 		assert project.consolidated_peaks is not None
 		print(project.consolidated_peaks)
 		print(len(project.consolidated_peaks))
 
 
 @click.argument("unknown_toml", default="unknown.toml")
```

### Comparing `gunshotmatch_cli-0.8.0/gunshotmatch_cli/decision_tree.py` & `gunshotmatch_cli-0.9.0/gunshotmatch_cli/decision_tree.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_cli-0.8.0/gunshotmatch_cli/__init__.py` & `gunshotmatch_cli-0.9.0/gunshotmatch_cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2023 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.8.0"
+__version__: str = "0.9.0"
 __email__: str = "dominic@davis-foster.co.uk"
```

