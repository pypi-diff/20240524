# Comparing `tmp/eyeballvul-0.2.0.tar.gz` & `tmp/eyeballvul-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeballvul-0.2.0.tar", max compression
+gzip compressed data, was "eyeballvul-0.3.0.tar", max compression
```

## Comparing `eyeballvul-0.2.0.tar` & `eyeballvul-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-05-13 18:22:34.820247 eyeballvul-0.2.0/LICENSE
--rw-r--r--   0        0        0    23270 2024-05-22 08:35:07.106995 eyeballvul-0.2.0/README.md
--rw-r--r--   0        0        0      685 2024-05-22 08:35:07.106995 eyeballvul-0.2.0/eyeballvul/__init__.py
--rw-r--r--   0        0        0     7447 2024-05-21 13:38:57.247501 eyeballvul-0.2.0/eyeballvul/api.py
--rw-r--r--   0        0        0     2301 2024-05-17 10:05:37.180830 eyeballvul-0.2.0/eyeballvul/cli.py
--rw-r--r--   0        0        0       48 2024-04-24 12:29:04.251010 eyeballvul-0.2.0/eyeballvul/config/__init__.py
--rw-r--r--   0        0        0      710 2024-05-22 08:39:48.617888 eyeballvul-0.2.0/eyeballvul/config/config.toml
--rw-r--r--   0        0        0     1286 2024-05-22 07:52:26.149055 eyeballvul-0.2.0/eyeballvul/config/config_loader.py
--rw-r--r--   0        0        0    23509 2024-05-22 08:21:37.785923 eyeballvul-0.2.0/eyeballvul/converter.py
--rw-r--r--   0        0        0      731 2024-05-15 16:33:53.123068 eyeballvul-0.2.0/eyeballvul/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 09:14:27.186264 eyeballvul-0.2.0/eyeballvul/models/__init__.py
--rw-r--r--   0        0        0     3249 2024-05-15 15:40:32.119299 eyeballvul-0.2.0/eyeballvul/models/cache.py
--rw-r--r--   0        0        0      167 2024-05-13 18:05:00.254883 eyeballvul-0.2.0/eyeballvul/models/common.py
--rw-r--r--   0        0        0     3968 2024-05-17 10:05:11.804390 eyeballvul-0.2.0/eyeballvul/models/eyeballvul.py
--rw-r--r--   0        0        0     4039 2024-05-14 08:38:45.464076 eyeballvul-0.2.0/eyeballvul/models/osv.py
--rw-r--r--   0        0        0        0 2024-05-17 08:30:21.997460 eyeballvul-0.2.0/eyeballvul/py.typed
--rw-r--r--   0        0        0     8681 2024-05-22 08:21:37.785923 eyeballvul-0.2.0/eyeballvul/score.py
--rw-r--r--   0        0        0     6839 2024-05-21 13:35:15.816506 eyeballvul-0.2.0/eyeballvul/util.py
--rw-r--r--   0        0        0     1361 2024-05-22 08:35:07.142996 eyeballvul-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    23952 1970-01-01 00:00:00.000000 eyeballvul-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-13 18:22:34.820247 eyeballvul-0.3.0/LICENSE
+-rw-r--r--   0        0        0    23521 2024-05-24 08:01:01.697510 eyeballvul-0.3.0/README.md
+-rw-r--r--   0        0        0      287 2024-05-24 07:27:29.716177 eyeballvul-0.3.0/eyeballvul/__init__.py
+-rw-r--r--   0        0        0     9338 2024-05-24 07:35:56.581707 eyeballvul-0.3.0/eyeballvul/api.py
+-rw-r--r--   0        0        0     2301 2024-05-17 10:05:37.180830 eyeballvul-0.3.0/eyeballvul/cli.py
+-rw-r--r--   0        0        0       48 2024-04-24 12:29:04.251010 eyeballvul-0.3.0/eyeballvul/config/__init__.py
+-rw-r--r--   0        0        0      710 2024-05-22 08:39:48.617888 eyeballvul-0.3.0/eyeballvul/config/config.toml
+-rw-r--r--   0        0        0     1374 2024-05-24 07:20:46.698632 eyeballvul-0.3.0/eyeballvul/config/config_loader.py
+-rw-r--r--   0        0        0    23509 2024-05-22 08:21:37.785923 eyeballvul-0.3.0/eyeballvul/converter.py
+-rw-r--r--   0        0        0      731 2024-05-15 16:33:53.123068 eyeballvul-0.3.0/eyeballvul/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 09:14:27.186264 eyeballvul-0.3.0/eyeballvul/models/__init__.py
+-rw-r--r--   0        0        0     3249 2024-05-15 15:40:32.119299 eyeballvul-0.3.0/eyeballvul/models/cache.py
+-rw-r--r--   0        0        0      167 2024-05-13 18:05:00.254883 eyeballvul-0.3.0/eyeballvul/models/common.py
+-rw-r--r--   0        0        0     3968 2024-05-17 10:05:11.804390 eyeballvul-0.3.0/eyeballvul/models/eyeballvul.py
+-rw-r--r--   0        0        0     4039 2024-05-14 08:38:45.464076 eyeballvul-0.3.0/eyeballvul/models/osv.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:30:21.997460 eyeballvul-0.3.0/eyeballvul/py.typed
+-rw-r--r--   0        0        0     8681 2024-05-22 08:21:37.785923 eyeballvul-0.3.0/eyeballvul/score.py
+-rw-r--r--   0        0        0     6839 2024-05-21 13:35:15.816506 eyeballvul-0.3.0/eyeballvul/util.py
+-rw-r--r--   0        0        0     1361 2024-05-24 07:38:49.290177 eyeballvul-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    24203 1970-01-01 00:00:00.000000 eyeballvul-0.3.0/PKG-INFO
```

### Comparing `eyeballvul-0.2.0/LICENSE` & `eyeballvul-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/README.md` & `eyeballvul-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,32 @@
+Metadata-Version: 2.1
+Name: eyeballvul
+Version: 0.3.0
+Summary: 
+Author: Timothee Chauvin
+Author-email: timothee.chauvin28@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fire (>=0.6.0,<0.7.0)
+Requires-Dist: litellm (>=1.37.12,<2.0.0)
+Requires-Dist: ortools (>=9.9.3963,<10.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sqlmodel (>=0.0.18,<0.0.19)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: typeguard (>=4.2.1,<5.0.0)
+Description-Content-Type: text/markdown
+
 # eyeballvul
 
-eyeballvul is an open-source benchmark designed to enable the evaluation of [SAST](https://en.wikipedia.org/wiki/Static_application_security_testing) vulnerability detection tools, especially ones based on language models, designed to be future-proof.
+eyeballvul is an open-source benchmark designed to enable the evaluation of [SAST](https://en.wikipedia.org/wiki/Static_application_security_testing) vulnerability detection tools, especially ones based on language models.
 
-While most benchmarks eventually make it into the training data of language models, eyeballvul is designed to be continuously updated from the data source of CVEs in open-source repositories. This means that it will remain relevant as long as models have a reasonably delayed training data cutoff, by evaluating on the subset of the vulnerabilities that were published after the training data cutoff of the considered model. The current goal is to update it weekly.
+While most benchmarks eventually make it into the training data of language models, eyeballvul is designed to be future-proof, as it can be continuously updated from the stream of CVEs in open-source repositories. This means that it will remain relevant as long as models have a reasonably delayed training data cutoff, by evaluating on the subset of the vulnerabilities that were published after the training data cutoff of the considered model. The current goal is to update it weekly.
 
 At a high level, eyeballvul converts the data stream of CVEs in open-source repositories into a small set of commits for each repository, and a set of vulnerabilities present at each of these commits.
 
 The typical use case that this benchmark enables is the following:
 1. select a list of repositories and commits for which there is at least one vulnerability published after some date;
 1. run a SAST tool (typically LLM-based) on the source code at each of these commits;
 1. compare the results of the SAST tool with the list of known vulnerabilities for each commit, especially the ones that were published after the training data cutoff.
@@ -20,17 +40,25 @@
 * [Motivation](#motivation)
 * [How it works](#how-it-works)
 * [Full example](#full-example)
 
 
 ## Installation
 ```bash
-pip install 'git+https://github.com/timothee-chauvin/eyeballvul.git'
+pip install eyeballvul
+```
+
+Then import the data:
+```python
+from eyeballvul import download_data
+download_data()
 ```
 
+(if you want to stick to a particular version of the data, you can use `download_data(date="YYYY-MM-DD")`. See valid dates in the [eyeballvul_data](https://github.com/timothee-chauvin/eyeballvul_data/tags) repo).
+
 ## Data model
 The data can be seen in the `data` directory. There are two kinds of items: **vulnerabilities** and **revisions**. A vulnerability corresponds to an entry in the [osv.dev](https://osv.dev/) database (typically a CVE), and may be present at multiple revisions of the repository. A revision represents the state of a repository at a given commit, and may be associated with multiple vulnerabilities. Let's look at an example of each (commands explained in the [How to use](#how-to-use) section):
 ```python
 >>> from eyeballvul import get_by_project, get_revision
 >>> import json
 >>> vulnerability = get_by_project("https://github.com/gnome/nautilus")[0]
 >>> print(json.dumps(vulnerability.to_dict(), indent=2))
@@ -405,7 +433,8 @@
 >>> recall = tp / (tp + fn)
 >>> recall
 0.5
 >>> f1 = 2 / (1 / precision + 1 / recall)
 >>> f1
 0.6666666666666666
 ```
+
```

### Comparing `eyeballvul-0.2.0/eyeballvul/api.py` & `eyeballvul-0.3.0/eyeballvul/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,57 @@
+import io
+import shutil
+import tarfile
+import tempfile
 from datetime import datetime
 from pathlib import Path
 
+import requests
 from sqlmodel import Session, SQLModel, create_engine, select
 from typeguard import typechecked
 
 from eyeballvul.config.config_loader import Config
 from eyeballvul.models.eyeballvul import EyeballvulItem, EyeballvulRevision
 from eyeballvul.util import str_or_datetime_to_datetime
 
 
+def download_data(date: str | None = None):
+    """
+    Download the data from the eyeballvul_data repository.
+
+    If `date` is provided (format: YYYY-MM-DD), the data at the specific date is downloaded. Otherwise, the latest data is downloaded. See https://github.com/timothee-chauvin/eyeballvul_data/tags for a list of valid dates.
+
+    The data is then extracted into (by default) ~/.cache/eyeballvul/data.
+
+    An SQLite database is instantiated from that data for faster access, in ~/.cache/eyeballvul/db.
+    """
+    if date is None:
+        print("Fetching latest version of the data...")
+        all_tags = requests.get(f"{Config.eyeballvul_data_api}/tags", timeout=30).json()
+        date = all_tags[0]["name"]
+    url = f"{Config.eyeballvul_data_api}/tarball/refs/tags/{date}"
+    print(f"Downloading data from {url}...")
+    response = requests.get(url, timeout=30)
+    if response.status_code != 200:
+        raise ValueError(
+            f"Failed to download the data from {url}. Status code: {response.status_code}"
+        )
+    with tempfile.TemporaryDirectory(prefix=str(Config.paths.workdir)) as tmpdir:
+        tar_file = io.BytesIO(response.content)
+        tar = tarfile.open(fileobj=tar_file)
+        tar_base = tar.getnames()[0].split("/")[0]
+        tar.extractall(path=tmpdir, filter="data")
+        tar.close()
+        shutil.rmtree(Config.paths.data, ignore_errors=True)
+        shutil.move(Path(tmpdir) / tar_base / "data", Config.paths.data)
+    print(f"Successfully downloaded data from {url} to {Config.paths.data}.")
+    print("Initializing the database from the data...")
+    json_import(force=True)
+
+
 @typechecked
 def get_projects() -> list[str]:
     """Get the list of repo URLs."""
     engine = create_engine(f"sqlite:///{Config.paths.db}/eyeballvul.db")
     with Session(engine) as session:
         query = select(EyeballvulItem.repo_url).distinct()
         return list(session.exec(query).all())
@@ -152,21 +191,26 @@
             revision.log()
     print(
         f"Successfully exported {len(eyeballvul_items)} EyeballvulItems and {len(eyeballvul_revisions)} EyeballvulRevisions to {Config.paths.data}."
     )
 
 
 @typechecked
-def json_import(db_dest: Path = Config.paths.db) -> None:
-    """Import the contents of the JSON files in the data directory into the SQL database at
-    `db_dest`."""
+def json_import(db_dest: Path = Config.paths.db, force: bool = False) -> None:
+    """
+    Import the contents of the JSON files in the data directory into the SQL database at `db_dest`.
+
+    If `force` is set to True, the possibly existing database at `db_dest` will be overwritten.
+    """
+    if force:
+        shutil.rmtree(db_dest, ignore_errors=True)
     if db_dest.exists():
         raise ValueError(
             f"The database directory already exists at {db_dest}.\n"
-            "Please remove it or back it up before importing."
+            "Use force=True if you wish to overwrite it."
         )
     db_dest.mkdir(parents=True, exist_ok=True)
     engine = create_engine(f"sqlite:///{db_dest}/eyeballvul.db")
     SQLModel.metadata.create_all(engine)
     with Session(engine) as session:
         eyeballvul_item_files = list(Config.paths.eyeballvul_vulns.glob("*/*/*.json"))
         for path in eyeballvul_item_files:
```

### Comparing `eyeballvul-0.2.0/eyeballvul/cli.py` & `eyeballvul-0.3.0/eyeballvul/cli.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/eyeballvul/config/config.toml` & `eyeballvul-0.3.0/eyeballvul/config/config.toml`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/eyeballvul/config/config_loader.py` & `eyeballvul-0.3.0/eyeballvul/config/config_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,24 +21,25 @@
     workdir: Path
 
 
 class Config:
     ecosystems = config["ecosystems"]
     supported_domains = config["supported_domains"]
     cache_path = Path(config["cache_path"]).expanduser()
-    data_path = PROJECT_DIR / "data"
+    data_path = cache_path / "data"
     scoring_model = config["scoring_model"]
+    eyeballvul_data_api = "https://api.github.com/repos/timothee-chauvin/eyeballvul_data"
 
     paths = Paths(
         project=PROJECT_DIR,
         osv=cache_path / "osv",
         data=data_path,
         eyeballvul_vulns=data_path / "vulns",
         eyeballvul_revisions=data_path / "revisions",
-        db=PROJECT_DIR / "db",
+        db=cache_path / "db",
         repo_info_cache=cache_path / "repo_info",
         workdir=Path(config["workdir"]),
     )
 
 
 no_mkdir = [
     Config.paths.data,
```

### Comparing `eyeballvul-0.2.0/eyeballvul/converter.py` & `eyeballvul-0.3.0/eyeballvul/converter.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/eyeballvul/exceptions.py` & `eyeballvul-0.3.0/eyeballvul/exceptions.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/eyeballvul/models/cache.py` & `eyeballvul-0.3.0/eyeballvul/models/cache.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/eyeballvul/models/eyeballvul.py` & `eyeballvul-0.3.0/eyeballvul/models/eyeballvul.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/eyeballvul/models/osv.py` & `eyeballvul-0.3.0/eyeballvul/models/osv.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/eyeballvul/score.py` & `eyeballvul-0.3.0/eyeballvul/score.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/eyeballvul/util.py` & `eyeballvul-0.3.0/eyeballvul/util.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.2.0/pyproject.toml` & `eyeballvul-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eyeballvul"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Timothee Chauvin <timothee.chauvin28@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "eyeballvul" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `eyeballvul-0.2.0/PKG-INFO` & `eyeballvul-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,12 @@
-Metadata-Version: 2.1
-Name: eyeballvul
-Version: 0.2.0
-Summary: 
-Author: Timothee Chauvin
-Author-email: timothee.chauvin28@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fire (>=0.6.0,<0.7.0)
-Requires-Dist: litellm (>=1.37.12,<2.0.0)
-Requires-Dist: ortools (>=9.9.3963,<10.0.0)
-Requires-Dist: pydantic (>=2.7.1,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: sqlmodel (>=0.0.18,<0.0.19)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: typeguard (>=4.2.1,<5.0.0)
-Description-Content-Type: text/markdown
-
 # eyeballvul
 
-eyeballvul is an open-source benchmark designed to enable the evaluation of [SAST](https://en.wikipedia.org/wiki/Static_application_security_testing) vulnerability detection tools, especially ones based on language models, designed to be future-proof.
+eyeballvul is an open-source benchmark designed to enable the evaluation of [SAST](https://en.wikipedia.org/wiki/Static_application_security_testing) vulnerability detection tools, especially ones based on language models.
 
-While most benchmarks eventually make it into the training data of language models, eyeballvul is designed to be continuously updated from the data source of CVEs in open-source repositories. This means that it will remain relevant as long as models have a reasonably delayed training data cutoff, by evaluating on the subset of the vulnerabilities that were published after the training data cutoff of the considered model. The current goal is to update it weekly.
+While most benchmarks eventually make it into the training data of language models, eyeballvul is designed to be future-proof, as it can be continuously updated from the stream of CVEs in open-source repositories. This means that it will remain relevant as long as models have a reasonably delayed training data cutoff, by evaluating on the subset of the vulnerabilities that were published after the training data cutoff of the considered model. The current goal is to update it weekly.
 
 At a high level, eyeballvul converts the data stream of CVEs in open-source repositories into a small set of commits for each repository, and a set of vulnerabilities present at each of these commits.
 
 The typical use case that this benchmark enables is the following:
 1. select a list of repositories and commits for which there is at least one vulnerability published after some date;
 1. run a SAST tool (typically LLM-based) on the source code at each of these commits;
 1. compare the results of the SAST tool with the list of known vulnerabilities for each commit, especially the ones that were published after the training data cutoff.
@@ -40,17 +20,25 @@
 * [Motivation](#motivation)
 * [How it works](#how-it-works)
 * [Full example](#full-example)
 
 
 ## Installation
 ```bash
-pip install 'git+https://github.com/timothee-chauvin/eyeballvul.git'
+pip install eyeballvul
+```
+
+Then import the data:
+```python
+from eyeballvul import download_data
+download_data()
 ```
 
+(if you want to stick to a particular version of the data, you can use `download_data(date="YYYY-MM-DD")`. See valid dates in the [eyeballvul_data](https://github.com/timothee-chauvin/eyeballvul_data/tags) repo).
+
 ## Data model
 The data can be seen in the `data` directory. There are two kinds of items: **vulnerabilities** and **revisions**. A vulnerability corresponds to an entry in the [osv.dev](https://osv.dev/) database (typically a CVE), and may be present at multiple revisions of the repository. A revision represents the state of a repository at a given commit, and may be associated with multiple vulnerabilities. Let's look at an example of each (commands explained in the [How to use](#how-to-use) section):
 ```python
 >>> from eyeballvul import get_by_project, get_revision
 >>> import json
 >>> vulnerability = get_by_project("https://github.com/gnome/nautilus")[0]
 >>> print(json.dumps(vulnerability.to_dict(), indent=2))
@@ -425,8 +413,7 @@
 >>> recall = tp / (tp + fn)
 >>> recall
 0.5
 >>> f1 = 2 / (1 / precision + 1 / recall)
 >>> f1
 0.6666666666666666
 ```
-
```

