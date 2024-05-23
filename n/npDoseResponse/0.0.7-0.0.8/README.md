# Comparing `tmp/npdoseresponse-0.0.7.tar.gz` & `tmp/npdoseresponse-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdoseresponse-0.0.7.tar", last modified: Mon May 20 01:10:16 2024, max compression
+gzip compressed data, was "npdoseresponse-0.0.8.tar", last modified: Thu May 23 22:51:49 2024, max compression
```

## Comparing `npdoseresponse-0.0.7.tar` & `npdoseresponse-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-20 01:10:16.346737 npdoseresponse-0.0.7/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.7/LICENSE
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-20 01:10:16.346034 npdoseresponse-0.0.7/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1641 2024-05-19 23:42:02.000000 npdoseresponse-0.0.7/README.md
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-20 01:10:16.333261 npdoseresponse-0.0.7/npDoseResponse/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      242 2024-05-20 01:09:54.000000 npdoseresponse-0.0.7/npDoseResponse/__init__.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)    33881 2024-05-20 00:49:07.000000 npdoseresponse-0.0.7/npDoseResponse/npDoseResponse.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5934 2024-05-19 22:45:09.000000 npdoseresponse-0.0.7/npDoseResponse/rbf.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     6165 2024-05-19 23:40:58.000000 npdoseresponse-0.0.7/npDoseResponse/utils.py
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-20 01:10:16.345448 npdoseresponse-0.0.7/npDoseResponse.egg-info/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-20 01:10:16.000000 npdoseresponse-0.0.7/npDoseResponse.egg-info/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-20 01:10:16.000000 npdoseresponse-0.0.7/npDoseResponse.egg-info/SOURCES.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-20 01:10:16.000000 npdoseresponse-0.0.7/npDoseResponse.egg-info/dependency_links.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-20 01:10:16.000000 npdoseresponse-0.0.7/npDoseResponse.egg-info/requires.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-20 01:10:16.000000 npdoseresponse-0.0.7/npDoseResponse.egg-info/top_level.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-20 01:10:16.346845 npdoseresponse-0.0.7/setup.cfg
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-20 01:09:51.000000 npdoseresponse-0.0.7/setup.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-23 22:51:49.586390 npdoseresponse-0.0.8/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.8/LICENSE
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-23 22:51:49.585215 npdoseresponse-0.0.8/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1641 2024-05-19 23:42:02.000000 npdoseresponse-0.0.8/README.md
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-23 22:51:49.579294 npdoseresponse-0.0.8/npDoseResponse/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      242 2024-05-23 22:50:44.000000 npdoseresponse-0.0.8/npDoseResponse/__init__.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)    36365 2024-05-23 22:48:39.000000 npdoseresponse-0.0.8/npDoseResponse/npDoseResponse.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5934 2024-05-19 22:45:09.000000 npdoseresponse-0.0.8/npDoseResponse/rbf.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     6165 2024-05-19 23:40:58.000000 npdoseresponse-0.0.8/npDoseResponse/utils.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-23 22:51:49.584239 npdoseresponse-0.0.8/npDoseResponse.egg-info/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2141 2024-05-23 22:51:49.000000 npdoseresponse-0.0.8/npDoseResponse.egg-info/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-23 22:51:49.000000 npdoseresponse-0.0.8/npDoseResponse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-23 22:51:49.000000 npdoseresponse-0.0.8/npDoseResponse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-23 22:51:49.000000 npdoseresponse-0.0.8/npDoseResponse.egg-info/requires.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-23 22:51:49.000000 npdoseresponse-0.0.8/npDoseResponse.egg-info/top_level.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-23 22:51:49.586529 npdoseresponse-0.0.8/setup.cfg
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-23 22:50:55.000000 npdoseresponse-0.0.8/setup.py
```

### Comparing `npdoseresponse-0.0.7/LICENSE` & `npdoseresponse-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.7/PKG-INFO` & `npdoseresponse-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npDoseResponse
-Version: 0.0.7
+Version: 0.0.8
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npdoseresponse-0.0.7/README.md` & `npdoseresponse-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.7/npDoseResponse/npDoseResponse.py` & `npdoseresponse-0.0.8/npDoseResponse/npDoseResponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
     
     Y_est = LocalPolyRegMain(Y, X, x_eval=x_eval, degree=degree, deriv_ord=deriv_ord, 
                              h=h, b=b, kernT=kernT, kernS=kernS)
     return Y_est
 
 
-def LocalPolyRegMain(Y, X, x_eval=None, degree=2, deriv_ord=0, h=None, b=None, 
+def LocalPolyRegMain(Y, X, x_eval=None, degree=2, deriv_ord=1, h=None, b=None, 
                      kernT="epanechnikov", kernS="epanechnikov"):
     '''
     Main function for computing the local polynomial regression.
     
     
     Parameters
     ----------
@@ -356,17 +356,18 @@
                                          h=h, b=b, C_h=C_h, C_b=C_b, print_bw=print_bw, 
                                          kernT=kernT, kernS=kernS)
     
     theta_C = np.sum(weight_mat * beta_mat, axis=0)
     return theta_C
 
 
-def DerivEffectBoot(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, 
-                    b=None, C_h=7, C_b=3, print_bw=True, degree=2, deriv_ord=1, 
-                    kernT="epanechnikov", kernS="epanechnikov", boot_num=500, 
+def DerivEffectBoot(Y, X, t_eval=None, boot_num=500, alpha=0.95, h_bar=None, 
+                    kernT_bar="gaussian", h=None, b=None, C_h=7, C_b=3, 
+                    print_bw=True, degree=2, deriv_ord=1, 
+                    kernT="epanechnikov", kernS="epanechnikov", 
                     parallel=False, processes=20):
     '''
     Conduct inference on the derivative of the dose-response curve via Nadaraya-Watson 
     conditional CDF estimator and nonparametric bootstrap.
     
     Parameters
     ----------
@@ -377,14 +378,21 @@
             The first column of X is the treatment/exposure variable, while 
             the other d columns are confounding variables of n observations.
             
         t_eval: (m,)-array
             The coordinates of the m evaluation points. (Default: t_eval=None. 
             Then, t_eval=X[:,0], which consists of the observed treatment variables.)
             
+        boot_num: int
+            The number of bootstrapping times. (Default: bootstrap_num=500.) 
+            
+        alpha: float
+            The confidence level of both the uniform confidence band and pointwise
+            confidence interval. (Default: alpha=0.95.)
+            
         h_bar: float
             The bandwidth parameters for the Nadaraya-Watson conditional CDF estimator. 
             (Default: h_bar=None. Then, the Silverman's rule of thumb is applied. 
             See Chen et al.(2016) for details.)
             
         kernT_bar: str
             The name of the kernel function for Nadaraya-Watson conditional CDF 
@@ -408,51 +416,71 @@
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
             conditional mean outcome function with respect to the treatment variable.)
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
             
-        boot_num: int
-            The number of bootstrapping times. (Default: bootstrap_num=500.) 
-            
         parallel: boolean
             The indicator of whether the function should be parallel executed by
             multi-processing. (Default: parallel=False.)
             
         processes: int
             The number of processes for parallel execution. (Default: processes=20.)
     
     Return
     ----------
+        theta_C: (m,)-array
+            The estimated derivative of the dose-response curve evaluated at 
+            points "t_eval".
+            
         theta_C_boot: (m,)-array
             The estimated derivatives of the dose-response curve on bootstrap samples 
             evaluated at points "t_eval".
+            
+        theta_alpha: float
+            The width of the uniform confidence band.
+            
+        theta_alpha_var: (m,)-array
+            The widths of the pointwise confidence bands at evaluation points "t_eval".
     '''
     
     if t_eval is None: 
         t_eval = X[:,0].copy()
         
     n = X.shape[0]  ## Number of data points
     
+    theta_est = DerivEffect(Y, X, t_eval=t_eval, h_bar=h_bar, kernT_bar=kernT_bar, 
+                            h=h, b=b, C_h=C_h, C_b=C_b, print_bw=print_bw, 
+                            degree=degree, deriv_ord=deriv_ord, 
+                            kernT=kernT, kernS=kernS, parallel=parallel, processes=processes)
+    
     theta_C_boot = np.zeros((boot_num, t_eval.shape[0]))
     b = 0
     while b < boot_num:
         ind = np.random.choice(n, size=n, replace=True)
         X_boot = X[ind,:]
         Y_boot = Y[ind]
         theta_C_boot[b,:] = DerivEffect(Y_boot, X_boot, t_eval=t_eval, h_bar=h_bar, 
                                    kernT_bar=kernT_bar, h=h, b=b, C_h=C_h, C_b=C_b, 
                                    print_bw=print_bw, degree=degree, deriv_ord=deriv_ord, 
                                    kernT=kernT, kernS=kernS, parallel=parallel, 
                                    processes=processes)
         if np.sum(np.isnan(theta_C_boot[b,:])) == 0:
             b += 1
-        
-    return theta_C_boot
+    
+    # Compute the 95% uniform confidence bands
+    theta_boot_sup = np.max(np.abs(theta_C_boot - theta_est), axis=1)
+    theta_alpha = np.quantile(theta_boot_sup, 0.95)
+
+    # Compute the 95% pointwise confidence intervals
+    theta_boot_abs = np.abs(theta_C_boot - theta_est)
+    theta_alpha_var = np.quantile(theta_boot_abs, 0.95, axis=0)
+    
+    return theta_est, theta_C_boot, theta_alpha, theta_alpha_var
 
 
 def IntegEst(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
              C_h=7, C_b=3, print_bw=True, degree=2, deriv_ord=1, kernT="epanechnikov", 
              kernS="epanechnikov", parallel=False, processes=20):
     '''
     Estimating the dose-response curve via our integral estimator with linear 
@@ -536,17 +564,18 @@
     m_samp = np.mean(Y) + np.sum(int_mat_up - int_mat_down, axis=0)/n
     
     m_est = np.interp(t_eval, T_sort, m_samp)
             
     return m_est
 
 
-def IntegEstBoot(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
-             C_h=7, C_b=3, print_bw=True, degree=2, deriv_ord=1, kernT="epanechnikov", 
-             kernS="epanechnikov", boot_num=500, parallel=False, processes=20):
+def IntegEstBoot(Y, X, t_eval=None, boot_num=500, alpha=0.95, h_bar=None, 
+                 kernT_bar="gaussian", h=None, b=None, C_h=7, C_b=3, print_bw=True, 
+                 degree=2, deriv_ord=1, kernT="epanechnikov", kernS="epanechnikov", 
+                 parallel=False, processes=20):
     '''
     Conduct inference on the dose-response curve via our integral estimator and
     nonparametric bootstrap.
     
     Parameters
     ----------
         Y: (n,)-array
@@ -556,14 +585,21 @@
             The first column of X is the treatment/exposure variable, while 
             the other d columns are confounding variables of n observations.
             
         t_eval: (m,)-array
             The coordinates of the m evaluation points. (Default: t_eval=None. 
             Then, t_eval=X[:,0].)
             
+        boot_num: int
+            The number of bootstrapping times. (Default: bootstrap_num=500.) 
+        
+        alpha: float
+            The confidence level of both the uniform confidence band and pointwise
+            confidence interval. (Default: alpha=0.95.)
+            
         h_bar: float
             The bandwidth parameters for the Nadaraya-Watson conditional CDF estimator. 
             (Default: h_bar=None. Then, the Silverman's rule of thumb is applied. 
             See Chen et al.(2016) for details.)
             
         kernT_bar: str
             The name of the kernel function for Nadaraya-Watson conditional CDF estimator.
@@ -586,34 +622,45 @@
             The order of the estimated derivative the conditional mean outcome function. 
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
             conditional mean outcome function with respect to the treatment variable.)
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
-            
-        boot_num: int
-            The number of bootstrapping times. (Default: bootstrap_num=500.) 
         
         parallel: boolean
             The indicator of whether the function should be parallel executed by
             multi-processing. (Default: parallel=False.)
             
         processes: int
             The number of processes for parallel execution. (Default: processes=20.)
             
     Return
     ----------
+        m_est: (m,)-array
+            The estimated dose-response curve evaluated at points "t_eval".
+            
         m_est_boot: (boot_num, m)-array
             The estimated dose-response curves (or their derivatives) on the bootstrap 
             samples evaluated at points "t_eval".
+            
+        m_alpha: float
+            The width of the uniform confidence band.
+            
+        m_alpha_var: (m,)-array
+            The widths of the pointwise confidence bands at evaluation points "t_eval".
     '''
     
     if t_eval is None: 
         t_eval = X[:,0].copy()
+        
+    m_est = IntegEst(Y, X, t_eval=t_eval, h_bar=h_bar, kernT_bar=kernT_bar, 
+                     h=h, b=b, C_h=C_h, C_b=C_b, print_bw=print_bw, degree=degree, 
+                     deriv_ord=deriv_ord, kernT=kernT, kernS=kernS, parallel=parallel, 
+                     processes=processes)
     
     n = X.shape[0]  ## Number of data points
     m_est_boot = np.zeros((boot_num, t_eval.shape[0]))
     b = 0
     while b < boot_num:
         ind = np.random.choice(n, size=n, replace=True)
         X_boot = X[ind,:]
@@ -621,15 +668,23 @@
         m_est_boot[b,:] = IntegEst(Y_boot, X_boot, t_eval=t_eval, h_bar=h_bar, 
                                    kernT_bar=kernT_bar, h=h, b=b, C_h=C_h, C_b=C_b, 
                                    print_bw=print_bw, degree=degree, deriv_ord=deriv_ord, 
                                    kernT=kernT, kernS=kernS, parallel=parallel, 
                                    processes=processes)
         if np.sum(np.isnan(m_est_boot[b,:])) == 0:
             b += 1
-    return m_est_boot
+            
+    # Compute the 95% uniform confidence bands
+    m_boot_sup = np.max(np.abs(m_est_boot - m_est), axis=1)
+    m_alpha = np.quantile(m_boot_sup, 0.95)
+
+    # Compute the 95% pointwise confidence intervals
+    m_boot_abs = np.abs(m_est_boot - m_est)
+    m_alpha_var = np.quantile(m_boot_abs, 0.95, axis=0)
+    return m_est, m_est_boot, m_alpha, m_alpha_var
 
 
 def LocalPolyReg1D(Y, X, h=None, x_eval=None, degree=2, deriv_ord=0, kernel="epanechnikov"):
     '''
     Local polynomial regression in one dimension.
     
     Parameters
```

### Comparing `npdoseresponse-0.0.7/npDoseResponse/rbf.py` & `npdoseresponse-0.0.8/npDoseResponse/rbf.py`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.7/npDoseResponse/utils.py` & `npdoseresponse-0.0.8/npDoseResponse/utils.py`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.7/npDoseResponse.egg-info/PKG-INFO` & `npdoseresponse-0.0.8/npDoseResponse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npDoseResponse
-Version: 0.0.7
+Version: 0.0.8
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/npDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npdoseresponse-0.0.7/setup.py` & `npdoseresponse-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="npDoseResponse",
-    version="0.0.7",
+    version="0.0.8",
     author="Yikun Zhang",
     author_email="yikunzhang@foxmail.com",
     description="Nonparametric Estimation and Inference on Dose-Response Curves",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhangyk8/npDoseResponse",
     classifiers=[
```

