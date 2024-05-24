# Comparing `tmp/burrow_cli-0.1.2.tar.gz` & `tmp/burrow_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burrow_cli-0.1.2.tar", max compression
+gzip compressed data, was "burrow_cli-0.1.3.tar", max compression
```

## Comparing `burrow_cli-0.1.2.tar` & `burrow_cli-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2024-05-24 03:38:27.323179 burrow_cli-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.2/burrow_cli/__init__.py
--rw-r--r--   0        0        0     4114 2024-05-23 15:25:23.423512 burrow_cli-0.1.2/burrow_cli/main.py
--rw-r--r--   0        0        0      602 2024-05-24 03:38:47.739024 burrow_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 burrow_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-24 03:38:27.323179 burrow_cli-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.3/burrow_cli/__init__.py
+-rw-r--r--   0        0        0     4114 2024-05-24 04:54:26.693735 burrow_cli-0.1.3/burrow_cli/main.py
+-rw-r--r--   0        0        0      602 2024-05-24 04:54:40.107436 burrow_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 burrow_cli-0.1.3/PKG-INFO
```

### Comparing `burrow_cli-0.1.2/README.md` & `burrow_cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `burrow_cli-0.1.2/burrow_cli/main.py` & `burrow_cli-0.1.3/burrow_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     pattern = r'^\d+(mi|gi)$'
     if bool(re.match(pattern, gram)):
         # client = docker.DockerClient(base_url='unix://var/run/docker.sock',version='1.45')
         client = docker.from_env()
         typer.echo("Start a shared GPU with GRAM size of {}".format(gram[0:-2]))
         
         env = ["GENV_GPUS={}".format(1),"GENV_GPU_MEMORY={}".format(gram)]
-        # gpu_container = client.containers.run('jyzisgod/python3:latest',detach=True,remove=True,stdout=True,environment=env,runtime='genv',labels={"burrow-cli-container":uuid.uuid4.hex})
-        gpu_container = client.containers.run('jyzisgod/python3:latest',detach=True,remove=True,stdout=True,environment=env,labels={"burrow-cli-container":uuid.uuid4().hex})
+        gpu_container = client.containers.run('jyzisgod/python3:latest',detach=True,remove=True,stdout=True,environment=env,runtime='genv',labels={"burrow-cli-container":uuid.uuid4.hex})
+        # gpu_container = client.containers.run('jyzisgod/python3:latest',detach=True,remove=True,stdout=True,environment=env,labels={"burrow-cli-container":uuid.uuid4().hex})
         f = open('./sh_bin.tar', 'wb')
         with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
     ) as progress:
             progress.add_task(description="Creating GPU fractional container...", total=None)
```

### Comparing `burrow_cli-0.1.2/pyproject.toml` & `burrow_cli-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burrow-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "Burrow command line app, you can launch a fractional GPU contaienr with this app, and share a link of the container to your friends, you and your friends can work colloratively together"
 authors = ["Vurtne Saerdna <vurtnesaerdna@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 burrow = "burrow_cli.main:app"
```

### Comparing `burrow_cli-0.1.2/PKG-INFO` & `burrow_cli-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burrow-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Burrow command line app, you can launch a fractional GPU contaienr with this app, and share a link of the container to your friends, you and your friends can work colloratively together
 Author: Vurtne Saerdna
 Author-email: vurtnesaerdna@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

