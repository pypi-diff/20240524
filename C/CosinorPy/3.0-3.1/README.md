# Comparing `tmp/CosinorPy-3.0.tar.gz` & `tmp/CosinorPy-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CosinorPy-3.0.tar", last modified: Wed Aug 30 11:38:52 2023, max compression
+gzip compressed data, was "dist\CosinorPy-3.1.tar", last modified: Fri May 24 06:52:22 2024, max compression
```

## Comparing `CosinorPy-3.0.tar` & `CosinorPy-3.1.tar`

### file list

```diff
@@ -1,11 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-30 11:38:52.000000 CosinorPy-3.0/
-drwxrwxrwx   0        0        0        0 2023-08-30 11:38:52.000000 CosinorPy-3.0/CosinorPy/
--rw-rw-rw-   0        0        0        0 2020-01-31 11:38:57.000000 CosinorPy-3.0/CosinorPy/__init__.py
--rw-rw-rw-   0        0        0   176393 2023-05-25 14:59:42.000000 CosinorPy-3.0/CosinorPy/cosinor.py
--rw-rw-rw-   0        0        0    47270 2023-06-21 13:04:23.000000 CosinorPy-3.0/CosinorPy/cosinor1.py
--rw-rw-rw-   0        0        0   111987 2023-05-25 15:12:11.000000 CosinorPy-3.0/CosinorPy/cosinor_nonlin.py
--rw-rw-rw-   0        0        0    18116 2023-06-14 17:07:46.000000 CosinorPy-3.0/CosinorPy/file_parser.py
--rw-rw-rw-   0        0        0      205 2023-05-25 15:26:44.000000 CosinorPy-3.0/CosinorPy/helpers.py
--rw-rw-rw-   0        0        0      857 2023-08-30 11:38:52.000000 CosinorPy-3.0/PKG-INFO
--rw-rw-rw-   0        0        0       40 2020-02-04 14:43:54.000000 CosinorPy-3.0/setup.cfg
--rw-rw-rw-   0        0        0     1183 2023-08-30 11:31:55.000000 CosinorPy-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:52:22.000000 CosinorPy-3.1/
+drwxrwxrwx   0        0        0        0 2024-05-24 06:52:21.000000 CosinorPy-3.1/CosinorPy/
+-rw-rw-rw-   0        0        0        0 2024-03-04 07:09:31.000000 CosinorPy-3.1/CosinorPy/__init__.py
+-rw-rw-rw-   0        0        0   184849 2024-03-06 11:12:46.000000 CosinorPy-3.1/CosinorPy/cosinor.py
+-rw-rw-rw-   0        0        0    47270 2024-03-04 07:09:31.000000 CosinorPy-3.1/CosinorPy/cosinor1.py
+-rw-rw-rw-   0        0        0   111987 2024-03-04 07:09:31.000000 CosinorPy-3.1/CosinorPy/cosinor_nonlin.py
+-rw-rw-rw-   0        0        0    18116 2024-03-04 07:09:31.000000 CosinorPy-3.1/CosinorPy/file_parser.py
+-rw-rw-rw-   0        0        0      285 2024-03-06 11:03:52.000000 CosinorPy-3.1/CosinorPy/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:52:22.000000 CosinorPy-3.1/CosinorPy.egg-info/
+-rw-rw-rw-   0        0        0      843 2024-05-24 06:52:21.000000 CosinorPy-3.1/CosinorPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-05-24 06:52:21.000000 CosinorPy-3.1/CosinorPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 06:52:21.000000 CosinorPy-3.1/CosinorPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-24 06:52:21.000000 CosinorPy-3.1/CosinorPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 06:52:21.000000 CosinorPy-3.1/CosinorPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2024-03-04 07:09:31.000000 CosinorPy-3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      843 2024-05-24 06:52:22.000000 CosinorPy-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5179 2024-03-04 07:09:31.000000 CosinorPy-3.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-24 06:52:22.000000 CosinorPy-3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2024-05-24 06:47:15.000000 CosinorPy-3.1/setup.py
```

### Comparing `CosinorPy-3.0/CosinorPy/cosinor.py` & `CosinorPy-3.1/CosinorPy/cosinor.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 import copy
 import itertools
 from matplotlib.lines import Line2D
 from random import sample
 
 import os
 
+import copy
+
 from CosinorPy.helpers import df_add_row
 
 #from skopt.space import Space
 #from skopt.sampler import Lhs
 
    
 def periodogram_df(df, folder = '', **kwargs):
@@ -947,30 +949,37 @@
                     per = 100000
                     
                     
                 df_pop = df[df.test.str.startswith(name)]   
 
                 if folder:                    
                     save_to=os.path.join(folder,prefix+name+'_compnts='+str(n_comps) +'_per=' + str(per))                    
-                    _, statistics, _, rhythm_params, _ = population_fit(df_pop, n_components = n_comps, period = per, save_to = save_to, **kwargs)
+                    _, statistics, statistics_params, rhythm_params, _ = population_fit(df_pop, n_components = n_comps, period = per, save_to = save_to, **kwargs)
                 else:                    
-                    _, statistics, _, rhythm_params, _ = population_fit(df_pop, n_components = n_comps, period = per, **kwargs)
-                    
-                            
-                df_results = df_add_row(df_results,{'test': name, 
-                                            'period': per,
-                                            'n_components': n_comps,
-                                            'p': statistics['p'], 
-                                            'p_reject': statistics['p_reject'],
-                                            'RSS': statistics['RSS'],
-                                            'ME': statistics['ME'],
-                                            'resid_SE': statistics['resid_SE'],
-                                            'amplitude': rhythm_params['amplitude'],
-                                            'acrophase': rhythm_params['acrophase'],
-                                            'mesor': rhythm_params['mesor']})
+                    _, statistics, statistics_params, rhythm_params, _ = population_fit(df_pop, n_components = n_comps, period = per, **kwargs)
+
+
+                d = {'test': name, 
+                    'period': per,
+                    'n_components': n_comps,
+                    'p': statistics['p'], 
+                    'p_reject': statistics['p_reject'],
+                    'RSS': statistics['RSS'],
+                    'ME': statistics['ME'],
+                    'resid_SE': statistics['resid_SE'],
+                    'amplitude': rhythm_params['amplitude'],
+                    'acrophase': rhythm_params['acrophase'],
+                    'mesor': rhythm_params['mesor']}    
+                
+                
+                ind_params_stats = statistics_params['ind_params_stats'] 
+                for a,b in ind_params_stats.items():
+                    d[a] = b
+
+                df_results = df_add_row(df_results, d)
                 if n_comps == 0:
                     break
     
     df_results.q = multi.multipletests(df_results.p, method = 'fdr_bh')[1]
     df_results.q_reject = multi.multipletests(df_results.p_reject, method = 'fdr_bh')[1]
         
     return df_results
@@ -985,20 +994,26 @@
 
 """
 ******************************
 * start of fitting functions *
 ******************************
 """
     
-def population_fit(df_pop, n_components = 2, period = 24, lin_comp= False, model_type = 'lin', plot = True, plot_measurements=True, plot_individuals=True, plot_margins=True, hold = False, save_to = '', x_label='', y_label='', return_individual_params = False, params_CI = False, samples_per_param_CI=5, max_samples_CI = 1000, sampling_type = "LHS", parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase'], color="black", **kwargs):
+def population_fit(df_pop, n_components = 2, period = 24, lin_comp= False, model_type = 'lin', 
+                   plot = True, plot_measurements=True, plot_individuals=True, plot_margins=True, hold = False, save_to = '', x_label='', y_label='', 
+                   return_individual_params = False, params_CI = False, params_CI_analysis = 'sampling', bootstrap_size = 1000, samples_per_param_CI=5, max_samples_CI = 1000, 
+                   sampling_type = "LHS", parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase'], color="black", **kwargs):    
 
-    if return_individual_params:
-        ind_params = {}
-        for param in parameters_to_analyse:
-            ind_params[param] = []
+    
+
+    #if return_individual_params:
+    ind_params = {}
+    ind_params_stats = {}
+    for param in parameters_to_analyse:
+        ind_params[param] = []
 
         
     params = -1
 
     tests = df_pop.test.unique()
     k = len(tests)
     
@@ -1047,19 +1062,19 @@
         """
 
         results, statistics, rhythm_params, X_test, Y_test, model = fit_me(x, y, n_components = n_components, period = period, plot = False, return_model = True, lin_comp=lin_comp, **kwargs)
         X_fit_eval_params = generate_independents(X_test, n_components = n_components, period = period, lin_comp = lin_comp, remove_lin_comp=True)
         if lin_comp:
             X_fit_eval_params[:,1] = 0    
 
-        if return_individual_params:
-            Y_eval_params = results.predict(X_fit_eval_params)    
-            rhythm_ind_params = evaluate_rhythm_params(X_test, Y_eval_params, period=period)    
-            for param in parameters_to_analyse:
-                ind_params[param].append(rhythm_ind_params[param])
+        #if return_individual_params:
+        Y_eval_params = results.predict(X_fit_eval_params)    
+        rhythm_ind_params = evaluate_rhythm_params(X_test, Y_eval_params, period=period)    
+        for param in parameters_to_analyse:
+            ind_params[param].append(rhythm_ind_params[param])
             
         if (plot and plot_individuals):
             #Y_eval_params = results.predict(X_fit_eval_params)            
             Y_plot_fits = results.predict(X_plot_fits)            
             if (plot and plot_individuals):
                 if not hold:
                     plt.plot(X_plot,Y_plot_fits,color=color, alpha=0.25, label=test)
@@ -1084,38 +1099,68 @@
                 #_, l, u = wls_prediction_std(results, exog=X_fit_eval_params, alpha=0.05)    
                 #lowers = np.vstack([lowers, l])
                 #uppers = np.vstack([uppers, u])
                 Y_plot_fits_all = np.vstack([Y_plot_fits_all, Y_plot_fits])
     
 
 
-    # parameter statistics: means, variances, stadndard deviations, confidence intervals, p-values
+    # parameter statistics: means, variances, standard deviations, confidence intervals, p-values
     #http://reliawiki.com/index.php/Multiple_Linear_Regression_Analysis
     if k > 1:
         means = np.mean(params, axis=0)
         variances = np.sum((params-np.mean(params, axis=0))**2, axis = 0)/(k-1) # np.var(params, axis=0) # isto kot var z ddof=k-1
         sd = variances**0.5
         se = sd/((k-1)**0.5)
         T0 = means/se
         p_values = 2 * (1 - stats.t.cdf(abs(T0), k-1))
         t = abs(stats.t.ppf(0.05/2,df=k-1))
         lower_CI = means - ((t*sd)/((k-1)**0.5))
         upper_CI = means + ((t*sd)/((k-1)**0.5))        
         results.initialize(model, means)
+
+
+        # analysis of amplitude, mesor, acrophase...
+        for ind_param in parameters_to_analyse:
+            ind_vals = np.array(ind_params[ind_param])
+            
+            if ind_param in parameters_angular:
+                p_means = project_acr(circmean(ind_vals, high = np.pi, low = -np.pi))
+                p_sd = circstd(ind_vals, high = np.pi, low = -np.pi)
+            else:
+                p_means = np.mean(ind_vals)
+                p_variances = np.sum((ind_vals-np.mean(ind_vals))**2)/(k-1)
+                p_sd = p_variances**0.5
+            
+            p_se = p_sd/((k-1)**0.5)
+            p_T0 = p_means/p_se
+            ind_param_p = 2 * (1 - stats.t.cdf(abs(p_T0), k-1))
+            t = abs(stats.t.ppf(0.05/2,df=k-1))
+            ind_param_lower_CI = p_means - ((t*p_sd)/((k-1)**0.5))
+            ind_param_upper_CI = p_means + ((t*p_sd)/((k-1)**0.5))        
+           
+            ind_params_stats[f'mean({ind_param})'] = p_means
+            ind_params_stats[f'p({ind_param})'] = ind_param_p
+            ind_params_stats[f'CI({ind_param})'] = [ind_param_lower_CI, ind_param_upper_CI]          
+
     else:
         means = params
         sd = np.zeros(len(params))
         sd[:] = np.nan
         se = np.zeros(len(params))
         se[:] = np.nan
         lower_CI = means
         upper_CI = means
         p_values = np.zeros(len(params))
         p_values[:] = np.nan
 
+        for ind_param in parameters_to_analyse:
+            ind_params_stats[f'mean({ind_param})'] = ind_params[ind_param][0]
+            ind_params_stats[f'p({ind_param})'] = np.nan
+            ind_params_stats[f'CI({ind_param})'] = [np.nan, np.nan_to_num]
+
     x,y = df_pop.x, df_pop.y
     xy = list(zip(x,y))
     xy.sort()
     x,y = zip(*xy)
     x,y = np.array(x), np.array(y)
     X_fit = generate_independents(x, n_components = n_components, period = period, lin_comp = lin_comp)
     Y_fit = results.predict(X_fit)
@@ -1166,37 +1211,43 @@
                 plt.axis([min(min_X,0), 1.1*max(max_X,period), 0.9*min(min_Y, min_Y_test), 1.1*max(max_Y, max_Y_test)])
             else:
                 plt.axis([min(min_X,0), max_X, 0.9*min(min_Y, min_Y_test), 1.1*max(max_Y, max_Y_test)])
             
         else:
             plt.axis([0, period, min_Y_test*0.9, max_Y_test*1.1])
         
-    
+       
+    statistics = calculate_statistics(x, y, Y_fit, n_components, period, lin_comp)   
+    statistics_params = {'values': means,
+                        'SE': se,
+                        'CI': (lower_CI, upper_CI),
+                        'p-values': p_values,
+                        'ind_params_stats': ind_params_stats} 
+
     if plot:
         #pop_name = "_".join(test.split("_")[:-1])
         if not hold:
             plt.title(pop_name + ', p-value=' + "{0:.5f}".format(statistics['p']))
 
             if save_to:
                 plt.savefig(save_to+'.png')
                 plt.savefig(save_to+'.pdf')
                 plt.close()
             else:
                 plt.show()
-    
-    statistics = calculate_statistics(x, y, Y_fit, n_components, period, lin_comp)   
-    statistics_params = {'values': means,
-                        'SE': se,
-                        'CI': (lower_CI, upper_CI),
-                        'p-values': p_values} 
-
 
+    
     if params_CI:
-        population_eval_params_CI(X_test, X_fit_eval_params, results, statistics_params, rhythm_params, samples_per_param=samples_per_param_CI, max_samples = max_samples_CI, k=k, sampling_type=sampling_type, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, period=period)
-
+        if params_CI_analysis == 'bootstrap':
+            ind_params_stats = population_eval_params_bootstrap(X_test, X_fit_eval_params, model, results, params, bootstrap_size=bootstrap_size, bootstrap_type='std', t_test=True, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, period=period)               
+        elif params_CI_analysis == 'sampling':
+            ind_params_stats = population_eval_params_CI(X_test, X_fit_eval_params, results, statistics_params, rhythm_params, samples_per_param=samples_per_param_CI, max_samples = max_samples_CI, k=k, sampling_type=sampling_type, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, period=period)                
+        
+        rhythm_params.update(ind_params_stats)
+        
     if return_individual_params:        
         return params, statistics, statistics_params, rhythm_params, results, ind_params
 
     else:
         return params, statistics, statistics_params, rhythm_params, results
 
 def fit_me(X, Y, n_components = 2, period = 24, lin_comp = False, model_type = 'lin', alpha = 0, name = '', save_to = '', plot=True, plot_residuals=False, plot_measurements=True, plot_margins=True, return_model = False, color = False, plot_phase = True, hold=False, x_label = "", y_label = "", rescale_to_period=False, bootstrap=False, bootstrap_size=1000, bootstrap_type="std", params_CI = False, samples_per_param_CI=5, max_samples_CI = 1000, sampling_type="LHS", parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase']):
@@ -1499,25 +1550,27 @@
 
 # rhythm params
 def evaluate_rhythm_params(X,Y, project_acrophase=True, period=0):
     #plt.plot(X,Y)
     #plt.show()    
 
     m = min(Y)
-    M = max(Y)
+    M = max(Y)    
     A = M - m
     MESOR = m + A/2
     AMPLITUDE = abs(A/2)
     
     PHASE = 0
     PHASE_LOC = 0
         
     H = M - 0.01*M if M >= 0 else M + 0.01*M
     locs, heights = signal.find_peaks(Y, height = H)
     heights = heights['peak_heights'] 
+
+    
     
     if len(locs) >= 2:
         period2 = X[locs[1]] - X[locs[0]]
         period2 = int(round(period2))
     else:
         period2 = np.nan
     
@@ -1531,15 +1584,15 @@
     if period:
         ACROPHASE = phase_to_radians(PHASE, period)
         if project_acrophase:
             ACROPHASE = project_acr(ACROPHASE)
     else:
         ACROPHASE = np.nan
   
-
+    
     # peaks and heights
     #Y = Y[X < 24]
     #X = X[X < 24]
     locs, heights = signal.find_peaks(Y, height = MESOR)
     heights = heights['peak_heights'] 
 
     peaks = X[locs]
@@ -2719,29 +2772,31 @@
         for n_comps in n_components:
             for per in period:      
         
                 df_pop = df[df.test.str.startswith(name)] 
                     
                 if plot and folder:
                     save_to=os.path.join(folder,prefix+name+'_compnts='+str(n_comps) +'_per=' + str(per)) 
+            
 
-                _, statistics, _, rhythm_params, _ = population_fit(df_pop, n_components = n_comps, period = per, plot = plot, save_to = save_to, params_CI = True, **kwargs)  
+                _, statistics, _, rhythm_params, _ = population_fit(df_pop, n_components = n_comps, period = per, plot = plot, save_to = save_to, params_CI = True, parameters_to_analyse=parameters_to_analyse, parameters_angular=parameters_angular, **kwargs)  
                                 
                 row = {'test': name,
                     'period': per,
                     'n_components': n_comps,
                     'p': statistics['p'],
                     'q': np.nan,
                     'p_reject': statistics['p_reject'], 
                     'q_reject': np.nan, 
                     'amplitude': rhythm_params['amplitude'], 
                     'acrophase': rhythm_params['acrophase']}
                 
                 for param in parameters_to_analyse:
                     row[f'{param}'] =  rhythm_params[f'{param}']
+                    #row[f'mean({param})'] =  rhythm_params[f'mean({param})']
                     row[f'CI({param})'] = rhythm_params[f'CI({param})']
                     row[f'p({param})'] = rhythm_params[f'p({param})']
                     row[f'q({param})'] = np.nan   
 
                                    
                 #df_results_extended = df_results_extended.append(row, ignore_index=True, sort=False)
                 df_results_extended = df_add_row(df_results_extended, row)
@@ -2782,15 +2837,15 @@
         n_comps = row[1].n_components
         per = row[1].period
         df_pop = df[df.test.str.startswith(name)] 
                
         if plot and folder:
             save_to=os.path.join(folder,prefix+name+'_compnts='+str(n_comps) +'_per=' + str(per)) 
 
-        _, _, _, rhythm_params, _ = population_fit(df_pop, n_components = n_comps, period = per, plot = plot, save_to = save_to, params_CI = True, **kwargs)  
+        _, _, _, rhythm_params, _ = population_fit(df_pop, n_components = n_comps, period = per, plot = plot, save_to = save_to, params_CI = True, parameters_to_analyse=parameters_to_analyse, parameters_angular=parameters_angular, **kwargs)  
                         
         row = dict(row[1])
         
         for param in parameters_to_analyse:
             row[f'{param}'] =  rhythm_params[f'{param}']
             row[f'CI({param})'] = rhythm_params[f'CI({param})']
             row[f'p({param})'] = rhythm_params[f'p({param})']
@@ -3303,16 +3358,16 @@
         mean_params2 = {}
         ind_params_all = {}
         d_params = {}
         d_params_permute = {}
         # equations below only present an approximation
         for param in parameters_to_analyse:        
             if param in parameters_angular:
-                mean_params1[param] = project_acr(circmean(ind_params1[param], high = 0, low = -2*np.pi))
-                mean_params2[param] = project_acr(circmean(ind_params2[param], high = 0, low = -2*np.pi))
+                mean_params1[param] = project_acr(circmean(ind_params1[param], high = np.pi, low = -np.pi))
+                mean_params2[param] = project_acr(circmean(ind_params2[param], high = np.pi, low = -np.pi))
                 d_params[param] = project_acr(mean_params2[param] - mean_params1[param])
             else:
                 mean_params1[param] = np.mean(ind_params1[param])
                 mean_params2[param] = np.mean(ind_params2[param])
                 d_params[param] = mean_params2[param] - mean_params1[param]
             
             ind_params_all[param] = np.append(ind_params1[param], ind_params2[param])                  
@@ -3336,16 +3391,16 @@
         
         for perm1, perm2 in permutations:
             perm1 = np.array(perm1)
             perm2 = np.array(perm2)
 
             for param in parameters_to_analyse:     
                 if param in parameters_angular:
-                    test1 = project_acr(circmean(ind_params_all[param][perm1], high = 0, low = -2*np.pi))
-                    test2 = project_acr(circmean(ind_params_all[param][perm2], high = 0, low = -2*np.pi))
+                    test1 = project_acr(circmean(ind_params_all[param][perm1], high = np.pi, low = -np.pi))
+                    test2 = project_acr(circmean(ind_params_all[param][perm2], high = np.pi, low = -np.pi))
                     d_test = project_acr(test2 - test1)
                 else:
                     test1 = np.mean(ind_params_all[param][perm1])
                     test2 = np.mean(ind_params_all[param][perm2])
                     d_test = test2 - test1
 
                 d_params_permute[param].append(d_test)
@@ -3847,18 +3902,83 @@
         if t_test:
             rhythm_params[f'p(d_{param})'] = get_p_t_test(mean_params[param], se_param, DoF)            
         else:
             rhythm_params[f'p(d_{param})'] = get_p_z_test(mean_params[param], se_param) 
 
     return rhythm_params
 
+# eval parameters using bootstrap
+# bootstrap type should be set to either std (CI = X+-1.96*STD(X)) or percentile (CI = [2.5th percentile, 97.5th percentile])
+def population_eval_params_bootstrap(X_test, X_fit_eval_params, model, results, model_params, bootstrap_size=100, bootstrap_type='std', t_test=True, parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase'], period=24):           
+    
+    model_bs = copy.deepcopy(model) # precaution
+    results_bs = copy.deepcopy(results) # precaution
+        
+    # generate and evaluate bootstrap samples
+    params_bs = {}
+    for param in parameters_to_analyse:
+        params_bs[param] = np.zeros(bootstrap_size)
+        
+    n_models = model_params.shape[0] # number of models
+    n_params  = model_params.shape[1] # number of model params
+
+    for i in range(bootstrap_size):
+
+        idxs = np.random.choice(n_models, n_models)
+
+        model_params_sample = model_params[idxs,:] #resampling
+                
+        params_means = np.mean(model_params_sample, axis=0)
+        results_bs.initialize(model_bs, params_means)
+                
+        Y_eval_params = results_bs.predict(X_fit_eval_params) 
+        rhythm_params = evaluate_rhythm_params(X_test, Y_eval_params, period=period)
+        
+
+        for param in parameters_to_analyse:
+            params_bs[param][i] = rhythm_params[param]
+
+
+        """
+        # remove the fits that exhibit divergence
+        for param in parameters_to_analyse:
+            if (abs(rhythm_params_bs['amplitude']) > (np.max(Y)-np.min(Y))) or ((rhythm_params_bs['period2']) and (rhythm_params_bs['period2'] < rhythm_params_bs['period2'])):
+                params_bs[param][i] = np.nan                         
+            else:    
+                #plt.plot(X_test, Y_eval_params_bs, alpha=0.5)
+                params_bs[param][i] = rhythm_params_bs[param]                 
+        """
+
+    #print(params_bs)
+
+    # analyse bootstrap samples
+    DoF = bootstrap_size - n_params    
+    rhythm_params['DoF'] = DoF    
+
+    for param in parameters_to_analyse:
+        if param in parameters_angular:
+            angular = True
+        else:
+            angular = False
+    
+        sample_bs = params_bs[param]
+        mean, p_val, CI = bootstrap_statistics(sample_bs, angular=angular, bootstrap_type = bootstrap_type, t_test= t_test, n_params=n_params)
+
+        rhythm_params[f'{param}_bootstrap'] = mean
+        rhythm_params[f'CI({param})'] = CI
+        rhythm_params[f'p({param})'] = p_val
+    
+    return rhythm_params
+
+
 
 # sample the parameters from the confidence interval, builds a set of models and assesses the rhythmicity parameters confidence intervals   
 def population_eval_params_CI(X_test, X_fit_eval_params, results, statistics_params, rhythm_params, parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase'], samples_per_param=5, max_samples = 1000, t_test = True, k=0, sampling_type="LHS", period=24): 
     res2 = copy.deepcopy(results)
+    rhythm_params = copy.deepcopy(rhythm_params)
     params = res2.params    
     DoF = k-1
     rhythm_params['DoF'] = DoF
     CIs = statistics_params['CI']
     CIs = list(zip(*CIs))
                 
     P = np.zeros((len(params), samples_per_param))
@@ -3928,18 +4048,19 @@
     for param in parameters_to_analyse:
         se_param = dev_params[param]/t   
         if t_test:
             rhythm_params[f'p({param})'] = get_p_t_test(mean_params[param], se_param, DoF)            
         else:
             rhythm_params[f'p({param})'] = get_p_z_test(mean_params[param], se_param)            
         
+    #print(rhythm_params)
     return rhythm_params
 
 # compare two population fit pairs independently
-def compare_pair_population_CI(df, test1, test2, n_components = 1, period = 24, n_components2 = None, period2 = None, parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase'], samples_per_param_CI=5, max_samples_CI = 1000, t_test = True, sampling_type = "LHS", single_params = {}, **kwargs):
+def compare_pair_population_CI(df, test1, test2, n_components = 1, period = 24, n_components2 = None, period2 = None, parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase'], single_params = {}, t_test = True, **kwargs):
       
     rhythm_params = {}
 
     n_components1 = n_components
     period1 = period
     if not n_components2:
         n_components2 = n_components1
@@ -3950,16 +4071,16 @@
     df_pop2 = df[df.test.str.startswith(test2)] 
 
     if single_params:
         run_params_CI = False # fit_me is called without sampling
     else:
         run_params_CI = True # fit_me is called with sampling
 
-    _, statistics1, _, rhythm_params1, _ = population_fit(df_pop1, n_components = n_components1, period = period1, plot = False,plot_measurements=False, plot_individuals=False, plot_margins=False, params_CI = run_params_CI, samples_per_param_CI = samples_per_param_CI, max_samples_CI=max_samples_CI, sampling_type = sampling_type, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, **kwargs)
-    _, statistics2, _, rhythm_params2, _ = population_fit(df_pop2, n_components = n_components2, period = period2, plot = False, plot_measurements=False, plot_individuals=False, plot_margins=False, params_CI = run_params_CI, samples_per_param_CI = samples_per_param_CI, max_samples_CI=max_samples_CI, sampling_type = sampling_type, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, **kwargs)
+    _, statistics1, _, rhythm_params1, _ = population_fit(df_pop1, n_components = n_components1, period = period1, plot = False,plot_measurements=False, plot_individuals=False, plot_margins=False, params_CI = run_params_CI, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, **kwargs)
+    _, statistics2, _, rhythm_params2, _ = population_fit(df_pop2, n_components = n_components2, period = period2, plot = False, plot_measurements=False, plot_individuals=False, plot_margins=False, params_CI = run_params_CI, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, **kwargs)
 
     rhythm_params['rhythm_params1'] = rhythm_params1
     rhythm_params['rhythm_params2'] = rhythm_params2
 
     rhythm_params['statistics1'] = statistics1
     rhythm_params['statistics2'] = statistics2
 
@@ -4020,14 +4141,98 @@
             rhythm_params[f'p(d_{param})'] = get_p_t_test(d_param, se_param, DoF)
         else:
             rhythm_params[f'p(d_{param})'] = get_p_z_test(d_param, se_param)
     
     return rhythm_params
 
 
+# compare two population fit pairs independently - new variant that calculates CI amplitudes, CI acrophases etc. from individual models
+def compare_pair_population_CI_new(df, test1, test2, n_components = 1, period = 24, n_components2 = None, period2 = None, parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase'], t_test = True, **kwargs):
+      
+    rhythm_params = {}
+
+    n_components1 = n_components
+    period1 = period
+    if not n_components2:
+        n_components2 = n_components1
+    if not period2:
+        period2 = period1
+            
+    df_pop1 = df[df.test.str.startswith(test1)] 
+    df_pop2 = df[df.test.str.startswith(test2)] 
+
+    _, statistics1, statistics_params1, rhythm_params1, _ = population_fit(df_pop1, n_components = n_components1, period = period1, plot = False,plot_measurements=False, plot_individuals=False, plot_margins=False, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, **kwargs)
+    _, statistics2, statistics_params2, rhythm_params2, _ = population_fit(df_pop2, n_components = n_components2, period = period2, plot = False, plot_measurements=False, plot_individuals=False, plot_margins=False, parameters_to_analyse = parameters_to_analyse, parameters_angular = parameters_angular, **kwargs)
+
+    rhythm_params['rhythm_params1'] = rhythm_params1
+    rhythm_params['rhythm_params2'] = rhythm_params2
+
+    rhythm_params['statistics1'] = statistics1
+    rhythm_params['statistics2'] = statistics2
+
+    #p1 = statistics1['p']
+    #p2 = statistics2['p']
+
+    #if p1 > 0.05 or p2 > 0.05:
+    #    print("rhythmicity in one is not significant")
+    #    #return
+
+    d_params = {}
+    
+    for param in parameters_to_analyse:        
+
+        rhythm_params1[param] = statistics_params1['ind_params_stats'][f'mean({param})'] #override the joint cosinor model
+        rhythm_params2[param] = statistics_params2['ind_params_stats'][f'mean({param})'] #override the joint cosinor model
+
+        d_params[param] = rhythm_params2[param] - rhythm_params1[param]
+        if param in parameters_angular:
+            d_params[param] = project_acr(d_params[param])        
+    
+    CI1 = {}
+    CI2 = {}
+    for param in parameters_to_analyse:            
+        CI1[param] = statistics_params1['ind_params_stats'][f'CI({param})']
+        CI2[param] = statistics_params2['ind_params_stats'][f'CI({param})']
+        
+
+    # DoF
+    k1 = len(df_pop1.test.unique())
+    k2 = len(df_pop2.test.unique()) 
+    k = len(df_pop1.test.unique()) + len(df_pop2.test.unique()) 
+    DoF = k - 2
+    DoF1 = k1 - 1
+    DoF2 = k2 - 1
+    rhythm_params['DoF'] = DoF
+
+    # statistics
+    if t_test:
+        t = abs(stats.t.ppf(0.05/2,df=DoF)) 
+    else:
+        t = 1.96
+
+    for param in parameters_to_analyse:        
+        angular = True if param in parameters_angular else False
+        se_param = get_se_diff_from_CIs(CI1[param], CI2[param], DoF1, DoF2, t_test = t_test, angular=angular, CI_type = "se", n1 = k1, n2 = k2, DoF = DoF) 
+        d_param = d_params[param]
+
+        rhythm_params[f'd_{param}'] = d_param
+
+        if param in parameters_angular:
+            rhythm_params[f'CI(d_{param})'] =  get_acrophase_CI(d_param, t*se_param)
+        else:
+            rhythm_params[f'CI(d_{param})'] = [d_param - t*se_param, d_param + t*se_param]        
+  
+        if t_test:
+            rhythm_params[f'p(d_{param})'] = get_p_t_test(d_param, se_param, DoF)
+        else:
+            rhythm_params[f'p(d_{param})'] = get_p_z_test(d_param, se_param)
+    
+    return rhythm_params
+
+
 # compare two pairs independently
 def compare_pair_CI(df, test1, test2, n_components = 1, period = 24, n_components2 = None, period2 = None, parameters_to_analyse = ['amplitude', 'acrophase', 'mesor'], parameters_angular = ['acrophase'], samples_per_param_CI=5, max_samples_CI = 1000, t_test = True, sampling_type="LHS", rhythm_params = {}, single_params = {}, **kwargs):    
     
     n_components1 = n_components
     period1 = period
     if not n_components2:
         n_components2 = n_components1
@@ -4314,16 +4519,16 @@
         n_devs = 1.96
 
 
     # SE or STD?
     # https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1255808/
     # https://ocw.mit.edu/courses/mathematics/18-05-introduction-to-probability-and-statistics-spring-2014/readings/MIT18_05S14_Reading24.pdf
     if angular:
-        mean = project_acr(circmean(sample_bs, high = 0, low = -2*np.pi))
-        std = circstd(sample_bs, high = 0, low = -2*np.pi)
+        mean = project_acr(circmean(sample_bs, high = np.pi, low = -np.pi))
+        std = circstd(sample_bs, high = np.pi, low = -np.pi)
 
         if bootstrap_type == "se":
             se = std/(len(sample_bs)-1)**0.5
             #se_params[param] = std_phase/(len(phases))**0.5
         elif bootstrap_type == "std":
             se = std
         elif bootstrap_type == "percentile":
```

### Comparing `CosinorPy-3.0/CosinorPy/cosinor1.py` & `CosinorPy-3.1/CosinorPy/cosinor1.py`

 * *Files identical despite different names*

### Comparing `CosinorPy-3.0/CosinorPy/cosinor_nonlin.py` & `CosinorPy-3.1/CosinorPy/cosinor_nonlin.py`

 * *Files identical despite different names*

### Comparing `CosinorPy-3.0/CosinorPy/file_parser.py` & `CosinorPy-3.1/CosinorPy/file_parser.py`

 * *Files identical despite different names*

### Comparing `CosinorPy-3.0/PKG-INFO` & `CosinorPy-3.1/CosinorPy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: CosinorPy
-Version: 3.0
+Version: 3.1
 Summary: Python package for cosinor based rhytmometry
 Home-page: https://github.com/mmoskon/CosinorPy
+Download-URL: https://github.com/mmoskon/CosinorPy/archive/v3.1.tar.gz
 Author: Miha Moskon
 Author-email: miha.moskon@fri.uni-lj.si
 License: MIT
-Download-URL: https://github.com/mmoskon/CosinorPy/archive/v3.0.tar.gz
-Description: UNKNOWN
 Keywords: cosinor,rhytmometry,regression,bioinformatics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE.txt
```

### Comparing `CosinorPy-3.0/setup.py` & `CosinorPy-3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'CosinorPy',
   packages = ['CosinorPy'],  
-  version = '3.0',      
+  version = '3.1',      
   license='MIT',        
   description = 'Python package for cosinor based rhytmometry',   
   author = 'Miha Moskon',                   
   author_email = 'miha.moskon@fri.uni-lj.si',      
   url = 'https://github.com/mmoskon/CosinorPy',   
-  download_url = 'https://github.com/mmoskon/CosinorPy/archive/v3.0.tar.gz',  
+  download_url = 'https://github.com/mmoskon/CosinorPy/archive/v3.1.tar.gz',  
   keywords = ['cosinor', 'rhytmometry', 'regression', 'bioinformatics'],  
   install_requires=[            
           'pandas',
           'numpy',
           'matplotlib',
           'statsmodels',
           'scipy',
```

