# Comparing `tmp/browsergym_experiments-0.3.2.tar.gz` & `tmp/browsergym_experiments-0.3.3.tar.gz`

## Comparing `browsergym_experiments-0.3.2.tar` & `browsergym_experiments-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/requirements.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/src/browsergym/experiments/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/src/browsergym/experiments/agent.py
--rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/src/browsergym/experiments/loop.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/src/browsergym/experiments/utils.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/tests/test_exp_loop.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/.gitignore
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/README.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/requirements.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/src/browsergym/experiments/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/src/browsergym/experiments/agent.py
+-rw-r--r--   0        0        0    21193 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/src/browsergym/experiments/loop.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/src/browsergym/experiments/utils.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/tests/test_exp_loop.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/README.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.3/PKG-INFO
```

### Comparing `browsergym_experiments-0.3.2/src/browsergym/experiments/agent.py` & `browsergym_experiments-0.3.3/src/browsergym/experiments/agent.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.2/src/browsergym/experiments/loop.py` & `browsergym_experiments-0.3.3/src/browsergym/experiments/loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,18 @@
     record_video: bool = False
     wait_for_user_message: bool = False
     viewport: dict = None  # use default value from BrowserGym
     slow_mo: int = None  # use default value from BrowserGym
     storage_state: Optional[str | Path | dict] = None
     task_kwargs: dict = field(default_factory=lambda: {})
 
-    def make_env(self, action_mapping):
+    def make_env(self, action_mapping, exp_dir):
         extra_kwargs = {}
         if self.record_video:
-            extra_kwargs["record_video_dir"] = self.exp_dir
+            extra_kwargs["record_video_dir"] = exp_dir
         if self.viewport:
             extra_kwargs["viewport"] = self.viewport
         if self.slow_mo is not None:
             extra_kwargs["slow_mo"] = self.slow_mo
         if self.storage_state:
             extra_kwargs["pw_context_kwargs"] = {"storage_state": self.storage_state}
 
@@ -148,15 +148,17 @@
     def run(self):
         """Run the experiment and save the results"""
 
         episode_info = []
         try:
             logging.info(f"Running experiment {self.exp_name} in:\n  {self.exp_dir}")
             agent = self.agent_args.make_agent()
-            env = self.env_args.make_env(action_mapping=agent.action_set.to_python_code)
+            env = self.env_args.make_env(
+                action_mapping=agent.action_set.to_python_code, exp_dir=self.exp_dir
+            )
 
             err_msg, stack_trace = None, None
             step_info = StepInfo(step=0)
             episode_info = [step_info]
             step_info.from_reset(env, seed=self.env_args.task_seed)
 
             while not step_info.is_done:  # set a limit
```

### Comparing `browsergym_experiments-0.3.2/src/browsergym/experiments/utils.py` & `browsergym_experiments-0.3.3/src/browsergym/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.2/tests/test_exp_loop.py` & `browsergym_experiments-0.3.3/tests/test_exp_loop.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.2/pyproject.toml` & `browsergym_experiments-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.2/PKG-INFO` & `browsergym_experiments-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: browsergym-experiments
-Version: 0.3.2
+Version: 0.3.3
 Summary: Experimentation tools for BrowserGym
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Alex Lacoste, Massimo Caccia, Maxime Gasse, Thibault Le Sellier De Chezelles
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
-Requires-Dist: browsergym-core==0.3.2
+Requires-Dist: browsergym-core==0.3.3
 Requires-Dist: tiktoken>=0.4
 Description-Content-Type: text/markdown
 
 # BrowserGym experiments
 
 This package provides `browsergym.experiments`, a suite of experimentation tools for [BrowserGym](https://github.com/ServiceNow/BrowserGym).
```

