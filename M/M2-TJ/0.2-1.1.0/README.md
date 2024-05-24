# Comparing `tmp/M2_TJ-0.2.tar.gz` & `tmp/m2_tj-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/charles/Python/ForGitHub/M2_TJ/dist/.tmp-6m5ewjwq/M2_TJ-0.2.tar", last modified: Tue Mar 12 14:19:51 2024, max compression
+gzip compressed data, was "/home/charles/Python/ForGitHub/M2_TJ/dist/.tmp-sw1o0sxp/m2_tj-1.1.0.tar", last modified: Fri May 24 12:47:32 2024, max compression
```

## Comparing `M2_TJ-0.2.tar` & `m2_tj-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-12 14:19:51.932691 M2_TJ-0.2/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1071 2024-02-02 14:25:43.000000 M2_TJ-0.2/LICENSE
--rw-rw-r--   0 charles   (1000) charles   (1000)       33 2024-02-26 23:26:03.000000 M2_TJ-0.2/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)     1014 2024-03-12 14:19:51.932691 M2_TJ-0.2/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      191 2024-03-12 01:45:58.000000 M2_TJ-0.2/README.md
--rw-rw-r--   0 charles   (1000) charles   (1000)      742 2024-02-26 21:40:03.000000 M2_TJ-0.2/pyproject.toml
--rw-rw-r--   0 charles   (1000) charles   (1000)      990 2024-03-12 14:19:51.932691 M2_TJ-0.2/setup.cfg
--rw-rw-r--   0 charles   (1000) charles   (1000)       69 2024-02-02 02:19:36.000000 M2_TJ-0.2/setup.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-12 14:19:51.928691 M2_TJ-0.2/src/
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-12 14:19:51.928691 M2_TJ-0.2/src/M2_ProposalTools/
--rw-rw-r--   0 charles   (1000) charles   (1000)    13030 2024-02-29 00:53:44.000000 M2_TJ-0.2/src/M2_ProposalTools/FilterImages.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    31227 2024-03-12 02:39:06.000000 M2_TJ-0.2/src/M2_ProposalTools/MakeRMSmap.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    43928 2024-03-12 13:46:15.000000 M2_TJ-0.2/src/M2_ProposalTools/ModelFitting.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    53946 2024-03-06 17:48:16.000000 M2_TJ-0.2/src/M2_ProposalTools/WorkHorse.py
--rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-02-02 02:19:36.000000 M2_TJ-0.2/src/M2_ProposalTools/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    49953 2024-02-29 17:47:00.000000 M2_TJ-0.2/src/M2_ProposalTools/analytic_integrations.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     7509 2024-02-27 21:02:37.000000 M2_TJ-0.2/src/M2_ProposalTools/numerical_integration.py
--rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-02-02 02:19:36.000000 M2_TJ-0.2/src/M2_ProposalTools/py.typed
--rw-rw-r--   0 charles   (1000) charles   (1000)     3538 2024-02-23 22:17:00.000000 M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_2p5_21Aonly_PCA5_0f08Filtering.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)     3660 2024-02-29 02:44:12.000000 M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_3p0_21Aonly_PCA5_0f08Filtering.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)     3660 2024-02-29 02:44:10.000000 M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_3p5_21Aonly_PCA5_0f08Filtering.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)     3660 2024-02-29 02:35:56.000000 M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_4p0_21Aonly_PCA5_0f08Filtering.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)     3721 2024-02-29 02:37:29.000000 M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_4p5_21Aonly_PCA5_0f08Filtering.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)     3721 2024-02-29 02:38:54.000000 M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_5p0_21Aonly_PCA5_0f08Filtering.txt
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-12 14:19:51.928691 M2_TJ-0.2/src/M2_TJ.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)     1014 2024-03-12 14:19:51.000000 M2_TJ-0.2/src/M2_TJ.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)     1008 2024-03-12 14:19:51.000000 M2_TJ-0.2/src/M2_TJ.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2024-03-12 14:19:51.000000 M2_TJ-0.2/src/M2_TJ.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2024-02-02 18:39:44.000000 M2_TJ-0.2/src/M2_TJ.egg-info/not-zip-safe
--rw-rw-r--   0 charles   (1000) charles   (1000)      164 2024-03-12 14:19:51.000000 M2_TJ-0.2/src/M2_TJ.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       17 2024-03-12 14:19:51.000000 M2_TJ-0.2/src/M2_TJ.egg-info/top_level.txt
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-12 14:19:51.928691 M2_TJ-0.2/tests/
--rw-rw-r--   0 charles   (1000) charles   (1000)     4500 2024-02-27 22:42:39.000000 M2_TJ-0.2/tests/test_M2_ProposalTools.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-05-24 12:47:32.642592 m2_tj-1.1.0/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1071 2024-02-02 14:25:43.000000 m2_tj-1.1.0/LICENSE
+-rw-rw-r--   0 charles   (1000) charles   (1000)       33 2024-02-26 23:26:03.000000 m2_tj-1.1.0/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)     1248 2024-05-24 12:47:32.642592 m2_tj-1.1.0/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)      191 2024-03-12 01:45:58.000000 m2_tj-1.1.0/README.md
+-rw-rw-r--   0 charles   (1000) charles   (1000)      742 2024-02-26 21:40:03.000000 m2_tj-1.1.0/pyproject.toml
+-rw-rw-r--   0 charles   (1000) charles   (1000)      992 2024-05-24 12:47:32.642592 m2_tj-1.1.0/setup.cfg
+-rw-rw-r--   0 charles   (1000) charles   (1000)      328 2024-05-24 12:47:01.000000 m2_tj-1.1.0/setup.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-05-24 12:47:32.634592 m2_tj-1.1.0/src/
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-05-24 12:47:32.638592 m2_tj-1.1.0/src/M2_ProposalTools/
+-rw-rw-r--   0 charles   (1000) charles   (1000)    13064 2024-05-06 14:42:14.000000 m2_tj-1.1.0/src/M2_ProposalTools/FilterImages.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    31630 2024-05-24 09:53:39.000000 m2_tj-1.1.0/src/M2_ProposalTools/MakeRMSmap.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    44773 2024-05-24 12:05:32.000000 m2_tj-1.1.0/src/M2_ProposalTools/ModelFitting.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    56971 2024-05-24 10:09:41.000000 m2_tj-1.1.0/src/M2_ProposalTools/WorkHorse.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-02-02 02:19:36.000000 m2_tj-1.1.0/src/M2_ProposalTools/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    50507 2024-05-24 08:17:17.000000 m2_tj-1.1.0/src/M2_ProposalTools/analytic_integrations.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     7509 2024-02-27 21:02:37.000000 m2_tj-1.1.0/src/M2_ProposalTools/numerical_integration.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-02-02 02:19:36.000000 m2_tj-1.1.0/src/M2_ProposalTools/py.typed
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3538 2024-02-23 22:17:00.000000 m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_2p5_21Aonly_PCA5_0f08Filtering.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3660 2024-02-29 02:44:12.000000 m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_3p0_21Aonly_PCA5_0f08Filtering.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3660 2024-02-29 02:44:10.000000 m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_3p5_21Aonly_PCA5_0f08Filtering.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3660 2024-02-29 02:35:56.000000 m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_4p0_21Aonly_PCA5_0f08Filtering.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3721 2024-02-29 02:37:29.000000 m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_4p5_21Aonly_PCA5_0f08Filtering.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3721 2024-02-29 02:38:54.000000 m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_5p0_21Aonly_PCA5_0f08Filtering.txt
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-05-24 12:47:32.642592 m2_tj-1.1.0/src/M2_TJ.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)     1248 2024-05-24 12:47:32.000000 m2_tj-1.1.0/src/M2_TJ.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1008 2024-05-24 12:47:32.000000 m2_tj-1.1.0/src/M2_TJ.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2024-05-24 12:47:32.000000 m2_tj-1.1.0/src/M2_TJ.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2024-02-02 18:39:44.000000 m2_tj-1.1.0/src/M2_TJ.egg-info/not-zip-safe
+-rw-rw-r--   0 charles   (1000) charles   (1000)      164 2024-05-24 12:47:32.000000 m2_tj-1.1.0/src/M2_TJ.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       17 2024-05-24 12:47:32.000000 m2_tj-1.1.0/src/M2_TJ.egg-info/top_level.txt
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-05-24 12:47:32.642592 m2_tj-1.1.0/tests/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     6770 2024-05-24 10:21:54.000000 m2_tj-1.1.0/tests/test_M2_ProposalTools.py
```

### Comparing `M2_TJ-0.2/LICENSE` & `m2_tj-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/pyproject.toml` & `m2_tj-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/setup.cfg` & `m2_tj-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = M2_TJ
 description = Functions for technical justification
 author = Charles Romero
-version = 0.2
+version = 1.1.0
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
```

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/FilterImages.py` & `m2_tj-1.1.0/src/M2_ProposalTools/FilterImages.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
            frequency vector
     """
     kx =  np.outer(np.fft.fftfreq(nx),np.zeros(ny).T+1.0)/psx
     ky =  np.outer(np.zeros(nx).T+1.0,np.fft.fftfreq(ny))/psy
     k = np.sqrt(kx*kx + ky*ky)
     return k
 
-def power_spectrum_2d(arr,nbins=10,psx=1,psy=1,logbins=0):
+def power_spectrum_2d(arr,nbins=10,psx=1,psy=1,logbins=False):
     """
     Compute 2D power spectrum of arr
     
     Parameters
     ----------
     arr: float 2D numpy array
          2D array for which we compute the power spectrum
@@ -56,18 +56,18 @@
     else:
         kbinarr = np.arange(nbins+1)/np.double(nbins)*(k.max()-k.min())
     kbin   = np.zeros(nbins+1)
     pkbin  = np.zeros(nbins+1)
     pkbins = np.zeros(nbins+1)
 
     for idx in range(0,nbins):
-        list = np.nonzero((k > kbinarr[idx]) * (k<= kbinarr[idx+1]))
-        kbin[idx+1] = np.median(k[list])
-        pkbin[idx+1] = np.mean(pk[list])
-        pkbins[idx+1] = np.std(pk[list])/np.sqrt(len(list[0]))
+        mylist        = np.nonzero((k > kbinarr[idx]) * (k<= kbinarr[idx+1]))
+        kbin[idx+1]   = np.median(k[mylist])
+        pkbin[idx+1]  = np.mean(pk[mylist])
+        pkbins[idx+1] = np.std(pk[mylist])/np.sqrt(len(mylist[0]))
     return kbin,pkbin,pkbins
 
 def cross_power_spectrum_2d(arr,arr1,nbins=10,psx=1.0,psy=1.0,logbins=False):
     """
     Compute 2D cross-power spectrum of arr and arr1
     
     Parameters
@@ -102,18 +102,18 @@
                 kbinarr = np.logspace(0.0,np.log(k.max()),nbins+1) 
             else:
                 kbinarr = np.arange(nbins+1)/np.double(nbins)*(k.max()-k.min())
             kbin = np.zeros(nbins+1)
             pkbin = np.zeros(nbins+1)
             pkbins = np.zeros(nbins+1)
             for idx in range(0,nbins):
-                list = np.nonzero((k > kbinarr[idx]) * (k<= kbinarr[idx+1]))
-                kbin[idx+1] = np.median(k[list])
-                pkbin[idx+1] = np.mean(pk[list])
-                pkbins[idx+1] = np.std(pk[list])/np.sqrt(len(list[0]))
+                mylist = np.nonzero((k > kbinarr[idx]) * (k<= kbinarr[idx+1]))
+                kbin[idx+1] = np.median(k[mylist])
+                pkbin[idx+1] = np.mean(pk[mylist])
+                pkbins[idx+1] = np.std(pk[mylist])/np.sqrt(len(mylist[0]))
     return kbin,pkbin,pkbins
 
 def fourier_conv_2d(arr,kernel):
     """
     From JMP; perform convolution, i.e. (arr * kernel)
     
     Parameters
```

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/MakeRMSmap.py` & `m2_tj-1.1.0/src/M2_ProposalTools/MakeRMSmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
-from matplotlib import cm
+#from matplotlib import cm
+from matplotlib import colormaps
 from reproject import reproject_interp
 from astropy.wcs import WCS
 from astropy.io import fits
 import scipy.ndimage
 
 def get_rms_cmap():
     """
     Tiny function to get a colormap with desired indexing, and importantly make values above or below it white.
 
     :return: colormap
     :rtype: object
     """
-    mycmap=cm.get_cmap('tab20b').copy()
-    mydcm=cm.get_cmap('tab20b',256)
-    newcolors = mydcm(np.linspace(0,1,256))
+    #mycmap=cm.get_cmap('tab20b').copy()
+    #mydcm=cm.get_cmap('tab20b',256)
+    mycmap=colormaps['tab20b'].copy()
+    #mydcm = colormaps['tab20b']
+    #newcolors = mydcm(np.linspace(0,1,256))
     mycmap.set_under('w')
     mycmap.set_over('w')
     
     return mycmap
 
 def conv_wtmap_torms(wtmap):
 
@@ -493,17 +496,28 @@
 
     if WIKID:
         #print(p)
         p[0] = p[0]/10.0
         p[1] = p[1]/2.0
         p[2] = p[2]*2.0
         p[3] = p[3]/2.0
+        if size == 2.5:
+            p = [2.9*3.3,0.26]
+        if size == 3.0:
+            p = [3.1*3.3,0.26]
         if size == 3.5:
             #print("Heya")
-            p = [11.2, 0.2]
+            p = [3.4*3.3, 0.18]
+        if size == 4.0:
+            p = [3.85*3.3,0.17]
+        if size == 4.5:
+            p - [4.2*3.3,0.128]
+        if size == 5.0:
+            p - [5.02*3.3,0.12]
+            
         #print(p)
         ### To be confirmed
 
     return p
         
 def make_rmap(xymap):
     """
```

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/ModelFitting.py` & `m2_tj-1.1.0/src/M2_ProposalTools/ModelFitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import scipy.special as scs
 import M2_ProposalTools.FilterImages as FI
 
 WH=reload(WH)
     
 
 def fit_spherical_model(z,M500,hdul,model="NP",pink=True,alpha=2,knee=1.0/120.0,nkbin=100,fwhm=9.0,nsteps=1000,
-                        y2k=-3.4,uKinput=True,ySph=True,YMrel="A10",outdir="/home/data/",outbase="NP_fit_corner.png",
-                        size=3.5,Dist=False,plotPin=True,adPhys=True,WIKID=False):
+                        y2k=-3.4,uKinput=True,ySph=True,YMrel="A10",outdir="/tmp/",outbase="NP_fit_corner.png",
+                        size=3.5,Dist=False,plotPin=True,adPhys=True,WIKID=False,fit_cen=True,addNoise=True):
 
     """
     :param z: Redshift
     :type z: float
     :param M500: :math:`M\_{500}`
     :type M500: quantity (mass units)
     :param hdul: Astropy/fits HDU list (Make sure wtmap and img have appropriate units)
@@ -50,38 +50,51 @@
     :type YMrel: str
     :param outdir: A string indicating the output directory, including trailing "/".
     :type outdir: str
     :param outbase: filename, without the directory path.
     :type outbase: str
     :param size: size of Lissajous daisy scan used (for transfer function). Options are 2.5, 3.0, 3.5, 4.0, 4.5, or 5.0
     :type size: float.
+    :param fit_cen: Fit for a center? Default is True
+    :type fit_cen: bool
     
     """
 
     ### First, we need to establish the radius out to which we fit and how many bins we want.
     ### This relies on how good our data are.
     
     conv         = 1e-6/y2k if uKinput else 1.0/y2k 
     sf           = WH.get_smoothing_factor(fwhm=fwhm)
-    hdul[0].data = hdul[0].data*conv
-    hdul[1].data = hdul[1].data / ( conv**2 )
+    if addNoise:
+        hdul[0].data = hdul[0].data*conv
+        hdul[1].data = hdul[1].data / ( conv**2 )
+    else:
+        pixsize      = WH.get_pixarcsec(hdul)
+        SigImg       = FI.fourier_filtering_2d(hdu[0].data,"gauss",fwhm/pixsize)
+        SigWts       = FI.fourier_filtering_2d(hdu[1].data,"gauss",fwhm/pixsize)
+        SigWts      *= (sf/pixsize)**2
+        hdul[0].data = SigImg*1.0
+        hdul[1].data = SigWts*1.0
     SNRmap       = WH.get_SNR_map(hdul)
     SNRhdu       = fits.PrimaryHDU(SNRmap,header=hdul[0].header)
     SNRhdu.writeto(outdir+"SNRmap.fits",overwrite=True)
     CosmoPars    = WH.get_cosmo_pars(z)
     pixsize      = WH.get_pixarcsec(hdul)
     intSNR,xc,yc,xymap = get_int_SNR(SNRmap,pixsize,maxRad=2.0,bv=120.0,SNRthresh=1.0)
 
-    Noise        = WH.get_noise_realization(hdul,pink=pink,alpha=alpha,knee=knee,nkbin=nkbin,fwhm=fwhm)
+    if addNoise:
+        Noise        = WH.get_noise_realization(hdul,pink=pink,alpha=alpha,knee=knee,nkbin=nkbin,fwhm=fwhm)
+    else:
+        Noise        = np.zeros(hdul[0].data.shape)
     # Modify HDU list to have mock-data and correctly weighted pixels.
     # Want to work in Compton y for fitting.
 
     ###############################################################################################
 
-    efv        = get_emcee_fit_vars(CosmoPars,M500,intSNR,xc,yc,pixsize,outdir,
+    efv        = get_emcee_fit_vars(CosmoPars,M500,intSNR,xc,yc,pixsize,outdir,fit_cen=fit_cen,
                                     MinRes=pixsize/2.0,model=model,ySph=ySph,YMrel=YMrel,size=size,
                                     Dist=Dist,WIKID=WIKID)
     mask         = automated_mask(xymap,CosmoPars,efv)
 
     hdul[0].data = hdul[0].data + Noise
     hdul[1].data = hdul[1].data*mask / ( sf**2 )
 
@@ -386,14 +399,16 @@
     OutHDU1 = fits.PrimaryHDU(outmap,header=hdul[0].header)
     OutHDU2 = fits.ImageHDU(model,header=hdul[1].header)
     OutHDU  = fits.HDUList([OutHDU1,OutHDU2])
     OutName = "FittedModel_"+efv["Mstr"]+"_"+efv["zstr"]+"_"+repr(efv["nsteps"])+"steps.fits"
     OutHDU.writeto(efv["outdir"]+OutName,overwrite=True)
 
     m500_res = np.abs(np.array([m500v,m_unc_values[0],m_unc_values[1]])) * 1e14
+    if np.any(np.isnan(m500_res)) or np.any(np.isinf(m500_res)):
+         m500_res = np.ones(3)*1e10
     plot_pressure_profiles(mysolns,efv,cosmo_pars,m500_res,plotPin=plotPin,adPhys=adPhys)
 
 def plot_pressure_profiles(solns,efv,cosmo_pars,m500,myfs=10,plotPin=True,adPhys=True):
 
     """
     For now, assuming model == "NP"... need to add others
 
@@ -805,15 +820,15 @@
     xinit   = np.asarray(xymap)
     grads   = (rmap < maxRad*60.0)
     xdata   = xinit[:,grads]
     ydata   = SNRflat[grads]
     #p0      = np.array([x0,y0,amplitude,sigma,mnlvl])
     xshift  = 1.0  # As a guess
     yshift  = 1.0  # in arcseconds
-    sigma   = 10.0 # Gaussian sigma, in arcseconds
+    sigma   = 20.0 # Gaussian sigma, in arcseconds
     mnlvl   = 1e-2 # Plausible, for an SNR map
     p0      = np.array([xshift,yshift,maxSNR,sigma,mnlvl])
     
     popt, pcov = curve_fit(circ_Gauss, xdata, ydata,p0=p0)
 
     return popt,pcov,xc,yc
     
@@ -1014,20 +1029,27 @@
     :param cal: calibration error. Default is None
     :type cal: float
     """
 
     mypow = np.floor(np.log10(med))
     myexp = 10.0**mypow
 
-    if mypow > 0:
-        psign = '+'
-        pStr = psign+str(int(mypow))
+    if np.isfinite(mypow):
+        if mypow > 0:
+            psign = '+'
+            pStr = psign+str(int(mypow))
+        else:
+            pStr = str(int(mypow))
     else:
+        # This captures an exceptional case.
+        print(med)
+        mypow = 0.0
+        myexp = 1.0
         pStr = str(int(mypow))
-        
+            
     msig  = med/myexp
     hsig  = high_err/myexp
     lsig  = low_err/myexp
 
     
     msStr = "{:.2F}".format(msig)
     hsStr = '+'+"{:.2F}".format(hsig)
```

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/WorkHorse.py` & `m2_tj-1.1.0/src/M2_ProposalTools/WorkHorse.py`

 * *Files 7% similar despite different names*

```diff
@@ -423,15 +423,15 @@
        A map of radii
     """
 
     rmap = np.sqrt(xymap[0]**2 + xymap[1]**2)
 
     return rmap
 
-def make_a10_map(M500,z,xymap,Theta500,nx,ny,nb_theta_range=150,Dist=False):
+def make_a10_map(M500,z,xymap,Theta500,nx,ny,nb_theta_range=150,Dist=False,c500=None,p=None,a=None,b=None,c=None):
     """
     Return a tuple of x- and y-coordinates.
 
     Parameters
     ----------
     M500 : quantity
        :math:`M\_{500}` with units of mass.
@@ -445,28 +445,38 @@
        Number of pixels along axis 0
     ny : int
        Number of pixels along axis 1
     nb_theta_range : int
        Number of elements in an array of radii.
     Dist : bool
        Assume a disturbed A10 profile? Default is False
+    c500 : float, none-type
+      If None, adopts the radius scaling value for A10 (full or disturbed) sample
+    p : float, none-type
+      If None, adopts the normalization value for A10 (full or disturbed) sample
+    a : float, none-type
+      If None, adopts the alpha value for A10 (full or disturbed) sample
+    b : float, none-type
+      If None, adopts the beta value for A10 (full or disturbed) sample
+    c : float, none-type
+      If None, adopts the gamma value for A10 (full or disturbed) sample
 
     Returns
     -------
     ymap : class:`numpy.ndarray`
        An output Compton y map
 
     """
 
     minpixrad = (1.0*u.arcsec).to('rad')
     tnx       = [minpixrad.value,10.0*Theta500]  # In radians
     thetas    = np.logspace(np.log10(tnx[0]),np.log10(tnx[1]), nb_theta_range)
     d_ang     = get_d_ang(z)
     radkpc    = thetas*d_ang.to("kpc")
-    PresProf  = a10_from_m500_z(M500, z,radkpc,Dist=Dist)
+    PresProf  = a10_from_m500_z(M500, z,radkpc,Dist=Dist,c500=c500,p=p,a=a,b=b,c=c)
     to,yProf  = get_yProf(radkpc,PresProf,z)
     #x2p,y2p   = xymap
     #origshape = x2p.shape
     #xy2pass   = (x2p.flatten(),y2p.flatten())
     #print(xy2pass[0].shape,thetas.shape,yProf.shape,origshape)
     
     flatymap  = grid_profile(thetas,yProf,xymap)
@@ -565,49 +575,58 @@
 
     """
  
     xnew = x/ella ; ynew = y/ellb
 
     return xnew, ynew
 
-def a10_from_m500_z(m500, z,rads,Dist=False):
+def a10_from_m500_z(m500, z,rads,Dist=True,c500=None,p=None,a=None,b=None,c=None):
     """
     Parameters
     ----------
     M500 : quantity
        :math:`M\_{500}` with units of mass.
     z : float
        Redshift
     xymap : tuple(class:`numpy.ndarray`)
        A tuple of x- and y-coordinates
     rads : quantity,array
        Array of radii (with units of length)
     Dist : bool
        Assume a disturbed A10 profile? Default is False
+    c500 : float, none-type
+      If None, adopts the radius scaling value for A10 (full or disturbed) sample
+    p : float, none-type
+      If None, adopts the normalization value for A10 (full or disturbed) sample
+    a : float, none-type
+      If None, adopts the alpha value for A10 (full or disturbed) sample
+    b : float, none-type
+      If None, adopts the beta value for A10 (full or disturbed) sample
+    c : float, none-type
+      If None, adopts the gamma value for A10 (full or disturbed) sample
 
     Returns
     -------
     gnfw_prof : quantity,array
        A radial profile with units of pressure
 
     """
     
     r500, p500 = R500_P500_from_M500_z(m500,z)
-    if Dist:
-        c500= 1.083
-        p=3.202
-        a=1.4063
-        b=5.4905
-        c=0.3798
-    else:
-        c500= 1.177
-        p=8.403
-        a=1.0510
-        b=5.4905
-        c=0.3081
+    if c500 is None:
+        c500 = 1.083 if Dist else 1.177
+    if p is None:
+        p = 3.202 if Dist else 8.403
+    if a is None:
+        a = 1.4063 if Dist else 1.0510
+    if b is None:
+        b = 5.4905     # Fixed to simulations for all subsets.
+    if c is None:
+        c = 0.3798 if Dist else 0.3081 # Steeper for the disturbed sample! Oh Degeneracies.
+    
     gnfw_prof  = gnfw(r500,p500,rads,c500=c500,p=p,a=a,b=b,c=c)
     
     return gnfw_prof
 
 def get_yProf(radii,pprof,z):
     """
     Parameters
@@ -733,15 +752,15 @@
                     "planck":planck,"tcmb":tcmb.value,"c":c.value,}
     ### The following "constants" have units attached (in Python)!
     sz_cons_units={"Icmb":Icmb,"Jycmb":Jycmb,"thom_cross":thom_cross,
                    "m_e_c2":m_e_c2}
 
     return sz_cons_values, sz_cons_units
 
-def make_A10Map(M500,z,pixsize=2,h70=1,nb_theta_range=150,Dist=False,nR500=3.0):
+def make_A10Map(M500,z,pixsize=2,h70=1,nb_theta_range=150,Dist=True,nR500=3.0,c500=None,p=None,a=None,b=None,c=None):
     """
     Makes an A10 map with automated mapsize.
 
     Parameters
     ----------
     M500 : quantity
        :math:`M\_{500}` with units of mass.
@@ -751,14 +770,24 @@
        Pixel size, in arcseconds
     h70 : float
        Normalization of the Hubble parameter.
     nb_theta_range : int
        Number of elements in an array of radii.
     Dist : bool
        Assume a disturbed A10 profile? Default is False
+    c500 : float, none-type
+      If None, adopts the radius scaling value for A10 (full or disturbed) sample
+    p : float, none-type
+      If None, adopts the normalization value for A10 (full or disturbed) sample
+    a : float, none-type
+      If None, adopts the alpha value for A10 (full or disturbed) sample
+    b : float, none-type
+      If None, adopts the beta value for A10 (full or disturbed) sample
+    c : float, none-type
+      If None, adopts the gamma value for A10 (full or disturbed) sample
 
     Returns
     -------
     ymap : class:`numpy.ndarray`
        An output Compton y map
 
     """
@@ -768,15 +797,15 @@
     tnx        = [minpixrad.value,10.0*Theta500]  # In radians
     thetas     = np.logspace(np.log10(tnx[0]),np.log10(tnx[1]), nb_theta_range)
     map_vars   = {"thetas":thetas}
     nx         = int( np.round( (Theta500*3600*180/np.pi)*nR500*2/pixsize) )
     mapshape   = (nx,nx)
     zeromap    = np.zeros(mapshape)
     xymap      = get_xymap(zeromap,pixsize=pixsize*u.arcsec)
-    ymap       = make_a10_map(M500,z,xymap,Theta500,nx,nx,Dist=Dist)
+    ymap       = make_a10_map(M500,z,xymap,Theta500,nx,nx,Dist=Dist,c500=c500,p=p,a=a,b=b,c=c)
 
     return ymap
 
 def smooth_by_M2_beam(image,pixsize=2.0):
     """
     Smooths an image by a double Gaussian that is representative for MUSTANG-2.
 
@@ -947,16 +976,16 @@
 
     tab   = get_xfertab(size,WIKID=WIKID)
     yxfer = FI.apply_xfer(skymap,tab,pixsize)
 
     return yxfer
 
 def lightweight_simobs_A10(z,M500,ptgs=[[180,45.0]],sizes=[3.5],times=[10.0],offsets=[1.5],
-                           center=[180,45.0],xsize=12.0,ysize=12.0,pixsize=2.0,Dist=False,
-                           fwhm=9.0,conv2uK=False,verbose=False,y2k=-3.4):
+                           center=[180,45.0],xsize=12.0,ysize=12.0,pixsize=2.0,Dist=True,
+                           fwhm=9.0,conv2uK=False,verbose=False,y2k=-3.4,c500=None,p=None,a=None,b=None,c=None):
     """   
     A lightweight mock observation tool. To be lightweight, everything is approximate -- but it's fast!
 
     Parameters
     ----------
     z : float
        The redshift
@@ -982,20 +1011,30 @@
        Adopt a disturbed A10 model?
     fwhm : float
        The smoothing kernal for a resultant MIDAS map, in arcseconds. 9" is the default.
     conv2uK : bool
        Convert the resultant images from Compton y to microK_RJ (the standard units for MUSTANG-2 maps).
     verbose : bool
        Have the function print extraneous information?
+    c500 : float, none-type
+      If None, adopts the radius scaling value for A10 (full or disturbed) sample
+    p : float, none-type
+      If None, adopts the normalization value for A10 (full or disturbed) sample
+    a : float, none-type
+      If None, adopts the alpha value for A10 (full or disturbed) sample
+    b : float, none-type
+      If None, adopts the beta value for A10 (full or disturbed) sample
+    c : float, none-type
+      If None, adopts the gamma value for A10 (full or disturbed) sample
 
     """
     
     sig2fwhm       = np.sqrt(8.0*np.log(2.0)) 
     pix_sigma      = fwhm/(pixsize*sig2fwhm)
-    ymap           = make_A10Map(M500,z,pixsize=pixsize,Dist=Dist)
+    ymap           = make_A10Map(M500,z,pixsize=pixsize,Dist=Dist,c500=c500,p=p,a=a,b=b,c=c)
     mymap          = smooth_by_M2_beam(ymap,pixsize=pixsize)
     nx,ny          = mymap.shape
     SkyHDU         = MRM.make_template_hdul(nx,ny,center,pixsize)
     SkyHDU[0].data = mymap*1.0
     Skyhdr         = SkyHDU[0].header
     SkyCoadd       = MRM.make_template_hdul(nx,ny,center,pixsize)
 
@@ -1046,15 +1085,16 @@
     SkyCoadd[0].data =  SkyObs*myFactor
     SSP              =  fits.PrimaryHDU(SkySmooth,header=SkyCoadd[0].header)
     SSS              =  fits.ImageHDU(SkyCoadd[1].data,header=SkyCoadd[0].header)
     SkySmHDU         =  fits.HDUList([SSP,SSS])
     
     return SkyCoadd, SkySmHDU,SkyHDU
 
-def make_A10_hdu(z,M500,pixsize,center=[180,45.0],nR500=3.0,Dist=False,beamConvolve=True,conv2uK=True,y2k=-3.4):
+def make_A10_hdu(z,M500,pixsize,center=[180,45.0],nR500=3.0,Dist=True,beamConvolve=True,conv2uK=True,y2k=-3.4,
+                 c500=None,p=None,a=None,b=None,c=None):
     """   
     Compute and grid an A10 Compton y profile and put it into an HDUList
 
     Parameters
     ----------
     z : float
        The redshift
@@ -1068,18 +1108,28 @@
        Adopt a disturbed A10 model?
     conv2uK : bool
        Convert the resultant images from Compton y to microK_RJ (the standard units for MUSTANG-2 maps).
     y2k : float
        What is the conversion factor between Compton y and K_RJ (for MUSTANG-2)? The default is -3.4, which corresponds to the conversion with relativistic corrections for kT_e ~ 7 keV. This factor is -3.5 at kT_e = 2 keV and -3.3 at kT_e = 12 keV.
     verbose : bool
        Have the function print extraneous information?
+    c500 : float, none-type
+      If None, adopts the radius scaling value for A10 (full or disturbed) sample
+    p : float, none-type
+      If None, adopts the normalization value for A10 (full or disturbed) sample
+    a : float, none-type
+      If None, adopts the alpha value for A10 (full or disturbed) sample
+    b : float, none-type
+      If None, adopts the beta value for A10 (full or disturbed) sample
+    c : float, none-type
+      If None, adopts the gamma value for A10 (full or disturbed) sample
 
     """
 
-    ymap           = make_A10Map(M500,z,pixsize=pixsize,Dist=Dist,nR500=nR500)
+    ymap           = make_A10Map(M500,z,pixsize=pixsize,Dist=Dist,nR500=nR500,c500=c500,p=p,a=a,b=b,c=c)
     if beamConvolve:
         mymap          = smooth_by_M2_beam(ymap,pixsize=pixsize)
     else:
         mymap          = ymap.copy()
     nx,ny          = mymap.shape
     SkyHDU         = MRM.make_template_hdul(nx,ny,center,pixsize)
     myFactor       =  y2k*1e6 if conv2uK else 1.0
```

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/analytic_integrations.py` & `m2_tj-1.1.0/src/M2_ProposalTools/analytic_integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import astropy.units as u
 from scipy.interpolate import interp1d # numpy should be faster...
 import scipy.special as sps
+#import warnings
 
 def log_profile(args,r_bins,radii,alphas=[],rintmax=[],finite=False):
     """   
     Performs logarithmic interpolation and extrapolation. This can easily be improved, but hasn't been the bottleneck.
     
     r_bins and radii must be in the same units.
     Parameters
@@ -25,14 +26,16 @@
 
     Returns
     -------
     presprof : Interpolated (pressure) profile
     alphas : The power-law indices between bins (e.g. pressures)
     """
 
+    #warnings.showwarning = handle_warning
+    
     #r_uniqe = np.unique(r_bins)
     #mybins=[0] + r_bins
     if not finite:
         mybins=np.insert(r_bins,0,0)
         mybins[-1]=-1
         #import pdb;pdb.set_trace()
     else:
@@ -73,15 +76,16 @@
             lp=np.log10(args[idx+1]/args[idx])
             if aset == 0:
                 alpha=-lp/lr
                 #                myind=np.where((radii < rout) & (radii >= rin))
             myind=(radii < rout) & (radii >= rin)
             myrad=radii[myind]
             mypres=epsnot*(myrad/rout)**(-alpha)
-            yint = 1.0 - (rin/rout)**(2-alpha)  # I could leave out the second term...
+            # I'm often not using the integrated y; but we can keep it for now.
+            yint = 0 if rin == 0 else 1.0 - (rin/rout)**(2-alpha)
             # but this ensures an error if alpha >2 ...
             rnot=rout
         elif rout == -1:
             lr=np.log10(r_bins[idx]/r_bins[idx-1])
             lp=np.log10(args[idx]/args[idx-1])
             if aset == 0:
                 alpha=-lp/lr
@@ -1181,7 +1185,23 @@
     lnp = np.log(Int_Pres)
     ltr = np.log(theta_range)
 
     alpha = (np.roll(lnp,-1) - lnp ) / (np.roll(ltr,-1) - ltr )
     k     = Int_Pres / theta_range**alpha
 
     return alpha,k
+
+def handle_warning(message, category, filename, lineno, file=None, line=None):
+    print('A warning occurred:')
+    print(message)
+    print('Do you wish to continue?')
+
+    while True:
+        response = input('y/n: ').lower()
+        if response not in {'y', 'n'}:
+            print('Not understood.')
+        else:
+            break
+
+    if response == 'n':
+        import pdb;pdb.set_trace()
+        #raise category(message)
```

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/numerical_integration.py` & `m2_tj-1.1.0/src/M2_ProposalTools/numerical_integration.py`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_2p5_21Aonly_PCA5_0f08Filtering.txt` & `m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_2p5_21Aonly_PCA5_0f08Filtering.txt`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_3p0_21Aonly_PCA5_0f08Filtering.txt` & `m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_3p0_21Aonly_PCA5_0f08Filtering.txt`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_3p5_21Aonly_PCA5_0f08Filtering.txt` & `m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_3p5_21Aonly_PCA5_0f08Filtering.txt`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_4p0_21Aonly_PCA5_0f08Filtering.txt` & `m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_4p0_21Aonly_PCA5_0f08Filtering.txt`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_4p5_21Aonly_PCA5_0f08Filtering.txt` & `m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_4p5_21Aonly_PCA5_0f08Filtering.txt`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/src/M2_ProposalTools/xfer_Function_5p0_21Aonly_PCA5_0f08Filtering.txt` & `m2_tj-1.1.0/src/M2_ProposalTools/xfer_Function_5p0_21Aonly_PCA5_0f08Filtering.txt`

 * *Files identical despite different names*

### Comparing `M2_TJ-0.2/src/M2_TJ.egg-info/SOURCES.txt` & `m2_tj-1.1.0/src/M2_TJ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

