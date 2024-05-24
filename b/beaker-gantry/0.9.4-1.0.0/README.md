# Comparing `tmp/beaker-gantry-0.9.4.tar.gz` & `tmp/beaker_gantry-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaker-gantry-0.9.4.tar", last modified: Tue Mar  7 21:03:06 2023, max compression
+gzip compressed data, was "beaker_gantry-1.0.0.tar", last modified: Fri May 24 17:48:50 2024, max compression
```

## Comparing `beaker-gantry-0.9.4.tar` & `beaker_gantry-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/beaker_gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/gantry/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/common/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/common/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:48:50.064303 beaker_gantry-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-24 17:48:50.064303 beaker_gantry-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:48:50.060303 beaker_gantry-1.0.0/beaker_gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-24 17:48:50.000000 beaker_gantry-1.0.0/beaker_gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-24 17:48:50.000000 beaker_gantry-1.0.0/beaker_gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:48:50.000000 beaker_gantry-1.0.0/beaker_gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 17:48:50.000000 beaker_gantry-1.0.0/beaker_gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 17:48:50.000000 beaker_gantry-1.0.0/beaker_gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 17:48:50.000000 beaker_gantry-1.0.0/beaker_gantry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:48:50.060303 beaker_gantry-1.0.0/gantry/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:48:50.060303 beaker_gantry-1.0.0/gantry/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/commands/follow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/commands/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/gantry/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-24 17:48:27.000000 beaker_gantry-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:48:50.064303 beaker_gantry-1.0.0/setup.cfg
```

### Comparing `beaker-gantry-0.9.4/LICENSE` & `beaker_gantry-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beaker-gantry-0.9.4/PKG-INFO` & `beaker_gantry-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,10 @@
-Metadata-Version: 2.1
-Name: beaker-gantry
-Version: 0.9.4
-Home-page: https://github.com/allenai/beaker-gantry
-Author: Allen Institute for Artificial Intelligence
-Author-email: contact@allenai.org
-License: Apache
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
-<!-- TODO: Add logo -->
 <br>
-<img src="https://raw.githubusercontent.com/allenai/beaker-gantry/main/.github/gantry-logo-ascii.png"/>
+<img src="https://raw.githubusercontent.com/allenai/beaker-py/main/docs/source/_static/beaker-500px-transparent.png" width="200"/>
 <br>
 <h1>Beaker Gantry</h1>
 <p>Gantry streamlines running Python experiments in <a href="https://beaker.org">Beaker</a> by managing containers and boilerplate for you</p>
 <hr/>
 <!-- TODO: Add badges once this is open source -->
 <a href="https://github.com/allenai/beaker-gantry/actions">
     <img alt="CI" src="https://github.com/allenai/beaker-gantry/workflows/Main/badge.svg?event=push&branch=main">
@@ -128,15 +110,15 @@
 
 2. **Configure Gantry.**
 
     If you've already configured the [Beaker command-line client](https://github.com/allenai/beaker/), Gantry will 
     find and use the existing configuration file (usually located at `$HOME/.beaker/config.yml`).
     Otherwise just set the environment variable `BEAKER_TOKEN` to your Beaker [user token](https://beaker.org/user).
 
-    The first time you call `gantry run ...` you'll also be prompted to provide a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) with the `repo` scope. This allows Gantry to clone your private repository when it runs in Beaker. You don't have to do this just yet (Gantry will prompt you for it), but if you need to update this token later you can use the `gantry config set-gh-token` command.
+    The first time you call `gantry run ...` you'll also be prompted to provide a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) with the `repo` scope if your repository is not public. This allows Gantry to clone your private repository when it runs in Beaker. You don't have to do this just yet (Gantry will prompt you for it), but if you need to update this token later you can use the `gantry config set-gh-token` command.
 
 3. **Specify your Python environment.**
 
     Lastly - and this is the most important part - you'll have to create one of several different files that specify your Python environment. There are three options:
 
     1. A conda [`environment.yml`](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#create-env-file-manually) file.
     2. A [`setup.py`](https://docs.python.org/3/distutils/introduction.html#a-simple-example) file.
@@ -153,25 +135,25 @@
 First make sure you've committed *and* pushed all changes so far in your repository.
 Then (from the root of your repository) run:
 
 ```bash
 gantry run --workspace {WORKSPACE} --cluster {CLUSTER} -- python -c 'print("Hello, World!")'
 ```
 
-Just replace `{WORKSPACE}` with the name of your own Beaker [*private*](#use-your-own-private-beaker-workspace) workspace and `{CLUSTER}` with the name of the Beaker cluster you want to run on.
+Just replace `{WORKSPACE}` with the name of your own Beaker [*non-public*](#use-your-own-non-public-beaker-workspace) workspace and `{CLUSTER}` with the name of the Beaker cluster you want to run on.
 
 *❗Note: Everything after the `--` is the command + arguments you want to run on Beaker. It's necessary to include the `--` if any of your arguments look like options themselves (like `-c` in this example) so gantry can differentiate them from its own options.*
 
 Try `gantry run --help` to see all of the available options.
 
 ## Best practices
 
-### Use your own private Beaker workspace
+### Use your own non-public Beaker workspace
 
-Any authorized contributors to your workspace will have access to the secrets in your workspace, and Gantry needs to store your GitHub personal access token (PAT) as a secret in the workspace.
+Any authorized contributors to your workspace will have access to the secrets in your workspace, and Gantry needs to store your GitHub personal access token (PAT) as a secret in the workspace (for non-public repos).
 That's also why it's important to [limit the scope and lifetime of your GitHub token](#limit-the-scope-and-lifetime-of-your-github-token).
 
 ### Limit the scope and lifetime of your GitHub token
 
 Your PAT only needs to have the `repo` scope and should have a short expiration time (e.g. 30 days).
 This limits the harm a bad actor could cause if they were able to read your PAT from your Beaker workspace somehow.
 
@@ -191,15 +173,15 @@
 
 ## FAQ
 
 ### Can I use my own Docker/Beaker image?
 
 You sure can! Just set the `--beaker-image` or `--docker-image` flag.
 
-Gantry can use any image that has bash and conda installed. This can be useful when you have dependencies that take a long time to download and build (like PyTorch).
+Gantry can use any image that has bash installed. This can be useful when you have dependencies that take a long time to download and build (like PyTorch).
 
 In this case it works best if you build your image with a conda environment that already has your big dependencies installed. Then when you call `gantry run`, use the `--venv` option to tell Gantry to use that environment instead of creating a new conda environment in the container. You may also want to add a `requirements.txt` file to your repository that lists all of your dependencies (including PyTorch and anything else already installed in your image's conda environment) so Gantry can make sure the environment on the image is up-to-date when it runs.
 
 For example, you could use one of our [pre-built PyTorch images](https://beaker.org/ws/ai2/fab/images?text=pytorch&sort=created:descending), such as [`ai2/pytorch1.11.0-cuda11.3-python3.9`](https://beaker.org/im/01G3S1CBQ0K832MCFDA77XQXFJ/details), like this:
 
 ```bash
 gantry run \
@@ -285,10 +267,14 @@
 
 Just use the `--dataset` option for `gantry run`. For example:
 
 ```bash
 gantry run --dataset 'petew/squad-train:/input-data' -- ls /input-data
 ```
 
+### How can I run distributed batch jobs with Gantry?
+
+The three options `--replicas` (int), `--leader-selection` (flag), and `--host-networking` (flag) used together give you the ability to run distributed batch jobs. See the [Beaker docs](https://beaker-docs.apps.allenai.org/distributed-training.html#batch-jobs) for more information.
+
 ### Why "Gantry"?
 
 A gantry is a structure that's used, among other things, to lift containers off of ships. Analogously Beaker Gantry's purpose is to lift Docker containers (or at least the *management* of Docker containers) away from users.
```

#### html2text {}

```diff
@@ -1,19 +1,10 @@
-Metadata-Version: 2.1 Name: beaker-gantry Version: 0.9.4 Home-page: https://
-github.com/allenai/beaker-gantry Author: Allen Institute for Artificial
-Intelligence Author-email: contact@allenai.org License: Apache Classifier:
-Intended Audience :: Science/Research Classifier: Development Status :: 3 -
-Alpha Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE
 
- [https://raw.githubusercontent.com/allenai/beaker-gantry/main/.github/gantry-
-                                logo-ascii.png]
+[https://raw.githubusercontent.com/allenai/beaker-py/main/docs/source/_static/
+                         beaker-500px-transparent.png]
                           ************ BBeeaakkeerr GGaannttrryy ************
 Gantry streamlines running Python experiments in _B_e_a_k_e_r by managing containers
                             and boilerplate for you
 ===============================================================================
                               _[_C_I_]_[_P_y_P_I_]_[_L_i_c_e_n_s_e_]
 â¡ï¸*Easy to use* - **No Docker required!** ð« ð³ - No writing YAML
 experiment specs. - Easy setup. - Simple CLI. ð *Fast* - Fire off Beaker
@@ -51,118 +42,123 @@
 If you've already configured the [Beaker command-line client](https://
 github.com/allenai/beaker/), Gantry will find and use the existing
 configuration file (usually located at `$HOME/.beaker/config.yml`). Otherwise
 just set the environment variable `BEAKER_TOKEN` to your Beaker [user token]
 (https://beaker.org/user). The first time you call `gantry run ...` you'll also
 be prompted to provide a [GitHub personal access token](https://
 docs.github.com/en/authentication/keeping-your-account-and-data-secure/
-creating-a-personal-access-token) with the `repo` scope. This allows Gantry to
-clone your private repository when it runs in Beaker. You don't have to do this
-just yet (Gantry will prompt you for it), but if you need to update this token
-later you can use the `gantry config set-gh-token` command. 3. **Specify your
-Python environment.** Lastly - and this is the most important part - you'll
-have to create one of several different files that specify your Python
-environment. There are three options: 1. A conda [`environment.yml`](https://
-docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-
-environments.html#create-env-file-manually) file. 2. A [`setup.py`](https://
-docs.python.org/3/distutils/introduction.html#a-simple-example) file. 3. A PIP
-[`requirements.txt`](https://pip.pypa.io/en/stable/user_guide/#requirements-
-files) file. The first method is [the recommended approach](#use-conda),
-especially if you're already using conda. But it's perfectly okay to use a
-combination of these different approaches as well. This can be useful when, for
-example, you need to [use a CUDA-enabled version of PyTorch on Beaker but a
-CPU-only version locally](#how-do-i-use-a-cuda-enabled-version-of-pytorch-on-
-beaker-when-im-using-a-cpu-only-version-locally). ### Submit your first
-experiment with Gantry Let's spin up a Beaker experiment that just prints
-"Hello, World!" from Python. First make sure you've committed *and* pushed all
-changes so far in your repository. Then (from the root of your repository) run:
-```bash gantry run --workspace {WORKSPACE} --cluster {CLUSTER} -- python -
-c 'print("Hello, World!")' ``` Just replace `{WORKSPACE}` with the name of your
-own Beaker [*private*](#use-your-own-private-beaker-workspace) workspace and `
-{CLUSTER}` with the name of the Beaker cluster you want to run on. *âNote:
-Everything after the `--` is the command + arguments you want to run on Beaker.
-It's necessary to include the `--` if any of your arguments look like options
-themselves (like `-c` in this example) so gantry can differentiate them from
-its own options.* Try `gantry run --help` to see all of the available options.
-## Best practices ### Use your own private Beaker workspace Any authorized
-contributors to your workspace will have access to the secrets in your
-workspace, and Gantry needs to store your GitHub personal access token (PAT) as
-a secret in the workspace. That's also why it's important to [limit the scope
-and lifetime of your GitHub token](#limit-the-scope-and-lifetime-of-your-
-github-token). ### Limit the scope and lifetime of your GitHub token Your PAT
-only needs to have the `repo` scope and should have a short expiration time
-(e.g. 30 days). This limits the harm a bad actor could cause if they were able
-to read your PAT from your Beaker workspace somehow. ### Use conda Adding a
-[conda environment file](https://docs.conda.io/projects/conda/en/latest/user-
-guide/tasks/manage-environments.html#create-env-file-manually) will generally
-make your exact Python environment easier to reproduce, especially when you
-have platform-dependent requirements like PyTorch. You don't necessarily need
-to write the `environment.yml` file manually either. If you've already
-initialized a conda environment locally, you can just run: ```bash conda env
-export --from-history ``` See [Exporting an Environment File Across Platforms]
+creating-a-personal-access-token) with the `repo` scope if your repository is
+not public. This allows Gantry to clone your private repository when it runs in
+Beaker. You don't have to do this just yet (Gantry will prompt you for it), but
+if you need to update this token later you can use the `gantry config set-gh-
+token` command. 3. **Specify your Python environment.** Lastly - and this is
+the most important part - you'll have to create one of several different files
+that specify your Python environment. There are three options: 1. A conda
+[`environment.yml`](https://docs.conda.io/projects/conda/en/latest/user-guide/
+tasks/manage-environments.html#create-env-file-manually) file. 2. A
+[`setup.py`](https://docs.python.org/3/distutils/introduction.html#a-simple-
+example) file. 3. A PIP [`requirements.txt`](https://pip.pypa.io/en/stable/
+user_guide/#requirements-files) file. The first method is [the recommended
+approach](#use-conda), especially if you're already using conda. But it's
+perfectly okay to use a combination of these different approaches as well. This
+can be useful when, for example, you need to [use a CUDA-enabled version of
+PyTorch on Beaker but a CPU-only version locally](#how-do-i-use-a-cuda-enabled-
+version-of-pytorch-on-beaker-when-im-using-a-cpu-only-version-locally). ###
+Submit your first experiment with Gantry Let's spin up a Beaker experiment that
+just prints "Hello, World!" from Python. First make sure you've committed *and*
+pushed all changes so far in your repository. Then (from the root of your
+repository) run: ```bash gantry run --workspace {WORKSPACE} --cluster {CLUSTER}
+-- python -c 'print("Hello, World!")' ``` Just replace `{WORKSPACE}` with the
+name of your own Beaker [*non-public*](#use-your-own-non-public-beaker-
+workspace) workspace and `{CLUSTER}` with the name of the Beaker cluster you
+want to run on. *âNote: Everything after the `--` is the command + arguments
+you want to run on Beaker. It's necessary to include the `--` if any of your
+arguments look like options themselves (like `-c` in this example) so gantry
+can differentiate them from its own options.* Try `gantry run --help` to see
+all of the available options. ## Best practices ### Use your own non-public
+Beaker workspace Any authorized contributors to your workspace will have access
+to the secrets in your workspace, and Gantry needs to store your GitHub
+personal access token (PAT) as a secret in the workspace (for non-public
+repos). That's also why it's important to [limit the scope and lifetime of your
+GitHub token](#limit-the-scope-and-lifetime-of-your-github-token). ### Limit
+the scope and lifetime of your GitHub token Your PAT only needs to have the
+`repo` scope and should have a short expiration time (e.g. 30 days). This
+limits the harm a bad actor could cause if they were able to read your PAT from
+your Beaker workspace somehow. ### Use conda Adding a [conda environment file]
 (https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-
-environments.html#exporting-an-environment-file-across-platforms) for more
-details. It's also okay to [use a combination of conda environment and PIP
-requirements files](#can-i-use-both-conda-environment-and-pip-requirements-
-files). ## FAQ ### Can I use my own Docker/Beaker image? You sure can! Just set
-the `--beaker-image` or `--docker-image` flag. Gantry can use any image that
-has bash and conda installed. This can be useful when you have dependencies
-that take a long time to download and build (like PyTorch). In this case it
-works best if you build your image with a conda environment that already has
-your big dependencies installed. Then when you call `gantry run`, use the `--
-venv` option to tell Gantry to use that environment instead of creating a new
-conda environment in the container. You may also want to add a
-`requirements.txt` file to your repository that lists all of your dependencies
-(including PyTorch and anything else already installed in your image's conda
-environment) so Gantry can make sure the environment on the image is up-to-date
-when it runs. For example, you could use one of our [pre-built PyTorch images]
-(https://beaker.org/ws/ai2/fab/images?text=pytorch&sort=created:descending),
-such as [`ai2/pytorch1.11.0-cuda11.3-python3.9`](https://beaker.org/im/
-01G3S1CBQ0K832MCFDA77XQXFJ/details), like this: ```bash gantry run \ --beaker-
-image 'ai2/pytorch1.11.0-cuda11.3-python3.9' \ --venv 'base' \ --pip
-requirements.txt \ -- python -c 'print("Hello, World!")' ``` ### Will Gantry
-work for GPU experiments? Absolutely! This was the main use-case Gantry was
-developed for. Just set the `--gpus` option for `gantry run` to the number of
-GPUs you need. You should also ensure that the way in which you specify your
-Python environment (e.g. conda `environment.yml`, `setup.py`, or PIP
-`requirements.txt` file) will lead to your dependencies being properly
-installed to support the GPU hardware specific to the cluster you're running
-on. For example, if one of your dependencies is [PyTorch](https://pytorch.org/
-), you're probably best off writing a conda `environment.yml` file since conda
-is the preferred way to install PyTorch. You'll generally want to use the
-latest supported CUDA version, so in this case your `environment.yml` file
-could look like this: ```yaml name: torch-env channels: - pytorch dependencies:
-- python=3.9 - cudatoolkit=11.3 - numpy - pytorch - ... ``` ### Can I use both
-conda environment and PIP requirements files? Yes you can. Gantry will
-initialize your environment using your conda environment file (if you have one)
-and then will also check for a PIP requirements file. ### How do I use a CUDA-
-enabled version of PyTorch on Beaker when I'm using a CPU-only version locally?
-One way to handle this would be to start with a `requirements.txt` that lists
-the `torch` version you need along with any other dependencies, e.g. ``` #
-requirements.txt torch==1.11.0 ... ``` Then add a conda `environment.yml`
-somewhere in your repository that specifies exactly how to install PyTorch (and
-a CUDA toolkit) on Beaker, e.g.: ```yaml # beaker/environment.yml name: torch-
-env channels: - pytorch dependencies: - python=3.9 - cudatoolkit=11.3 -
-pytorch==1.11.0 # make sure this matches the version in requirements.txt ```
-When you call `gantry run`, use the `--conda` flag to specify the path to your
-conda env file (e.g. `--conda beaker/environment.yml`). Gantry will use that
-env file to initialize the environment, and then will install the rest of your
-dependencies from the `requirements.txt` file. ### How can I save results or
-metrics from an experiment? By default Gantry uses the `/results` directory on
-the image as the location of the results dataset. That means that everything
-your experiment writes to this directory will be persisted as a Beaker dataset
-when the experiment finalizes. And you can also create Beaker metrics for your
-experiment by writing a JSON file called `metrics.json` in the `/results`
-directory. ### Can I access data on NFS? Yes. When you choose an on-premise
-cluster managed by the Beaker team that supports the NFS drive it will be
-automatically attached to the experiment's container. ### How can I just see
-the Beaker experiment spec that Gantry uses? You can use the `--dry-run` option
-with `gantry run` to see what Gantry will submit without actually submitting an
-experiment. You can also use `--save-spec PATH` in combination with `--dry-run`
-to save the actual experiment spec to a YAML file. ### How can I update
-Gantry's GitHub token? Just use the command `gantry config set-gh-token`. ###
-How can I attach Beaker datasets to an experiment? Just use the `--dataset`
-option for `gantry run`. For example: ```bash gantry run --dataset 'petew/
-squad-train:/input-data' -- ls /input-data ``` ### Why "Gantry"? A gantry is a
+environments.html#create-env-file-manually) will generally make your exact
+Python environment easier to reproduce, especially when you have platform-
+dependent requirements like PyTorch. You don't necessarily need to write the
+`environment.yml` file manually either. If you've already initialized a conda
+environment locally, you can just run: ```bash conda env export --from-history
+``` See [Exporting an Environment File Across Platforms](https://docs.conda.io/
+projects/conda/en/latest/user-guide/tasks/manage-environments.html#exporting-
+an-environment-file-across-platforms) for more details. It's also okay to [use
+a combination of conda environment and PIP requirements files](#can-i-use-both-
+conda-environment-and-pip-requirements-files). ## FAQ ### Can I use my own
+Docker/Beaker image? You sure can! Just set the `--beaker-image` or `--docker-
+image` flag. Gantry can use any image that has bash installed. This can be
+useful when you have dependencies that take a long time to download and build
+(like PyTorch). In this case it works best if you build your image with a conda
+environment that already has your big dependencies installed. Then when you
+call `gantry run`, use the `--venv` option to tell Gantry to use that
+environment instead of creating a new conda environment in the container. You
+may also want to add a `requirements.txt` file to your repository that lists
+all of your dependencies (including PyTorch and anything else already installed
+in your image's conda environment) so Gantry can make sure the environment on
+the image is up-to-date when it runs. For example, you could use one of our
+[pre-built PyTorch images](https://beaker.org/ws/ai2/fab/
+images?text=pytorch&sort=created:descending), such as [`ai2/pytorch1.11.0-
+cuda11.3-python3.9`](https://beaker.org/im/01G3S1CBQ0K832MCFDA77XQXFJ/details),
+like this: ```bash gantry run \ --beaker-image 'ai2/pytorch1.11.0-cuda11.3-
+python3.9' \ --venv 'base' \ --pip requirements.txt \ -- python -c 'print
+("Hello, World!")' ``` ### Will Gantry work for GPU experiments? Absolutely!
+This was the main use-case Gantry was developed for. Just set the `--gpus`
+option for `gantry run` to the number of GPUs you need. You should also ensure
+that the way in which you specify your Python environment (e.g. conda
+`environment.yml`, `setup.py`, or PIP `requirements.txt` file) will lead to
+your dependencies being properly installed to support the GPU hardware specific
+to the cluster you're running on. For example, if one of your dependencies is
+[PyTorch](https://pytorch.org/), you're probably best off writing a conda
+`environment.yml` file since conda is the preferred way to install PyTorch.
+You'll generally want to use the latest supported CUDA version, so in this case
+your `environment.yml` file could look like this: ```yaml name: torch-env
+channels: - pytorch dependencies: - python=3.9 - cudatoolkit=11.3 - numpy -
+pytorch - ... ``` ### Can I use both conda environment and PIP requirements
+files? Yes you can. Gantry will initialize your environment using your conda
+environment file (if you have one) and then will also check for a PIP
+requirements file. ### How do I use a CUDA-enabled version of PyTorch on Beaker
+when I'm using a CPU-only version locally? One way to handle this would be to
+start with a `requirements.txt` that lists the `torch` version you need along
+with any other dependencies, e.g. ``` # requirements.txt torch==1.11.0 ... ```
+Then add a conda `environment.yml` somewhere in your repository that specifies
+exactly how to install PyTorch (and a CUDA toolkit) on Beaker, e.g.: ```yaml #
+beaker/environment.yml name: torch-env channels: - pytorch dependencies: -
+python=3.9 - cudatoolkit=11.3 - pytorch==1.11.0 # make sure this matches the
+version in requirements.txt ``` When you call `gantry run`, use the `--conda`
+flag to specify the path to your conda env file (e.g. `--conda beaker/
+environment.yml`). Gantry will use that env file to initialize the environment,
+and then will install the rest of your dependencies from the `requirements.txt`
+file. ### How can I save results or metrics from an experiment? By default
+Gantry uses the `/results` directory on the image as the location of the
+results dataset. That means that everything your experiment writes to this
+directory will be persisted as a Beaker dataset when the experiment finalizes.
+And you can also create Beaker metrics for your experiment by writing a JSON
+file called `metrics.json` in the `/results` directory. ### Can I access data
+on NFS? Yes. When you choose an on-premise cluster managed by the Beaker team
+that supports the NFS drive it will be automatically attached to the
+experiment's container. ### How can I just see the Beaker experiment spec that
+Gantry uses? You can use the `--dry-run` option with `gantry run` to see what
+Gantry will submit without actually submitting an experiment. You can also use
+`--save-spec PATH` in combination with `--dry-run` to save the actual
+experiment spec to a YAML file. ### How can I update Gantry's GitHub token?
+Just use the command `gantry config set-gh-token`. ### How can I attach Beaker
+datasets to an experiment? Just use the `--dataset` option for `gantry run`.
+For example: ```bash gantry run --dataset 'petew/squad-train:/input-data' -- ls
+/input-data ``` ### How can I run distributed batch jobs with Gantry? The three
+options `--replicas` (int), `--leader-selection` (flag), and `--host-
+networking` (flag) used together give you the ability to run distributed batch
+jobs. See the [Beaker docs](https://beaker-docs.apps.allenai.org/distributed-
+training.html#batch-jobs) for more information. ### Why "Gantry"? A gantry is a
 structure that's used, among other things, to lift containers off of ships.
 Analogously Beaker Gantry's purpose is to lift Docker containers (or at least
 the *management* of Docker containers) away from users.
```

### Comparing `beaker-gantry-0.9.4/gantry/__main__.py` & `beaker_gantry-1.0.0/gantry/commands/run.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,40 @@
-import os
-import signal
+import platform
+import random
+import string
 import sys
-import time
+from fnmatch import fnmatch
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 import click
 import rich
 from beaker import (
+    Beaker,
+    ExperimentConflict,
+    ExperimentSpec,
     ImageNotFound,
     Job,
     JobTimeoutError,
     Priority,
     SecretNotFound,
     TaskResources,
+    TaskSpec,
 )
-from click_help_colors import HelpColorsCommand, HelpColorsGroup
-from rich import pretty, print, prompt, traceback
+from rich import print, prompt
 
-from .common import constants, util
-from .common.aliases import PathOrStr
-from .common.util import print_stderr
-from .exceptions import *
-from .version import VERSION
-
-_CLICK_GROUP_DEFAULTS = {
-    "cls": HelpColorsGroup,
-    "help_options_color": "green",
-    "help_headers_color": "yellow",
-    "context_settings": {"max_content_width": 115},
-}
-
-_CLICK_COMMAND_DEFAULTS = {
-    "cls": HelpColorsCommand,
-    "help_options_color": "green",
-    "help_headers_color": "yellow",
-    "context_settings": {"max_content_width": 115},
-}
+from .. import constants, util
+from ..aliases import PathOrStr
+from ..exceptions import *
+from ..util import print_stderr
+from ..version import VERSION
+from .main import CLICK_COMMAND_DEFAULTS, main
 
 
-def excepthook(exctype, value, tb):
-    """
-    Used to patch `sys.excepthook` in order to customize handling of uncaught exceptions.
-    """
-    # Ignore `GantryError` because we don't need a traceback for those.
-    if issubclass(exctype, (GantryError,)):
-        print_stderr(f"[red][bold]{exctype.__name__}:[/] [i]{value}[/][/]")
-    # For interruptions, call the original exception handler.
-    elif issubclass(exctype, (KeyboardInterrupt, TermInterrupt)):
-        sys.__excepthook__(exctype, value, tb)
-    else:
-        print_stderr(traceback.Traceback.from_exception(exctype, value, tb, suppress=[click]))
-
-
-sys.excepthook = excepthook
-
-
-def handle_sigterm(sig, frame):
-    raise TermInterrupt
-
-
-@click.group(**_CLICK_GROUP_DEFAULTS)
-@click.version_option(version=VERSION)
-def main():
-    # Configure rich.
-    if os.environ.get("GANTRY_GITHUB_TESTING"):
-        # Force a broader terminal when running tests in GitHub Actions.
-        console_width = 180
-        rich.reconfigure(width=console_width, force_terminal=True, force_interactive=False)
-        pretty.install()
-    else:
-        pretty.install()
-
-    # Handle SIGTERM just like KeyboardInterrupt
-    signal.signal(signal.SIGTERM, handle_sigterm)
-
-    rich.get_console().print(
-        '''
-[cyan b]                                             o=======[]   [/]
-[cyan b]   __ _                    _               _ |_      []   [/]
-[cyan b]  / _` |  __ _    _ _     | |_      _ _   | || |     []   [/]
-[cyan b]  \__, | / _` |  | ' \    |  _|    | '_|   \_, |   _/ ]_  [/]
-[cyan b]  |___/  \__,_|  |_||_|   _\__|   _|_|_   _|__/   |_____| [/]
-[blue b]_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_| """"| [/]
-[blue b] `---------------------------------------------' [/]
-''',  # noqa: W605
-        highlight=False,
-    )
-
-    util.check_for_upgrades()
-
-
-@main.command(**_CLICK_COMMAND_DEFAULTS)
+@main.command(**CLICK_COMMAND_DEFAULTS)
 @click.argument("arg", nargs=-1)
 @click.option(
     "-n",
     "--name",
     type=str,
     help="""A name to assign to the experiment on Beaker. Defaults to a randomly generated name.""",
 )
@@ -118,19 +57,29 @@
 @click.option(
     "-c",
     "--cluster",
     type=str,
     multiple=True,
     default=None,
     help="""A potential cluster to use. This option can be used multiple times to allow multiple clusters.
+    You also specify it as a wildcard, e.g. '--cluster ai2/*-cirrascale'.
     If you don't specify a cluster or the priority, the priority will default to 'preemptible' and
     the job will be able to run on any on-premise cluster.""",
     show_default=True,
 )
 @click.option(
+    "--hostname",
+    type=str,
+    multiple=True,
+    default=None,
+    help="""Hostname constraints to apply to the experiment spec. This option can be used multiple times to allow
+    multiple hosts.""",
+    show_default=True,
+)
+@click.option(
     "--beaker-image",
     type=str,
     default=constants.DEFAULT_IMAGE,
     help="""The name or ID of an image on Beaker to use for your experiment.
     Mutually exclusive with --docker-image.""",
     show_default=True,
 )
@@ -160,15 +109,16 @@
     type=str,
     help="""Size of /dev/shm as a number with unit suffix (e.g. 2.5GiB).""",
 )
 @click.option(
     "--dataset",
     type=str,
     multiple=True,
-    help="""An input dataset in the form of 'dataset-name:/mount/location' to attach to your experiment.
+    help="""An input dataset in the form of 'dataset-name:/mount/location' or
+    'dataset-name:sub/path:/mount/location' to attach to your experiment.
     You can specify this option more than once to attach multiple datasets.""",
 )
 @click.option(
     "--gh-token-secret",
     type=str,
     help="""The name of the Beaker secret that contains your GitHub token.""",
     default=constants.GITHUB_TOKEN_SECRET,
@@ -245,21 +195,75 @@
     help="""A path to save the generated Beaker experiment spec to.""",
 )
 @click.option(
     "--priority",
     type=click.Choice([str(p) for p in Priority]),
     help="The job priority. If you don't specify at least one cluster, priority will default to 'preemptible'.",
 )
+@click.option(
+    "--install",
+    type=str,
+    help="""Override the default installation command, e.g. '--install "python setup.py install"'""",
+)
+@click.option(
+    "--no-python",
+    is_flag=True,
+    help="""If set, gantry will skip setting up a Python environment altogether.""",
+)
+@click.option(
+    "--replicas",
+    type=int,
+    help="""The number of task replicas to run.""",
+)
+@click.option(
+    "--leader-selection",
+    is_flag=True,
+    help="""Specifies that the first task replica should be the leader and populates each task
+    with 'BEAKER_LEADER_REPLICA_HOSTNAME' and 'BEAKER_LEADER_REPLICA_NODE_ID' environment variables.
+    This is only applicable when '--replicas INT' and '--host-networking' are used,
+    although the '--host-networking' flag can be omitted in this case since it's assumed.""",
+)
+@click.option(
+    "--host-networking",
+    is_flag=True,
+    help="""Specifies that each task replica should use the host's network.
+    When used with '--replicas INT', this allows the replicas to communicate with each
+    other using their hostnames.""",
+)
+@click.option(
+    "--propagate-failure", is_flag=True, help="""Stop the experiment if any task fails."""
+)
+@click.option(
+    "--synchronized-start-timeout",
+    type=str,
+    help="""
+    If set, jobs in the replicated task will wait this long to start until all other jobs are also ready.
+    """,
+)
+@click.option(
+    "-m",
+    "--mount",
+    type=str,
+    help="""Host directories to mount to the Beaker experiment. Should be in the form '{HOST_SOURCE}:{TARGET}'
+    similar to the '-v' option with 'docker run'.""",
+    multiple=True,
+)
+@click.option(
+    "-b", "--budget", type=str, help="""The budget account to associate with the experiment."""
+)
+@click.option("--preemptible", is_flag=True, help="""Mark the job as preemptible.""")
+@click.option("--stop-preemptible", is_flag=True, help="""Stop all preemptible on the cluster.""")
 def run(
     arg: Tuple[str, ...],
     name: Optional[str] = None,
     description: Optional[str] = None,
     task_name: str = "main",
     workspace: Optional[str] = None,
     cluster: Optional[Tuple[str, ...]] = None,
+    hostname: Optional[Tuple[str, ...]] = None,
     beaker_image: Optional[str] = constants.DEFAULT_IMAGE,
     docker_image: Optional[str] = None,
     cpus: Optional[float] = None,
     gpus: Optional[int] = None,
     memory: Optional[str] = None,
     shared_memory: Optional[str] = None,
     dataset: Optional[Tuple[str, ...]] = None,
@@ -273,14 +277,25 @@
     nfs: Optional[bool] = None,
     show_logs: bool = True,
     allow_dirty: bool = False,
     dry_run: bool = False,
     yes: bool = False,
     save_spec: Optional[PathOrStr] = None,
     priority: Optional[str] = None,
+    install: Optional[str] = None,
+    no_python: bool = False,
+    replicas: Optional[int] = None,
+    leader_selection: bool = False,
+    host_networking: bool = False,
+    propagate_failure: Optional[bool] = None,
+    synchronized_start_timeout: Optional[str] = None,
+    mount: Optional[Tuple[str, ...]] = None,
+    budget: Optional[str] = None,
+    preemptible: bool = False,
+    stop_preemptible: bool = False,
 ):
     """
     Run an experiment on Beaker.
 
     Example:
 
     $ gantry run --name 'hello-world' -- python -c 'print("Hello, World!")'
@@ -291,101 +306,146 @@
         )
 
     if (beaker_image is None) == (docker_image is None):
         raise ConfigurationError(
             "Either --beaker-image or --docker-image must be specified, but not both."
         )
 
+    if budget is None:
+        budget = prompt.Prompt.ask(
+            "[yellow]Missing '--budget' option, "
+            "see https://beaker-docs.apps.allenai.org/concept/budgets.html for more information.[/]\n"
+            "[i]Please enter the budget account to associate with this experiment[/]",
+        )
+
+    if not budget:
+        raise ConfigurationError("Budget account must be specified!")
+
     task_resources = TaskResources(
         cpu_count=cpus, gpu_count=gpus, memory=memory, shared_memory=shared_memory
     )
 
+    # Get repository account, name, and current ref.
+    github_account, github_repo, git_ref, is_public = util.ensure_repo(allow_dirty)
+
     # Initialize Beaker client and validate workspace.
-    beaker = util.ensure_workspace(workspace=workspace, yes=yes, gh_token_secret=gh_token_secret)
+    beaker = util.ensure_workspace(
+        workspace=workspace, yes=yes, gh_token_secret=gh_token_secret, public_repo=is_public
+    )
 
     if beaker_image is not None and beaker_image != constants.DEFAULT_IMAGE:
         try:
             beaker_image = beaker.image.get(beaker_image).full_name
         except ImageNotFound:
             raise ConfigurationError(f"Beaker image '{beaker_image}' not found")
 
-    # Get repository account, name, and current ref.
-    github_account, github_repo, git_ref = util.ensure_repo(allow_dirty)
-
     # Get the entrypoint dataset.
     entrypoint_dataset = util.ensure_entrypoint_dataset(beaker)
 
     # Get / set the GitHub token secret.
-    try:
-        beaker.secret.get(gh_token_secret)
-    except SecretNotFound:
-        print_stderr(
-            f"[yellow]GitHub token secret '{gh_token_secret}' not found in workspace.[/]\n"
-            f"You can create a suitable GitHub token by going to https://github.com/settings/tokens/new "
-            f"and generating a token with the '\N{ballot box with check} repo' scope."
-        )
-        gh_token = prompt.Prompt.ask(
-            "[i]Please paste your GitHub token here[/]",
-            password=True,
-        )
-        if not gh_token:
-            raise ConfigurationError("token cannot be empty!")
-        beaker.secret.write(gh_token_secret, gh_token)
-        print(
-            f"GitHub token secret uploaded to workspace as '{gh_token_secret}'.\n"
-            f"If you need to update this secret in the future, use the command:\n"
-            f"[i]$ gantry config set-gh-token[/]"
-        )
+    if not is_public:
+        try:
+            beaker.secret.get(gh_token_secret)
+        except SecretNotFound:
+            print_stderr(
+                f"[yellow]GitHub token secret '{gh_token_secret}' not found in workspace.[/]\n"
+                f"You can create a suitable GitHub token by going to https://github.com/settings/tokens/new "
+                f"and generating a token with the '\N{ballot box with check} repo' scope."
+            )
+            gh_token = prompt.Prompt.ask(
+                "[i]Please paste your GitHub token here[/]",
+                password=True,
+            )
+            if not gh_token:
+                raise ConfigurationError("token cannot be empty!")
+            beaker.secret.write(gh_token_secret, gh_token)
+            print(
+                f"GitHub token secret uploaded to workspace as '{gh_token_secret}'.\n"
+                f"If you need to update this secret in the future, use the command:\n"
+                f"[i]$ gantry config set-gh-token[/]"
+            )
 
-    gh_token_secret = util.ensure_github_token_secret(beaker, gh_token_secret)
+        gh_token_secret = util.ensure_github_token_secret(beaker, gh_token_secret)
 
     # Validate the input datasets.
-    datasets_to_use = util.ensure_datasets(beaker, *dataset) if dataset else []
+    datasets_to_use = ensure_datasets(beaker, *dataset) if dataset else []
 
     env_vars = []
     for e in env or []:
         try:
             env_name, val = e.split("=")
         except ValueError:
             raise ValueError("Invalid --env option: {e}")
         env_vars.append((env_name, val))
 
     env_secrets = []
     for e in env_secret or []:
         try:
             env_secret_name, secret = e.split("=")
         except ValueError:
-            raise ValueError(f"Invalid --env-secret option: {e}")
+            raise ValueError(f"Invalid --env-secret option: '{e}'")
         env_secrets.append((env_secret_name, secret))
 
+    mounts = []
+    for m in mount or []:
+        try:
+            source, target = m.split(":")
+        except ValueError:
+            raise ValueError(f"Invalid --mount option: '{m}'")
+        mounts.append((source, target))
+
+    # Validate clusters.
+    if cluster:
+        cl_objects = beaker.cluster.list()
+        final_clusters = []
+        for pat in cluster:
+            matching_clusters = [cl.full_name for cl in cl_objects if fnmatch(cl.full_name, pat)]
+            if matching_clusters:
+                final_clusters.extend(matching_clusters)
+            else:
+                raise ConfigurationError(f"cluster '{pat}' did not match any Beaker clusters")
+        cluster = list(set(final_clusters))  # type: ignore
+
     # Default to preemptible priority when no cluster has been specified.
     if not cluster and priority is None:
         priority = Priority.preemptible
 
     # Initialize experiment and task spec.
-    spec = util.build_experiment_spec(
+    spec = build_experiment_spec(
         task_name=task_name,
         clusters=list(cluster or []),
         task_resources=task_resources,
         arguments=list(arg),
         entrypoint_dataset=entrypoint_dataset.id,
         github_account=github_account,
         github_repo=github_repo,
         git_ref=git_ref,
+        budget=budget,
         description=description,
         beaker_image=beaker_image,
         docker_image=docker_image,
+        gh_token_secret=gh_token_secret if not is_public else None,
         conda=conda,
         pip=pip,
         venv=venv,
         nfs=nfs,
         datasets=datasets_to_use,
         env=env_vars,
         env_secrets=env_secrets,
         priority=priority,
+        install=install,
+        no_python=no_python,
+        replicas=replicas,
+        leader_selection=leader_selection,
+        host_networking=host_networking or (bool(replicas) and leader_selection),
+        propagate_failure=propagate_failure,
+        synchronized_start_timeout=synchronized_start_timeout,
+        mounts=mounts,
+        hostnames=None if hostname is None else list(hostname),
+        preemptible=preemptible,
     )
 
     if save_spec:
         if (
             Path(save_spec).is_file()
             and not yes
             and not prompt.Confirm.ask(
@@ -393,157 +453,250 @@
                 f"[i]Are you sure you want to overwrite it?[/][/]"
             )
         ):
             raise KeyboardInterrupt
         spec.to_file(save_spec)
         print(f"Experiment spec saved to {save_spec}")
 
+    if not name:
+        default_name = util.unique_name()
+        if yes:
+            name = default_name
+        else:
+            name = prompt.Prompt.ask(
+                "[i]What would you like to call this experiment?[/]", default=util.unique_name()
+            )
+
+    if not name:
+        raise ConfigurationError("Experiment name cannot be empty!")
+
     if dry_run:
         rich.get_console().rule("[b]Dry run[/]")
         print(
             f"[b]Workspace:[/] {beaker.workspace.url()}\n"
             f"[b]Commit:[/] https://github.com/{github_account}/{github_repo}/commit/{git_ref}\n"
+            f"[b]Name:[/] {name}\n"
             f"[b]Experiment spec:[/]",
             spec.to_json(),
         )
         return
 
-    name: str = name or prompt.Prompt.ask(  # type: ignore[assignment,no-redef]
-        "[i]What would you like to call this experiment?[/]", default=util.unique_name()
-    )
-    if not name:
-        raise ConfigurationError("Experiment name cannot be empty!")
+    name_prefix = name
+    while True:
+        try:
+            experiment = beaker.experiment.create(name, spec)
+            break
+        except ExperimentConflict:
+            name = (
+                name_prefix
+                + "-"
+                + random.choice(string.ascii_lowercase)
+                + random.choice(string.ascii_lowercase)
+                + random.choice(string.digits)
+                + random.choice(string.digits)
+            )
 
-    experiment = beaker.experiment.create(name, spec)
     print(f"Experiment submitted, see progress at {beaker.experiment.url(experiment)}")
 
+    if stop_preemptible:
+        if priority == Priority.preemptible:
+            print_stderr("[yellow]You cannot preempt other jobs when your job is preemptible.[/]")
+        elif not cluster:
+            print_stderr("[yellow]Preempt jobs requires specifying a cluster.[/]")
+        elif len(cluster) > 1:
+            print_stderr("[yellow]Preempt jobs requires specifying a single cluster.[/]")
+        elif not dry_run:
+            print(f"Preempting jobs on cluster {cluster[0]}...")
+            preempted = beaker.cluster.preempt_jobs(cluster[0], ignore_failures=True)
+            if preempted:
+                print(f"Preempted {len(preempted)} jobs on cluster {cluster[0]}")
+            else:
+                print("No more jobs to preempt")
+
     # Can return right away if timeout is 0.
     if timeout == 0:
         return
 
     job: Optional[Job] = None
-    exit_code: Optional[int] = None
-
     try:
         if show_logs:
-            start = time.monotonic()
-
-            print("Waiting for job to launch..", end="")
-            while job is None:
-                time.sleep(1.0)
-                print(".", end="")
-                job = beaker.experiment.tasks(experiment.id)[0].latest_job  # type: ignore
-
-            # Stream the logs.
-            print()
-            rich.get_console().rule("Logs")
-
-            last_timestamp: Optional[str] = None
-            while exit_code is None:
-                job = beaker.experiment.tasks(experiment.id)[0].latest_job  # type: ignore
-                assert job is not None
-                exit_code = job.status.exit_code
-                last_timestamp = util.display_logs(
-                    beaker.job.logs(job, quiet=True, since=last_timestamp),
-                    ignore_timestamp=last_timestamp,
-                )
-                time.sleep(2.0)
-                if timeout > 0 and time.monotonic() - start >= timeout:
-                    raise JobTimeoutError(f"Job did not finish within {timeout} seconds")
-
-            rich.get_console().rule("End logs")
-            print()
+            job = util.follow_experiment(beaker, experiment, timeout=timeout)
         else:
             experiment = beaker.experiment.wait_for(
                 experiment, timeout=timeout if timeout > 0 else None
             )[0]
             job = beaker.experiment.tasks(experiment)[0].latest_job  # type: ignore
             assert job is not None
-            exit_code = job.status.exit_code
-    except (KeyboardInterrupt, TermInterrupt, JobTimeoutError) as exc:
+    except (TermInterrupt, JobTimeoutError) as exc:
         print_stderr(f"[red][bold]{exc.__class__.__name__}:[/] [i]{exc}[/][/]")
         beaker.experiment.stop(experiment)
         print_stderr("[yellow]Experiment cancelled.[/]")
         sys.exit(1)
+    except KeyboardInterrupt as exc:
+        print_stderr(f"[red][bold]{exc.__class__.__name__}:[/] [i]{exc}[/][/]")
+        print(f"See the experiment at {beaker.experiment.url(experiment)}")
+        print_stderr(
+            f"[yellow]To cancel the experiment, run:\n[i]$ gantry stop {experiment.id}[/][/]"
+        )
+        sys.exit(1)
 
-    assert job is not None
-    assert exit_code is not None
+    util.display_results(beaker, experiment, job)
 
-    if exit_code > 0:
-        raise ExperimentFailedError(f"Experiment exited with non-zero code ({exit_code})")
 
-    assert job.execution is not None
-    assert job.status.started is not None
-    assert job.status.exited is not None
-
-    print(
-        f"[b green]\N{check mark}[/] [b cyan]{name}[/] completed successfully\n"
-        f"[b]Experiment:[/] {beaker.experiment.url(experiment)}\n"
-        f"[b]Runtime:[/] {util.format_timedelta(job.status.exited - job.status.started)}\n"
-        f"[b]Results:[/] {beaker.dataset.url(job.execution.result.beaker)}"
+def build_experiment_spec(
+    *,
+    task_name: str,
+    clusters: List[str],
+    task_resources: TaskResources,
+    arguments: List[str],
+    entrypoint_dataset: str,
+    github_account: str,
+    github_repo: str,
+    git_ref: str,
+    budget: str,
+    description: Optional[str] = None,
+    beaker_image: Optional[str] = None,
+    docker_image: Optional[str] = None,
+    gh_token_secret: Optional[str] = constants.GITHUB_TOKEN_SECRET,
+    conda: Optional[PathOrStr] = None,
+    pip: Optional[PathOrStr] = None,
+    venv: Optional[str] = None,
+    nfs: Optional[bool] = None,
+    datasets: Optional[List[Tuple[str, Optional[str], str]]] = None,
+    env: Optional[List[Tuple[str, str]]] = None,
+    env_secrets: Optional[List[Tuple[str, str]]] = None,
+    priority: Optional[Union[str, Priority]] = None,
+    install: Optional[str] = None,
+    no_python: bool = False,
+    replicas: Optional[int] = None,
+    leader_selection: bool = False,
+    host_networking: bool = False,
+    propagate_failure: Optional[bool] = None,
+    synchronized_start_timeout: Optional[str] = None,
+    mounts: Optional[List[Tuple[str, str]]] = None,
+    hostnames: Optional[List[str]] = None,
+    preemptible: bool = False,
+):
+    task_spec = (
+        TaskSpec.new(
+            task_name,
+            beaker_image=beaker_image,
+            docker_image=docker_image,
+            result_path=constants.RESULTS_DIR,
+            command=["bash", "/gantry/entrypoint.sh"],
+            arguments=arguments,
+            resources=task_resources,
+            priority=priority,
+            replicas=replicas,
+            leader_selection=leader_selection,
+            host_networking=host_networking,
+            propagate_failure=propagate_failure,
+            synchronized_start_timeout=synchronized_start_timeout,
+        )
+        .with_env_var(name="GANTRY_VERSION", value=VERSION)
+        .with_env_var(name="GITHUB_REPO", value=f"{github_account}/{github_repo}")
+        .with_env_var(name="GIT_REF", value=git_ref)
+        .with_env_var(name="GANTRY_TASK_NAME", value=task_name)
+        .with_dataset("/gantry", beaker=entrypoint_dataset)
     )
 
-    metrics = beaker.experiment.metrics(experiment)
-    if metrics is not None:
-        print("[b]Metrics:[/]", metrics)
+    if preemptible:
+        task_spec.context.preemptible = True
 
+    if clusters:
+        task_spec = task_spec.with_constraint(cluster=clusters)
 
-@main.group(**_CLICK_GROUP_DEFAULTS)
-def config():
-    """
-    Configure Gantry for a specific Beaker workspace.
-    """
+    if hostnames:
+        task_spec = task_spec.with_constraint(hostname=hostnames)
 
+    if gh_token_secret is not None:
+        task_spec = task_spec.with_env_var(name="GITHUB_TOKEN", secret=gh_token_secret)
 
-@config.command(**_CLICK_COMMAND_DEFAULTS)
-@click.argument("token")
-@click.option(
-    "-w",
-    "--workspace",
-    type=str,
-    help="""The Beaker workspace to use.
-    If not specified, your default workspace will be used.""",
-)
-@click.option(
-    "-s",
-    "--secret",
-    type=str,
-    help="""The name of the Beaker secret to write to.""",
-    default=constants.GITHUB_TOKEN_SECRET,
-    show_default=True,
-)
-@click.option(
-    "-y",
-    "--yes",
-    is_flag=True,
-    help="""Skip all confirmation prompts.""",
-)
-def set_gh_token(
-    token: str,
-    workspace: Optional[str] = None,
-    secret: str = constants.GITHUB_TOKEN_SECRET,
-    yes: bool = False,
-):
-    """
-    Set or update Gantry's GitHub token for the workspace.
+    for name, val in env or []:
+        task_spec = task_spec.with_env_var(name=name, value=val)
 
-    You can create a suitable GitHub token by going to https://github.com/settings/tokens/new
-    and generating a token with the '\N{ballot box with check} repo' scope.
+    for name, secret in env_secrets or []:
+        task_spec = task_spec.with_env_var(name=name, secret=secret)
 
-    Example:
+    if no_python:
+        task_spec = task_spec.with_env_var(name="NO_PYTHON", value="1")
+    else:
+        if conda is not None:
+            task_spec = task_spec.with_env_var(
+                name="CONDA_ENV_FILE",
+                value=str(conda),
+            )
+        elif Path(constants.CONDA_ENV_FILE).is_file():
+            task_spec = task_spec.with_env_var(
+                name="CONDA_ENV_FILE",
+                value=constants.CONDA_ENV_FILE,
+            )
+        elif Path(constants.CONDA_ENV_FILE_ALTERNATE).is_file():
+            task_spec = task_spec.with_env_var(
+                name="CONDA_ENV_FILE",
+                value=constants.CONDA_ENV_FILE_ALTERNATE,
+            )
+        else:
+            task_spec = task_spec.with_env_var(
+                name="PYTHON_VERSION", value=".".join(platform.python_version_tuple()[:-1])
+            )
 
-    $ gantry config set-gh-token "$GITHUB_TOKEN"
-    """
-    # Initialize Beaker client and validate workspace.
-    beaker = util.ensure_workspace(workspace=workspace, yes=yes, gh_token_secret=secret)
+        if pip is not None:
+            task_spec = task_spec.with_env_var(
+                name="PIP_REQUIREMENTS_FILE",
+                value=str(pip),
+            )
 
-    # Write token to secret.
-    beaker.secret.write(secret, token)
+        if venv is not None:
+            task_spec = task_spec.with_env_var(
+                name="VENV_NAME",
+                value=venv,
+            )
 
-    print(
-        f"[green]\N{check mark} GitHub token added to workspace "
-        f"'{beaker.config.default_workspace}' as the secret '{secret}'"
-    )
+        if install is not None:
+            task_spec = task_spec.with_env_var(name="INSTALL_CMD", value=install)
 
+    if (
+        nfs is None
+        and clusters
+        and all(
+            [
+                "cirrascale" in cluster and cluster not in constants.CLUSTERS_WITHOUT_NFS
+                for cluster in clusters
+            ]
+        )
+    ):
+        nfs = True
+
+    if nfs:
+        task_spec = task_spec.with_dataset(constants.NFS_MOUNT, host_path=constants.NFS_MOUNT)
 
-if __name__ == "__main__":
-    main()
+    if datasets:
+        for dataset_id, sub_path, path in datasets:
+            task_spec = task_spec.with_dataset(path, beaker=dataset_id, sub_path=sub_path)
+
+    if mounts:
+        for source, target in mounts:
+            task_spec = task_spec.with_dataset(target, host_path=source)
+
+    return ExperimentSpec(description=description, budget=budget, tasks=[task_spec])
+
+
+def ensure_datasets(beaker: Beaker, *datasets: str) -> List[Tuple[str, Optional[str], str]]:
+    out = []
+    for dataset_str in datasets:
+        dataset_name: str
+        path: str
+        sub_path: Optional[str] = None
+        if dataset_str.count(":") == 1:
+            dataset_name, path = dataset_str.split(":")
+        elif dataset_str.count(":") == 2:
+            dataset_name, sub_path, path = dataset_str.split(":")
+        else:
+            raise ValueError(
+                f"Bad '--dataset' specification: '{dataset_str}'\n"
+                f"Datasets should be in the form of 'dataset-name:/mount/location'"
+                f"or 'dataset-name:sub/path:/mount/location'"
+            )
+        dataset_id = beaker.dataset.get(dataset_name).id
+        out.append((dataset_id, sub_path, path))
+    return out
```

