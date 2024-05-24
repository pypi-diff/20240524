# Comparing `tmp/burrow_cli-0.1.0.tar.gz` & `tmp/burrow_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burrow_cli-0.1.0.tar", max compression
+gzip compressed data, was "burrow_cli-0.1.2.tar", max compression
```

## Comparing `burrow_cli-0.1.0.tar` & `burrow_cli-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      102 2024-05-23 03:17:22.086937 burrow_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-23 09:23:50.619060 burrow_cli-0.1.0/burrow_cli/__init__.py
--rw-r--r--   0        0        0     3113 2024-05-23 09:23:47.851904 burrow_cli-0.1.0/burrow_cli/main.py
--rw-r--r--   0        0        0      440 2024-05-23 13:16:21.721994 burrow_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 burrow_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-24 03:38:27.323179 burrow_cli-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.2/burrow_cli/__init__.py
+-rw-r--r--   0        0        0     4114 2024-05-23 15:25:23.423512 burrow_cli-0.1.2/burrow_cli/main.py
+-rw-r--r--   0        0        0      602 2024-05-24 03:38:47.739024 burrow_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 burrow_cli-0.1.2/PKG-INFO
```

### Comparing `burrow_cli-0.1.0/burrow_cli/main.py` & `burrow_cli-0.1.2/burrow_cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from rich import print
 from typing_extensions import Annotated
 import re
 import docker
 import tarfile
 import os
 import time
+import uuid
+from rich.progress import Progress, SpinnerColumn, TextColumn
 
 app = typer.Typer()
 
 def print_file_content(file_path):
     try:
         with open(file_path, 'r') as file:
             content = file.read()
-            print(content)
+            return content
     except FileNotFoundError:
         print(f"Error: The file at '{file_path}' was not found.")
     except IOError as e:
         print(f"Error: An I/O error occurred while accessing the file: {e}")
 
 def untar_and_list_files(tar_path, extract_path='.'):
     """
@@ -56,35 +58,55 @@
     Start a shared GPU container with a user set memory size
     """
     pattern = r'^\d+(mi|gi)$'
     if bool(re.match(pattern, gram)):
         # client = docker.DockerClient(base_url='unix://var/run/docker.sock',version='1.45')
         client = docker.from_env()
         typer.echo("Start a shared GPU with GRAM size of {}".format(gram[0:-2]))
-        name = "shared_gpu_1"
+        
         env = ["GENV_GPUS={}".format(1),"GENV_GPU_MEMORY={}".format(gram)]
-        file_name = 'server.txt'
-        # client.containers.run('jyzisgod/python3:latest','sshx -q > {}.txt'.format(file_name),detach=True,remove=True,stdout=True,name=name,environment=env,runtime='genv')
-        gpu_container = client.containers.run('jyzisgod/python3:latest',detach=True,remove=True,stdout=True,name=name)
+        # gpu_container = client.containers.run('jyzisgod/python3:latest',detach=True,remove=True,stdout=True,environment=env,runtime='genv',labels={"burrow-cli-container":uuid.uuid4.hex})
+        gpu_container = client.containers.run('jyzisgod/python3:latest',detach=True,remove=True,stdout=True,environment=env,labels={"burrow-cli-container":uuid.uuid4().hex})
         f = open('./sh_bin.tar', 'wb')
-        time.sleep(10)
+        with Progress(
+        SpinnerColumn(),
+        TextColumn("[progress.description]{task.description}"),
+        transient=True,
+    ) as progress:
+            progress.add_task(description="Creating GPU fractional container...", total=None)
+            time.sleep(5)
+        
         bits, stat = gpu_container.get_archive('/workspace/server.txt')
-        print(stat)
-        print(type(bits))
+        # print(stat)
+        # print(type(bits))
         for chunk in bits:
             f.write(chunk)
         f.close()
         untar_and_list_files('./sh_bin.tar')
-        print_file_content('./server.txt')
+        sshx_url = print_file_content('./server.txt')
+        print("[bold green]GPU fractional container created successfully![/bold green]")
+        print('Now you can send this link [bold blue]{}[/bold blue] to your friends, and start sharing GPU 🚀💻✨'.format(sshx_url))
     else:
         typer.echo("Wrong memory size format, size should be like 512mi or 2gi")
 
 
-@app.command()
+@app.command(name='stop')
 def stop(container_id: Annotated[str, typer.Argument(help="stop a container with container_id")]):
     """
     Stop a running container
     """
     client = docker.DockerClient(base_url='unix://var/run/docker.sock')
     gpu_container = client.containers.get(container_id=container_id)
     stop_result = gpu_container.stop()
-    typer.echo("Stop the container {}".format(stop_result))
+    typer.echo("Stop the container {}".format(stop_result))
+
+@app.command(name='list')
+def show_container():
+    """
+    List all running container started using burrow
+    """
+    client = docker.DockerClient(base_url='unix://var/run/docker.sock')
+    container_list = client.containers.list(filters={ "label":'burrow-cli-container'})
+    if len(container_list)==0:
+        print("No burrow container is running")
+    else:
+        print(container_list)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

