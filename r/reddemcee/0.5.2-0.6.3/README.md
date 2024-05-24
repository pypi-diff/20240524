# Comparing `tmp/reddemcee-0.5.2.tar.gz` & `tmp/reddemcee-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddemcee-0.5.2.tar", last modified: Wed Jan 24 17:20:15 2024, max compression
+gzip compressed data, was "reddemcee-0.6.3.tar", last modified: Fri May 24 17:37:46 2024, max compression
```

## Comparing `reddemcee-0.5.2.tar` & `reddemcee-0.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2024-01-24 17:20:15.289498 reddemcee-0.5.2/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1069 2023-11-13 21:26:55.000000 reddemcee-0.5.2/LICENSE
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        0 2023-11-13 21:26:55.000000 reddemcee-0.5.2/MANIFEST.in
--rw-r--r--   0 reddtea   (1000) reddtea   (1000)     1834 2024-01-24 17:20:15.289498 reddemcee-0.5.2/PKG-INFO
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1307 2023-11-13 21:27:47.000000 reddemcee-0.5.2/README.md
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       85 2023-11-13 21:26:55.000000 reddemcee-0.5.2/pyproject.toml
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       38 2024-01-24 17:20:15.289498 reddemcee-0.5.2/setup.cfg
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      842 2024-01-24 17:19:54.000000 reddemcee-0.5.2/setup.py
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2024-01-24 17:20:15.285498 reddemcee-0.5.2/src/
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2024-01-24 17:20:15.285498 reddemcee-0.5.2/src/reddemcee/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    13930 2024-01-24 17:19:44.000000 reddemcee-0.5.2/src/reddemcee/__init__.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1096 2023-11-13 21:32:01.000000 reddemcee-0.5.2/src/reddemcee/reddwrappers.py
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2024-01-24 17:20:15.289498 reddemcee-0.5.2/src/reddemcee.egg-info/
--rw-r--r--   0 reddtea   (1000) reddtea   (1000)     1834 2024-01-24 17:20:15.000000 reddemcee-0.5.2/src/reddemcee.egg-info/PKG-INFO
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      317 2024-01-24 17:20:15.000000 reddemcee-0.5.2/src/reddemcee.egg-info/SOURCES.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        1 2024-01-24 17:20:15.000000 reddemcee-0.5.2/src/reddemcee.egg-info/dependency_links.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       45 2024-01-24 17:20:15.000000 reddemcee-0.5.2/src/reddemcee.egg-info/requires.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       10 2024-01-24 17:20:15.000000 reddemcee-0.5.2/src/reddemcee.egg-info/top_level.txt
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2024-01-24 17:20:15.289498 reddemcee-0.5.2/tests/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      196 2023-11-13 21:26:55.000000 reddemcee-0.5.2/tests/test_reddemcee.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2024-05-24 17:37:46.909937 reddemcee-0.6.3/
+-rw-r--r--   0 reddtea    (501) staff       (20)     1069 2023-11-13 21:26:55.000000 reddemcee-0.6.3/LICENSE
+-rw-r--r--   0 reddtea    (501) staff       (20)       54 2024-05-24 17:27:21.000000 reddemcee-0.6.3/MANIFEST.in
+-rw-r--r--   0 reddtea    (501) staff       (20)     2636 2024-05-24 17:37:46.909619 reddemcee-0.6.3/PKG-INFO
+-rw-r--r--   0 reddtea    (501) staff       (20)     2108 2024-05-15 20:41:03.000000 reddemcee-0.6.3/README.md
+-rw-r--r--   0 reddtea    (501) staff       (20)       85 2023-11-13 21:26:55.000000 reddemcee-0.6.3/pyproject.toml
+-rw-r--r--   0 reddtea    (501) staff       (20)       38 2024-05-24 17:37:46.909993 reddemcee-0.6.3/setup.cfg
+-rw-r--r--   0 reddtea    (501) staff       (20)      842 2024-05-24 17:36:18.000000 reddemcee-0.6.3/setup.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2024-05-24 17:37:46.904611 reddemcee-0.6.3/src/
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2024-05-24 17:37:46.907205 reddemcee-0.6.3/src/reddemcee/
+-rw-r--r--   0 reddtea    (501) staff       (20)    14311 2024-05-24 17:36:30.000000 reddemcee-0.6.3/src/reddemcee/__init__.py
+-rw-r--r--   0 reddtea    (501) staff       (20)     1096 2023-11-13 21:32:01.000000 reddemcee-0.6.3/src/reddemcee/reddwrappers.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2024-05-24 17:37:46.909254 reddemcee-0.6.3/src/reddemcee.egg-info/
+-rw-r--r--   0 reddtea    (501) staff       (20)     2636 2024-05-24 17:37:46.000000 reddemcee-0.6.3/src/reddemcee.egg-info/PKG-INFO
+-rw-r--r--   0 reddtea    (501) staff       (20)      317 2024-05-24 17:37:46.000000 reddemcee-0.6.3/src/reddemcee.egg-info/SOURCES.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)        1 2024-05-24 17:37:46.000000 reddemcee-0.6.3/src/reddemcee.egg-info/dependency_links.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)       45 2024-05-24 17:37:46.000000 reddemcee-0.6.3/src/reddemcee.egg-info/requires.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)       10 2024-05-24 17:37:46.000000 reddemcee-0.6.3/src/reddemcee.egg-info/top_level.txt
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2024-05-24 17:37:46.908754 reddemcee-0.6.3/tests/
+-rw-r--r--   0 reddtea    (501) staff       (20)      196 2023-11-13 21:26:55.000000 reddemcee-0.6.3/tests/test_reddemcee.py
```

### Comparing `reddemcee-0.5.2/LICENSE` & `reddemcee-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reddemcee-0.5.2/setup.py` & `reddemcee-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="reddemcee",
-    version="0.5.2",
+    version="0.6.3",
     author="ReddTea",
     author_email="redd@tea.com",
     description="An Adaptative Parallel Tempering wrapper for emcee 3 for personal use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `reddemcee-0.5.2/src/reddemcee/__init__.py` & `reddemcee-0.6.3/src/reddemcee/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-__version__ = '0.5'
+__version__ = '0.6.3'
 __all__ = ['PTSampler']
 
 import numpy as np
 import emcee
 from emcee.utils import deprecation_warning
 
 from tqdm import tqdm
@@ -77,31 +77,31 @@
             if deprecated_args[i] is not None:
                 deprecation_warning(f"The '{deprecated_args_str[i]}' argument is deprecated")
         ######################################################
         # Parse the move schedule
 
         # Beta ladder initialization
         self.ntemps = ntemps or 5
-        self.betas = betas or set_temp_ladder(self.ntemps, ndim)
+        self.betas = betas if betas is not None else set_temp_ladder(self.ntemps, ndim)
         #####################################################
         # Initialize instance variables
         self.nwalkers = nwalkers
         self.ndim = ndim
         self.lp_ = log_prior_fn
         self.ll_ = log_likelihood_fn
 
         self.lp_args_ = logp_args
         self.ll_args_ = logl_args
 
         self.n_swap_accept = np.zeros(ntemps-1)
 
         self.pool = pool
         self.adaptative = adaptative
-        self.config_adaptation_lag = 10000
-        self.config_adaptation_time = 100
+        self.config_adaptation_halflife = 10000  # adaptations reduced by half at this time
+        self.config_adaptation_rate = 100  # smaller, faster
         self.nglobal = 0
 
         # Default values for lists
         default_list = lambda lst, size, default: [default for _ in range(size)] if lst is None else lst
         self.vectorize = [False for _ in range(self.ntemps)] if vectorize is False else vectorize
         self.moves = default_list(moves, self.ntemps, None)
         self.blobs_dtype = default_list(blobs_dtype, self.ntemps, None)
@@ -121,29 +121,32 @@
 
         self.sampler = [emcee.EnsembleSampler(self.nwalkers, self.ndim,
                         self.my_probs_fn[t], pool=self.pool,
                         moves=self.moves[t], backend=self.backend[t],
                         vectorize=self.vectorize[t], blobs_dtype=self.blobs_dtype[t],
                         ) for t in range(self.ntemps)]
 
+        self.betas_history = [[] for _ in range(self.ntemps)]
+        self.betas_history_bool = True
+        self.ratios_history = np.array([])
+
 
     def __str__(self):
         return 'My sampler, ntemps = %i' % self.ntemps
 
 
     def __getitem__(self, n):
         return self.sampler[n]
 
 
     def __setitem__(self, n, thing):
         self.sampler[n] = thing
 
 
-    def sample(
-        self,
+    def sample(self,
         initial_state,
         iterations=1,
         tune=False,
         skip_initial_state_check=False,
         thin_by=1,
         thin=None,
         store=True,
@@ -159,15 +162,17 @@
                                                thin_by=thin_by,
                                                thin=thin,
                                                store=store,
                                                progress=progress,
                                                progress_kwargs=progress_kwargs):
                 pass
 
-
+        if self.betas_history_bool:
+            for ti in range(self.ntemps):
+                self.betas_history[ti].extend(np.ones(iterations) * self.betas[ti])
         self.temp_swaps_()
         if self.adaptative:
             dbetas = self.ladder_adjustment()
             self.betas += dbetas
 
             # Mutate my_probs_fn
             for t in range(self.ntemps-1, 0, -1):
@@ -193,30 +198,32 @@
             asel = paccept > raccept
 
             self.n_swap_accept[t-1] = np.sum(asel)
 
             self.samp[t].coords[asel], self.samp[t-1].coords[asel] = self.samp[t-1].coords[asel], self.samp[t].coords[asel]
             self.samp[t].log_prob[asel], self.samp[t-1].log_prob[asel] = self.samp[t-1].log_prob[asel] - dbeta*ll2[asel], self.samp[t].log_prob[asel] + dbeta*ll1[asel]
             self.samp[t].blobs[asel], self.samp[t-1].blobs[asel] = ll2[asel], ll1[asel]
-
+            
         self.ratios = self.n_swap_accept / self.nwalkers
-
+        self.ratios_history = np.append(self.ratios_history, self.ratios)
+        
 
     def ladder_adjustment(self):
         """
         Execute temperature adjustment according to dynamics outlined in
         `arXiv:1501.05823 <http://arxiv.org/abs/1501.05823>`_.
         """
 
         betas = self.betas.copy()
         time = self[0].iteration
 
         # Modulate temperature adjustments with a hyperbolic decay.
-        decay = self.config_adaptation_lag / (time + self.config_adaptation_lag)
-        kappa = decay / self.config_adaptation_time
+        decay = self.config_adaptation_halflife / (time + self.config_adaptation_halflife)
+
+        kappa = decay / self.config_adaptation_rate
 
         # Construct temperature adjustments.
         dSs = kappa * (self.ratios[:-1] - self.ratios[1:])
 
         # Compute new ladder (hottest and coldest chains don't move).
         deltaTs = np.diff(1 / betas[:-1])
         deltaTs *= np.exp(dSs)
@@ -226,16 +233,17 @@
         # Mutate Ladder
         #self.betas = betas
         # Mutate my_probs_fn
         #for t in range(self.ntemps):
         #    self.my_probs_fn[t].beta = self.betas[t]
 
 
-    def thermodynamic_integration(self):
-        sampler_dict = {'flat':False, 'discard':discard}
+    def thermodynamic_integration(self, coef=3, sampler_dict=None):
+        if sampler_dict is None:
+            sampler_dict = {'flat':False, 'discard':10}
         logls0 = self.get_func('get_blobs', kwargs=sampler_dict)
         logls = self.get_mean_logls(logls0, coef=coef)
 
         if self.betas[-1] != 0:
             betas1 = np.concatenate((self.betas, [0]))
             betas2 = np.concatenate((self.betas[::2], [0]))
 
@@ -316,46 +324,42 @@
             if len(chunk) > 1:
                 chunks.append(chunk)
                 end_index = start_index  # Update the end_index for the next iteration
         return chunks
 
 
     def get_Z(self, discard=1, coef=3, largo=100):
-        if True:
-            sampler_dict={'flat':True, 'discard':discard}
-            logl_r = np.array(self.get_func('get_blobs', kwargs=sampler_dict))
-
-            chunks = self.extract_chunks(logl_r, chunk_size=largo)
-
-            zz_ = []
-            zze_ = []
-            for subset in chunks:
-                logls = self.get_mean_logls(subset, coef=coef)
-                
-                z, zerr = self.hand_calc_z(logls)
-                zz_.append(z)
-                zze_.append(zerr)
-        if False:
-            print('Try larger sample')
-            return [0], [0]
+        sampler_dict={'flat':True, 'discard':discard}
+        logl_r = np.array(self.get_func('get_blobs', kwargs=sampler_dict))
+
+        chunks = self.extract_chunks(logl_r, chunk_size=largo)
+
+        zz_ = []
+        zze_ = []
+        for subset in chunks:
+            logls = self.get_mean_logls(subset, coef=coef)
+
+            z, zerr = self.hand_calc_z(logls)
+            zz_.append(z)
+            zze_.append(zerr)
         return zz_, zze_
 
 
     def get_mean_logls(self, logls, coef=3):
         ll0 = np.array([])
         for i in range(self.ntemps):
             loglrow = logls[i]
             mask = (np.mean(loglrow) + coef*np.std(loglrow) > loglrow) & (loglrow > np.mean(loglrow) - coef*np.std(loglrow))
             loglrow0 = np.mean(loglrow[mask])
             ll0 = np.append(ll0, loglrow0)
 
         return ll0
 
 
-    def run_mcmc(self, initial_state, nsteps, iterations=1, progress=True):
+    def run_mcmc(self, initial_state, nsweeps, nsteps, progress=True):
         if initial_state is None:
             print('Initial state is none')
             if self.__previous_state[0] is None:
                 raise ValueError(
                     "Cannot have `initial_state=None` if run_mcmc has never "
                     "been called.")
             initial_state = self.__previous_state
@@ -363,18 +367,18 @@
         self.sampler = [emcee.EnsembleSampler(self.nwalkers, self.ndim,
                         self.my_probs_fn[t], pool=self.pool,
                         moves=self.moves[t], backend=self.backend[t],
                         vectorize=self.vectorize[t], blobs_dtype=self.blobs_dtype[t],
                         ) for t in range(self.ntemps)]
 
         results = None
-        pbar = tqdm(total=nsteps*iterations, disable=not progress)
-        for _ in range(nsteps):
-            for results in self.sample(initial_state, iterations=iterations):
-                pbar.update(iterations)
+        pbar = tqdm(total=nsteps*nsweeps, disable=not progress)
+        for _ in range(nsweeps):
+            for results in self.sample(initial_state, iterations=nsteps):
+                pbar.update(nsteps)
 
         pbar.close()
 
         return results
 
 
     def get_attr(self, x):
```

### Comparing `reddemcee-0.5.2/src/reddemcee/reddwrappers.py` & `reddemcee-0.6.3/src/reddemcee/reddwrappers.py`

 * *Files identical despite different names*

