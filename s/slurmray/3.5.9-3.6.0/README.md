# Comparing `tmp/slurmray-3.5.9.tar.gz` & `tmp/slurmray-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmray-3.5.9.tar", max compression
+gzip compressed data, was "slurmray-3.6.0.tar", max compression
```

## Comparing `slurmray-3.5.9.tar` & `slurmray-3.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-11-03 09:04:55.530868 slurmray-3.5.9/LICENSE
--rw-r--r--   0        0        0     2591 2024-05-22 08:54:20.413962 slurmray-3.5.9/README.md
--rw-r--r--   0        0        0      751 2024-05-22 09:01:26.563863 slurmray-3.5.9/pyproject.toml
--rw-r--r--   0        0        0    22617 2024-05-22 08:54:20.413962 slurmray-3.5.9/slurmray/RayLauncher.py
--rw-r--r--   0        0        0        0 2023-11-03 09:04:55.530868 slurmray-3.5.9/slurmray/__init__.py
--rw-r--r--   0        0        0     2273 2023-11-03 09:04:55.530868 slurmray-3.5.9/slurmray/assets/sbatch_template.sh
--rw-r--r--   0        0        0      638 2023-12-11 23:26:19.853300 slurmray-3.5.9/slurmray/assets/slurmray_server.sh
--rw-r--r--   0        0        0      575 2024-05-22 08:54:20.413962 slurmray-3.5.9/slurmray/assets/slurmray_server_template.py
--rw-r--r--   0        0        0      597 2023-12-05 14:46:52.657175 slurmray-3.5.9/slurmray/assets/spython_template.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 slurmray-3.5.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-03 09:04:55.530868 slurmray-3.6.0/LICENSE
+-rw-r--r--   0        0        0     2572 2024-05-24 09:50:27.907919 slurmray-3.6.0/README.md
+-rw-r--r--   0        0        0      751 2024-05-24 10:15:08.917595 slurmray-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0    23279 2024-05-24 10:45:39.077195 slurmray-3.6.0/slurmray/RayLauncher.py
+-rw-r--r--   0        0        0        0 2023-11-03 09:04:55.530868 slurmray-3.6.0/slurmray/__init__.py
+-rw-r--r--   0        0        0     2273 2023-11-03 09:04:55.530868 slurmray-3.6.0/slurmray/assets/sbatch_template.sh
+-rw-r--r--   0        0        0     1506 2024-05-24 10:21:10.257516 slurmray-3.6.0/slurmray/assets/slurmray_server.sh
+-rw-r--r--   0        0        0      446 2024-05-24 10:40:31.647263 slurmray-3.6.0/slurmray/assets/slurmray_server_template.py
+-rw-r--r--   0        0        0      597 2023-12-05 14:46:52.657175 slurmray-3.6.0/slurmray/assets/spython_template.py
+-rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 slurmray-3.6.0/PKG-INFO
```

### Comparing `slurmray-3.5.9/LICENSE` & `slurmray-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.9/README.md` & `slurmray-3.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SLURM_RAY
 
-👉[Full documentation](https://henri-jamet.vercel.app/cards/documentation/slurm-ray/slurm-ray/)
+👉[Full documentation](https://www.henri-jamet.com/docs/slurmray/slurm-ray/)
 
 ## Description
 
 **SlurmRay** is a module for effortlessly distributing tasks on a [Slurm](https://slurm.schedmd.com/) cluster using the [Ray](https://ray.io/) library. **SlurmRay** was initially designed to work with the [Curnagl](https://wiki.unil.ch/ci/books/high-performance-computing-hpc/page/curnagl) cluster at the *University of Lausanne*. However, it should be able to run on any [Slurm](https://slurm.schedmd.com/) cluster with a minimum of configuration.
 
 ## Installation
```

### Comparing `slurmray-3.5.9/pyproject.toml` & `slurmray-3.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slurmray"
-version = "3.5.9"
+version = "3.6.0"
 description = "SlurmRay is a module for effortlessly distributing tasks on a Slurm cluster using the Ray library. "
 authors = ["Henri Jamet <henri.jamet@unil.ch>"]
 license = "Apache License"
 homepage = "https://henri-jamet.vercel.app/"
 documentation = "https://henri-jamet.vercel.app/cards/documentation/slurm-ray/slurm-ray/"
 readme = "README.md"
```

### Comparing `slurmray-3.5.9/slurmray/RayLauncher.py` & `slurmray-3.6.0/slurmray/RayLauncher.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,18 +164,20 @@
 
         Args:
             func (Callable, optional): Function to serialize. Defaults to None.
             args (list, optional): Arguments of the function. Defaults to None.
         """
         print("Serializing function and arguments...")
 
-        # Remove the old python script
-        for file in os.listdir(self.project_path):
-            if file.endswith(".pkl"):
-                os.remove(os.path.join(self.project_path, file))
+        # Check if there is already a func.pkl and args.pkl file
+        if os.path.exists(
+            os.path.join(self.project_path, "func.pkl")
+        ) and os.path.exists(os.path.join(self.project_path, "args.pkl")):
+            print("Function and arguments already serialized.")
+            return
 
         # Pickle the function
         with open(os.path.join(self.project_path, "func.pkl"), "wb") as f:
             dill.dump(func, f)
 
         # Pickle the arguments
         if args is None:
@@ -295,17 +297,15 @@
                 os.path.join(self.project_path, script_file),
                 os.path.join(self.project_path, "{}.log".format(job_name)),
             )
         )
 
         # Wait for log file to be created
         current_queue = None
-        queue_log_file = os.path.join(
-            self.project_path, "{}_queue.log".format(job_name)
-        )
+        queue_log_file = os.path.join(self.project_path, "queue.log")
         with open(queue_log_file, "w") as f:
             f.write("")
         print(
             "Start to monitor the queue... You can check the queue at: <{}>".format(
                 queue_log_file
             )
         )
@@ -369,15 +369,19 @@
                         for user, status, nodes, node_list in current_queue:
                             text += (
                                 format_row.format(user, status, nodes, node_list) + "\n"
                             )
                         text += "\n"
                         f.write(text)
 
+                        # Print the queue
+                        print(text)
+
         # Wait for the job to finish while printing the log
+        print("Job started! Waiting for the job to finish...")
         log_cursor_position = 0
         job_finished = False
         while not job_finished:
             time.sleep(0.25)
             if os.path.exists(os.path.join(self.project_path, "result.pkl")):
                 job_finished = True
             else:
@@ -403,15 +407,15 @@
         ssh_client = paramiko.SSHClient()
         ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
         while not connected:
             try:
                 if self.server_password is None:
                     # Add ssh key
                     self.server_password = getpass("Enter your cluster password: ")
-                
+
                 ssh_client.connect(
                     hostname=self.server_ssh,
                     username=self.server_username,
                     password=self.server_password,
                 )
                 sftp = ssh_client.open_sftp()
                 connected = True
@@ -436,19 +440,20 @@
             # lines = [re.sub(r"torch\n", "torch==2.0.1\n", line) for line in lines]
             # lines = [re.sub(r'torchvision\n', 'torchvision --pre --index-url https://download.pytorch.org/whl/nightly/cu121\n', line) for line in lines]
             # lines = [re.sub(r'torchaudio\n', 'torchaudio --pre --index-url https://download.pytorch.org/whl/nightly/cu121\n', line) for line in lines]
 
             # lines = [re.sub(r'bitsandbytes\n', 'bitsandbytes --global-option="--cuda_ext"\n', line) for line in lines]
             lines = [re.sub(r"slurmray\n", "", line) for line in lines]
             # Add slurmray --pre
-            lines.append("slurmray --pre\n")
+            lines.append("slurmray --pre \n")
             # Solve torch buf (https://github.com/pytorch/pytorch/issues/111469)
             if "torchaudio\n" or "torchvision\n" in lines:
-                lines.append("torch==2.1.1\n")
-                lines.append("--index-url https://download.pytorch.org/whl/cu121\n")
+                lines.append(
+                    "torch==2.1.1 --index-url https://download.pytorch.org/whl/cu121\n"
+                )
 
         with open(f"{self.project_path}/requirements.txt", "w") as file:
             file.writelines(lines)
 
         # Copy files from the project to the server
         for file in os.listdir(self.project_path):
             if file.endswith(".py") or file.endswith(".pkl") or file.endswith(".sh"):
@@ -480,21 +485,32 @@
         # Read the output in real time
         while True:
             line = stdout.readline()
             if not line:
                 break
             print(line, end="")
 
+        stdout.channel.recv_exit_status()
+
         # Downloading result
         print("Downloading result...")
-        sftp.get(
-            "slurmray-server/.slogs/server/result.pkl",
-            os.path.join(self.project_path, "result.pkl"),
-        )
-        print("Result downloaded!")
+        try:
+            sftp.get(
+                "slurmray-server/.slogs/server/result.pkl",
+                os.path.join(self.project_path, "result.pkl"),
+            )
+            print("Result downloaded!")
+        except FileNotFoundError:
+            # Check for errors
+            stderr_lines = stderr.readlines()
+            if stderr_lines:
+                print("\nErrors:\n")
+                for line in stderr_lines:
+                    print(line, end="")
+                print("An error occured, please check the logs.")
 
     def __write_server_script(self):
         """This funtion will write a script with the given specifications to run slurmray on the cluster"""
         print("Writing slurmray server script...")
         template_file = os.path.join(
             self.module_path, "assets", "slurmray_server_template.py"
         )
@@ -537,25 +553,29 @@
             f"GPU is available : {torch.cuda.is_available()}",
             x + 1,
             function_inside_function(),
         )
         return result
 
     launcher = RayLauncher(
-        project_name="example", # Name of the project (will create a directory with this name in the current directory)
-        func=example_func, # Function to execute
-        args={"x": 1}, # Arguments of the function
-        files=["slurmray/RayLauncher.py"], # List of files to push to the cluster (file path will be recreated on the cluster)
-        modules=[], # List of modules to load on the curnagl Cluster (CUDA & CUDNN are automatically added if use_gpu=True)
-        node_nbr=1, # Number of nodes to use
-        use_gpu=True, # If you need A100 GPU, you can set it to True
-        memory=8, # In MegaBytes
-        max_running_time=5, # In minutes
-        runtime_env={"env_vars": {"NCCL_SOCKET_IFNAME": "eno1"}}, # Example of environment variable
-        server_run=True, # To run the code on the cluster and not locally
-        server_ssh="curnagl.dcsr.unil.ch", # Address of the SLURM server
-        server_username="hjamet", # Username to connect to the server
-        server_password=None, # Will be asked in the terminal
+        project_name="example",  # Name of the project (will create a directory with this name in the current directory)
+        func=example_func,  # Function to execute
+        args={"x": 1},  # Arguments of the function
+        files=[
+            "slurmray/RayLauncher.py"
+        ],  # List of files to push to the cluster (file path will be recreated on the cluster)
+        modules=[],  # List of modules to load on the curnagl Cluster (CUDA & CUDNN are automatically added if use_gpu=True)
+        node_nbr=1,  # Number of nodes to use
+        use_gpu=False,  # If you need A100 GPU, you can set it to True
+        memory=8,  # In MegaBytes
+        max_running_time=5,  # In minutes
+        runtime_env={
+            "env_vars": {"NCCL_SOCKET_IFNAME": "eno1"}
+        },  # Example of environment variable
+        server_run=True,  # To run the code on the cluster and not locally
+        server_ssh="curnagl.dcsr.unil.ch",  # Address of the SLURM server
+        server_username="hjamet",  # Username to connect to the server
+        server_password=None,  # Will be asked in the terminal
     )
 
     result = launcher()
     print(result)
```

### Comparing `slurmray-3.5.9/slurmray/assets/sbatch_template.sh` & `slurmray-3.6.0/slurmray/assets/sbatch_template.sh`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.9/slurmray/assets/spython_template.py` & `slurmray-3.6.0/slurmray/assets/spython_template.py`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.9/PKG-INFO` & `slurmray-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmray
-Version: 3.5.9
+Version: 3.6.0
 Summary: SlurmRay is a module for effortlessly distributing tasks on a Slurm cluster using the Ray library. 
 Home-page: https://henri-jamet.vercel.app/
 License: Apache License
 Author: Henri Jamet
 Author-email: henri.jamet@unil.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -19,15 +19,15 @@
 Requires-Dist: ray[data,serve,train,tune] (>=2.7.1,<3.0.0)
 Requires-Dist: torch (>=2.1.1,<3.0.0)
 Project-URL: Documentation, https://henri-jamet.vercel.app/cards/documentation/slurm-ray/slurm-ray/
 Description-Content-Type: text/markdown
 
 # SLURM_RAY
 
-👉[Full documentation](https://henri-jamet.vercel.app/cards/documentation/slurm-ray/slurm-ray/)
+👉[Full documentation](https://www.henri-jamet.com/docs/slurmray/slurm-ray/)
 
 ## Description
 
 **SlurmRay** is a module for effortlessly distributing tasks on a [Slurm](https://slurm.schedmd.com/) cluster using the [Ray](https://ray.io/) library. **SlurmRay** was initially designed to work with the [Curnagl](https://wiki.unil.ch/ci/books/high-performance-computing-hpc/page/curnagl) cluster at the *University of Lausanne*. However, it should be able to run on any [Slurm](https://slurm.schedmd.com/) cluster with a minimum of configuration.
 
 ## Installation
```

