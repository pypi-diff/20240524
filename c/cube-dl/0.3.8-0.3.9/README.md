# Comparing `tmp/cube_dl-0.3.8.tar.gz` & `tmp/cube_dl-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cube_dl-0.3.8.tar", max compression
+gzip compressed data, was "cube_dl-0.3.9.tar", max compression
```

## Comparing `cube_dl-0.3.8.tar` & `cube_dl-0.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2024-03-31 06:39:15.080839 cube_dl-0.3.8/LICENSE
--rw-r--r--   0        0        0    33660 2024-03-31 06:39:15.080839 cube_dl-0.3.8/README.md
--rw-r--r--   0        0        0      130 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/__init__.py
--rw-r--r--   0        0        0     3164 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/c3lyr/__init__.py
--rw-r--r--   0        0        0     2021 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/c3lyr/dao.py
--rw-r--r--   0        0        0    11680 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/c3lyr/dao_json_impl.py
--rw-r--r--   0        0        0     3675 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/c3lyr/entities.py
--rw-r--r--   0        0        0      736 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/c3lyr/run_context.py
--rw-r--r--   0        0        0     1029 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/callback.py
--rw-r--r--   0        0        0      791 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/__init__.py
--rw-r--r--   0        0        0     1120 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/subcmd_add_exp.py
--rw-r--r--   0        0        0     3661 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/subcmd_ls.py
--rw-r--r--   0        0        0     1541 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/subcmd_new.py
--rw-r--r--   0        0        0     4961 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/subcmd_rm.py
--rw-r--r--   0        0        0     4471 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/subcmd_start.py
--rw-r--r--   0        0        0      376 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/subcmd_version.py
--rw-r--r--   0        0        0     7387 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/subcmds_exec.py
--rw-r--r--   0        0        0     1732 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/cli/utils.py
--rw-r--r--   0        0        0      483 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/config_sys/__init__.py
--rw-r--r--   0        0        0     1290 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/config_sys/config_decorators.py
--rw-r--r--   0        0        0    19230 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/config_sys/root_config.py
--rw-r--r--   0        0        0      917 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/config_sys/shared_config.py
--rw-r--r--   0        0        0      164 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/core/__init__.py
--rw-r--r--   0        0        0      584 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/core/components.py
--rw-r--r--   0        0        0     1832 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/main.py
--rw-r--r--   0        0        0     1559 2024-03-31 06:39:15.080839 cube_dl-0.3.8/cube_dl/utils.py
--rw-r--r--   0        0        0     1764 2024-03-31 06:39:15.084838 cube_dl-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    34665 1970-01-01 00:00:00.000000 cube_dl-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 05:29:19.118267 cube_dl-0.3.9/LICENSE
+-rw-r--r--   0        0        0    33660 2024-04-09 05:29:19.118267 cube_dl-0.3.9/README.md
+-rw-r--r--   0        0        0      130 2024-04-09 05:29:19.118267 cube_dl-0.3.9/cube_dl/__init__.py
+-rw-r--r--   0        0        0     3164 2024-04-09 05:29:19.118267 cube_dl-0.3.9/cube_dl/c3lyr/__init__.py
+-rw-r--r--   0        0        0     2021 2024-04-09 05:29:19.118267 cube_dl-0.3.9/cube_dl/c3lyr/dao.py
+-rw-r--r--   0        0        0    11680 2024-04-09 05:29:19.118267 cube_dl-0.3.9/cube_dl/c3lyr/dao_json_impl.py
+-rw-r--r--   0        0        0     3675 2024-04-09 05:29:19.118267 cube_dl-0.3.9/cube_dl/c3lyr/entities.py
+-rw-r--r--   0        0        0      736 2024-04-09 05:29:19.118267 cube_dl-0.3.9/cube_dl/c3lyr/run_context.py
+-rw-r--r--   0        0        0     1029 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/callback.py
+-rw-r--r--   0        0        0      791 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/subcmd_add_exp.py
+-rw-r--r--   0        0        0     3661 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/subcmd_ls.py
+-rw-r--r--   0        0        0     1541 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/subcmd_new.py
+-rw-r--r--   0        0        0     4961 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/subcmd_rm.py
+-rw-r--r--   0        0        0     4649 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/subcmd_start.py
+-rw-r--r--   0        0        0      376 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/subcmd_version.py
+-rw-r--r--   0        0        0     7387 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/subcmds_exec.py
+-rw-r--r--   0        0        0     1732 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/cli/utils.py
+-rw-r--r--   0        0        0      483 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/config_sys/__init__.py
+-rw-r--r--   0        0        0     1290 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/config_sys/config_decorators.py
+-rw-r--r--   0        0        0    19230 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/config_sys/root_config.py
+-rw-r--r--   0        0        0      917 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/config_sys/shared_config.py
+-rw-r--r--   0        0        0      164 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/core/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/core/components.py
+-rw-r--r--   0        0        0     1832 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/main.py
+-rw-r--r--   0        0        0     1559 2024-04-09 05:29:19.122267 cube_dl-0.3.9/cube_dl/utils.py
+-rw-r--r--   0        0        0     1764 2024-04-09 05:29:19.122267 cube_dl-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    34665 1970-01-01 00:00:00.000000 cube_dl-0.3.9/PKG-INFO
```

### Comparing `cube_dl-0.3.8/LICENSE` & `cube_dl-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/README.md` & `cube_dl-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/c3lyr/__init__.py` & `cube_dl-0.3.9/cube_dl/c3lyr/__init__.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/c3lyr/dao.py` & `cube_dl-0.3.9/cube_dl/c3lyr/dao.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/c3lyr/dao_json_impl.py` & `cube_dl-0.3.9/cube_dl/c3lyr/dao_json_impl.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/c3lyr/entities.py` & `cube_dl-0.3.9/cube_dl/c3lyr/entities.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/c3lyr/run_context.py` & `cube_dl-0.3.9/cube_dl/c3lyr/run_context.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/callback.py` & `cube_dl-0.3.9/cube_dl/callback.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/cli/__init__.py` & `cube_dl-0.3.9/cube_dl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/cli/subcmd_add_exp.py` & `cube_dl-0.3.9/cube_dl/cli/subcmd_add_exp.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/cli/subcmd_ls.py` & `cube_dl-0.3.9/cube_dl/cli/subcmd_ls.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/cli/subcmd_new.py` & `cube_dl-0.3.9/cube_dl/cli/subcmd_new.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/cli/subcmd_rm.py` & `cube_dl-0.3.9/cube_dl/cli/subcmd_rm.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/cli/subcmd_start.py` & `cube_dl-0.3.9/cube_dl/cli/subcmd_start.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,18 +93,23 @@
         if args.dest is not None:
             if not osp.exists(args.dest):
                 os.mkdir(args.dest)
             save_dir = args.dest
         else:
             save_dir = os.getcwd()
 
-        if len(os.listdir(save_dir)) != 0:
+        # Check non-hidden file(s)
+        non_hidden_file_cnt = 0
+        for fn in os.listdir(save_dir):
+            if not fn.startswith("."):
+                non_hidden_file_cnt += 1
+        if non_hidden_file_cnt != 0:
             print(
                 get_fail_colored_str(
-                    f'The destination directory "{save_dir}" is not empty, ' "please switch another one to avoid chaos."
+                    f'The destination directory "{save_dir}" is not empty, please switch another one to avoid chaos.'
                 )
             )
             return
 
         print(f'Downloading files to "{save_dir}"...')
         _download_github_directory(
             owner=args.owner,
```

### Comparing `cube_dl-0.3.8/cube_dl/cli/subcmds_exec.py` & `cube_dl-0.3.9/cube_dl/cli/subcmds_exec.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/cli/utils.py` & `cube_dl-0.3.9/cube_dl/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/config_sys/config_decorators.py` & `cube_dl-0.3.9/cube_dl/config_sys/config_decorators.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/config_sys/root_config.py` & `cube_dl-0.3.9/cube_dl/config_sys/root_config.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/config_sys/shared_config.py` & `cube_dl-0.3.9/cube_dl/config_sys/shared_config.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/core/components.py` & `cube_dl-0.3.9/cube_dl/core/components.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/main.py` & `cube_dl-0.3.9/cube_dl/main.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/cube_dl/utils.py` & `cube_dl-0.3.9/cube_dl/utils.py`

 * *Files identical despite different names*

### Comparing `cube_dl-0.3.8/pyproject.toml` & `cube_dl-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cube-dl"
-version = "0.3.8"
+version = "0.3.9"
 description = '"The last stop" for training your deep learning models. Manage tons of configurations and experiments with minimal changes to existing code.'
 keywords = ["python", "data-science", "machine-learning", "deep-learning", "python3", "pytorch", "pytorch-lightning"]
 authors = ["Alive1024 <2431945058@qq.com>"]
 readme = "README.md"
 license = ""
 classifiers = ["Development Status :: 3 - Alpha",
                "Programming Language :: Python :: 3",
```

### Comparing `cube_dl-0.3.8/PKG-INFO` & `cube_dl-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cube-dl
-Version: 0.3.8
+Version: 0.3.9
 Summary: "The last stop" for training your deep learning models. Manage tons of configurations and experiments with minimal changes to existing code.
 Keywords: python,data-science,machine-learning,deep-learning,python3,pytorch,pytorch-lightning
 Author: Alive1024
 Author-email: 2431945058@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: MacOS
```

