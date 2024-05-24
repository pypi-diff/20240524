# Comparing `tmp/jjuke-0.0.7.4.tar.gz` & `tmp/jjuke-0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jjuke-0.0.7.4.tar", last modified: Mon Mar 25 15:31:22 2024, max compression
+gzip compressed data, was "jjuke-0.0.7.5.tar", last modified: Fri May 24 16:39:18 2024, max compression
```

## Comparing `jjuke-0.0.7.4.tar` & `jjuke-0.0.7.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.474285 jjuke-0.0.7.4/
--rw-r--r--   0 root         (0) root         (0)      246 2024-03-25 15:31:22.474285 jjuke-0.0.7.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.470285 jjuke-0.0.7.4/jjuke/
--rw-r--r--   0 root         (0) root         (0)      337 2024-03-25 15:29:52.000000 jjuke-0.0.7.4/jjuke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.470285 jjuke-0.0.7.4/jjuke/datasets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 07:45:26.000000 jjuke-0.0.7.4/jjuke/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-12-12 14:15:11.000000 jjuke-0.0.7.4/jjuke/datasets/dataloaders.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-10-25 08:38:27.000000 jjuke-0.0.7.4/jjuke/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.470285 jjuke-0.0.7.4/jjuke/metrics/
--rw-r--r--   0 root         (0) root         (0)       67 2023-10-25 07:45:26.000000 jjuke-0.0.7.4/jjuke/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11621 2023-10-25 07:45:26.000000 jjuke-0.0.7.4/jjuke/metrics/evaluation_metrics.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-10-25 07:45:26.000000 jjuke-0.0.7.4/jjuke/metrics/pointcloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.474285 jjuke-0.0.7.4/jjuke/metrics/score/
--rw-r--r--   0 root         (0) root         (0)     5441 2023-10-25 07:45:26.000000 jjuke-0.0.7.4/jjuke/metrics/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7792 2023-10-25 07:45:26.000000 jjuke-0.0.7.4/jjuke/metrics/score/fid.py
--rw-r--r--   0 root         (0) root         (0)    11612 2023-10-25 07:45:26.000000 jjuke-0.0.7.4/jjuke/metrics/score/inception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.474285 jjuke-0.0.7.4/jjuke/models/
--rw-r--r--   0 root         (0) root         (0)      120 2023-10-25 08:45:24.000000 jjuke-0.0.7.4/jjuke/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11188 2024-02-24 08:45:45.000000 jjuke-0.0.7.4/jjuke/models/ema_trainer.py
--rw-r--r--   0 root         (0) root         (0)     7369 2023-10-25 07:45:27.000000 jjuke-0.0.7.4/jjuke/models/optimizer.py
--rw-r--r--   0 root         (0) root         (0)    18251 2023-12-22 05:50:14.000000 jjuke-0.0.7.4/jjuke/models/scheduler.py
--rw-r--r--   0 root         (0) root         (0)    23098 2024-03-25 15:28:40.000000 jjuke-0.0.7.4/jjuke/models/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.474285 jjuke-0.0.7.4/jjuke/net_utils/
--rw-r--r--   0 root         (0) root         (0)      423 2023-10-25 08:41:07.000000 jjuke-0.0.7.4/jjuke/net_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-12-04 16:48:19.000000 jjuke-0.0.7.4/jjuke/net_utils/dist.py
--rw-r--r--   0 root         (0) root         (0)     3024 2023-10-25 07:45:27.000000 jjuke-0.0.7.4/jjuke/net_utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     5957 2023-12-04 14:35:52.000000 jjuke-0.0.7.4/jjuke/net_utils/options.py
--rw-r--r--   0 root         (0) root         (0)     4170 2024-02-13 15:09:50.000000 jjuke-0.0.7.4/jjuke/net_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.474285 jjuke-0.0.7.4/jjuke/utils/
--rw-r--r--   0 root         (0) root         (0)      214 2023-11-01 15:44:44.000000 jjuke-0.0.7.4/jjuke/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9553 2023-10-25 07:45:27.000000 jjuke-0.0.7.4/jjuke/utils/interp1d.py
--rw-r--r--   0 root         (0) root         (0)    20788 2023-10-25 07:45:27.000000 jjuke-0.0.7.4/jjuke/utils/resize_right.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-11-01 15:29:40.000000 jjuke-0.0.7.4/jjuke/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)    25983 2024-02-13 15:17:05.000000 jjuke-0.0.7.4/jjuke/utils/vis3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:31:22.470285 jjuke-0.0.7.4/jjuke.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2024-03-25 15:31:22.000000 jjuke-0.0.7.4/jjuke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      828 2024-03-25 15:31:22.000000 jjuke-0.0.7.4/jjuke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 15:31:22.000000 jjuke-0.0.7.4/jjuke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 15:31:22.000000 jjuke-0.0.7.4/jjuke.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-25 15:31:22.000000 jjuke-0.0.7.4/jjuke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-25 15:31:22.000000 jjuke-0.0.7.4/jjuke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 15:31:22.474285 jjuke-0.0.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      555 2024-03-25 15:30:06.000000 jjuke-0.0.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      846 2023-10-25 07:46:37.000000 jjuke-0.0.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/jjuke/
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-24 16:38:34.000000 jjuke-0.0.7.5/jjuke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/jjuke/datasets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 07:45:26.000000 jjuke-0.0.7.5/jjuke/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-12-12 14:15:11.000000 jjuke-0.0.7.5/jjuke/datasets/dataloaders.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-10-25 08:38:27.000000 jjuke-0.0.7.5/jjuke/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/jjuke/metrics/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-10-25 07:45:26.000000 jjuke-0.0.7.5/jjuke/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11621 2023-10-25 07:45:26.000000 jjuke-0.0.7.5/jjuke/metrics/evaluation_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-10-25 07:45:26.000000 jjuke-0.0.7.5/jjuke/metrics/pointcloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/jjuke/metrics/score/
+-rw-r--r--   0 root         (0) root         (0)     5441 2023-10-25 07:45:26.000000 jjuke-0.0.7.5/jjuke/metrics/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7792 2023-10-25 07:45:26.000000 jjuke-0.0.7.5/jjuke/metrics/score/fid.py
+-rw-r--r--   0 root         (0) root         (0)    11612 2023-10-25 07:45:26.000000 jjuke-0.0.7.5/jjuke/metrics/score/inception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/jjuke/models/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-10-25 08:45:24.000000 jjuke-0.0.7.5/jjuke/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11188 2024-02-24 08:45:45.000000 jjuke-0.0.7.5/jjuke/models/ema_trainer.py
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-10-25 07:45:27.000000 jjuke-0.0.7.5/jjuke/models/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    18251 2023-12-22 05:50:14.000000 jjuke-0.0.7.5/jjuke/models/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    23098 2024-03-25 15:28:40.000000 jjuke-0.0.7.5/jjuke/models/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/jjuke/net_utils/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-10-25 08:41:07.000000 jjuke-0.0.7.5/jjuke/net_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-12-04 16:48:19.000000 jjuke-0.0.7.5/jjuke/net_utils/dist.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-10-25 07:45:27.000000 jjuke-0.0.7.5/jjuke/net_utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7160 2024-05-24 16:36:40.000000 jjuke-0.0.7.5/jjuke/net_utils/options.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2024-02-13 15:09:50.000000 jjuke-0.0.7.5/jjuke/net_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/jjuke/utils/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-11-01 15:44:44.000000 jjuke-0.0.7.5/jjuke/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9553 2023-10-25 07:45:27.000000 jjuke-0.0.7.5/jjuke/utils/interp1d.py
+-rw-r--r--   0 root         (0) root         (0)    20788 2023-10-25 07:45:27.000000 jjuke-0.0.7.5/jjuke/utils/resize_right.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-11-01 15:29:40.000000 jjuke-0.0.7.5/jjuke/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)    25983 2024-02-13 15:17:05.000000 jjuke-0.0.7.5/jjuke/utils/vis3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/jjuke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-05-24 16:39:18.000000 jjuke-0.0.7.5/jjuke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2024-05-24 16:39:18.000000 jjuke-0.0.7.5/jjuke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 16:39:18.000000 jjuke-0.0.7.5/jjuke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 16:39:18.000000 jjuke-0.0.7.5/jjuke.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-24 16:39:18.000000 jjuke-0.0.7.5/jjuke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-24 16:39:18.000000 jjuke-0.0.7.5/jjuke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 16:39:18.054471 jjuke-0.0.7.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-24 16:39:10.000000 jjuke-0.0.7.5/setup.py
```

### Comparing `jjuke-0.0.7.4/jjuke/datasets/dataloaders.py` & `jjuke-0.0.7.5/jjuke/datasets/dataloaders.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/main.py` & `jjuke-0.0.7.5/jjuke/main.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/metrics/evaluation_metrics.py` & `jjuke-0.0.7.5/jjuke/metrics/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/metrics/pointcloud.py` & `jjuke-0.0.7.5/jjuke/metrics/pointcloud.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/metrics/score/__init__.py` & `jjuke-0.0.7.5/jjuke/metrics/score/__init__.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/metrics/score/fid.py` & `jjuke-0.0.7.5/jjuke/metrics/score/fid.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/metrics/score/inception.py` & `jjuke-0.0.7.5/jjuke/metrics/score/inception.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/models/ema_trainer.py` & `jjuke-0.0.7.5/jjuke/models/ema_trainer.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/models/optimizer.py` & `jjuke-0.0.7.5/jjuke/models/optimizer.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/models/scheduler.py` & `jjuke-0.0.7.5/jjuke/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/models/trainer.py` & `jjuke-0.0.7.5/jjuke/models/trainer.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/net_utils/dist.py` & `jjuke-0.0.7.5/jjuke/net_utils/dist.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/net_utils/logger.py` & `jjuke-0.0.7.5/jjuke/net_utils/logger.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/net_utils/options.py` & `jjuke-0.0.7.5/jjuke/net_utils/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -179,7 +179,44 @@
         args.exp_path = Path(args.exp_path)
     else:
         print("There's no any experiment directory in the config file.")
 
     args = _postprocess_yaml_recursive(args)
 
     return args
+
+
+def get_acc_config(argv=None):
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--config_file", type=str)
+
+    opt, unknown = parser.parse_known_args(argv)
+
+    cfg = load_yaml(opt.config_file)
+    cli = OmegaConf.from_dotlist(unknown)
+    args = OmegaConf.merge(cfg, cli)
+
+    n = datetime.now()
+    timestr = "{}{:02d}{:02d}_{:02d}{:02d}".format(
+        n.year%100, n.month, n.day, n.hour, n.minute
+    )
+    timestr += "_" + Path(opt.config_file).stem
+    if "memo" in args.keys():
+        timestr += "_%s" % args.memo
+
+    if "exp_dir" in args.keys():
+        args.exp_path = os.path.join(args["exp_dir"], timestr)
+        (Path(args.exp_path) / "samples").mkdir(parents=True, exist_ok=True)
+        print("Start on exp_path:", args.exp_path)
+
+        with open(os.path.join(args.exp_path, "args.yaml"), "w") as f:
+            OmegaConf.save(args, f)
+
+        print(OmegaConf.to_yaml(args, resolve=True))
+        args = OmegaConf.to_container(args, resolve=True)
+        args = EasyDict(args)
+        args.exp_path = Path(args.exp_path)
+    else:
+        print("There's no any experiment directory in the config file.")
+
+    args = _postprocess_yaml_recursive(args)
+    return args
```

### Comparing `jjuke-0.0.7.4/jjuke/net_utils/utils.py` & `jjuke-0.0.7.5/jjuke/net_utils/utils.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/utils/interp1d.py` & `jjuke-0.0.7.5/jjuke/utils/interp1d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/utils/resize_right.py` & `jjuke-0.0.7.5/jjuke/utils/resize_right.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/utils/utils.py` & `jjuke-0.0.7.5/jjuke/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke/utils/vis3d.py` & `jjuke-0.0.7.5/jjuke/utils/vis3d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.7.4/jjuke.egg-info/SOURCES.txt` & `jjuke-0.0.7.5/jjuke.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 jjuke/__init__.py
 jjuke/main.py
 jjuke.egg-info/PKG-INFO
 jjuke.egg-info/SOURCES.txt
 jjuke.egg-info/dependency_links.txt
 jjuke.egg-info/not-zip-safe
```

### Comparing `jjuke-0.0.7.4/setup.py` & `jjuke-0.0.7.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import find_packages, setup
 
 setup(
     name="jjuke",
-    version="0.0.7.4",
+    version="0.0.7.5",
     description="Framework and utilities for Deep Learning models with Pytorch by JJukE",
     author="JJukE",
     author_email="psj9156@gmail.com",
     url="https://github.com/JJukE/JJuk_E.git",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
         "torch",
         "numpy",
-        "pytorch3d",
         "scikit-image",
         "omegaconf",
         "easydict",
         "tqdm",
         "einops"
     ],
     keywords=["JJukE", "jjuke"]
```

