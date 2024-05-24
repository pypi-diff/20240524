# Comparing `tmp/NFA_Aerosol-1.0.7.tar.gz` & `tmp/nfa_aerosol-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NFA_Aerosol-1.0.7.tar", last modified: Fri Feb 23 13:30:07 2024, max compression
+gzip compressed data, was "nfa_aerosol-1.0.8.tar", last modified: Thu May 23 14:07:50 2024, max compression
```

## Comparing `NFA_Aerosol-1.0.7.tar` & `nfa_aerosol-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:30:07.212149 NFA_Aerosol-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-23 13:29:58.000000 NFA_Aerosol-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-23 13:30:07.212149 NFA_Aerosol-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-23 13:29:58.000000 NFA_Aerosol-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-23 13:29:58.000000 NFA_Aerosol-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 13:30:07.212149 NFA_Aerosol-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:30:07.208150 NFA_Aerosol-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:30:07.208150 NFA_Aerosol-1.0.7/src/NFA_Aerosol/
--rw-r--r--   0 runner    (1001) docker     (127)    50371 2024-02-23 13:29:58.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol/Instrument_Lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    42571 2024-02-23 13:29:58.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol/Plot_Lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    41546 2024-02-23 13:29:58.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol/Utility_Lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 13:29:58.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:30:07.212149 NFA_Aerosol-1.0.7/src/NFA_Aerosol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-23 13:30:07.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-23 13:30:07.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 13:30:07.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-23 13:30:07.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-23 13:30:07.000000 NFA_Aerosol-1.0.7/src/NFA_Aerosol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:30:07.212149 NFA_Aerosol-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 13:29:58.000000 NFA_Aerosol-1.0.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:50.779547 nfa_aerosol-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 14:07:36.000000 nfa_aerosol-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-23 14:07:50.779547 nfa_aerosol-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-23 14:07:36.000000 nfa_aerosol-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-23 14:07:36.000000 nfa_aerosol-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:07:50.779547 nfa_aerosol-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:50.775547 nfa_aerosol-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:50.775547 nfa_aerosol-1.0.8/src/NFA_Aerosol/
+-rw-r--r--   0 runner    (1001) docker     (127)    53805 2024-05-23 14:07:36.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol/Instrument_Lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42593 2024-05-23 14:07:36.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol/Plot_Lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48426 2024-05-23 14:07:36.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol/Utility_Lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:07:36.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:50.779547 nfa_aerosol-1.0.8/src/NFA_Aerosol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-23 14:07:50.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 14:07:50.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:07:50.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 14:07:50.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 14:07:50.000000 nfa_aerosol-1.0.8/src/NFA_Aerosol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:50.779547 nfa_aerosol-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:07:36.000000 nfa_aerosol-1.0.8/tests/test.py
```

### Comparing `NFA_Aerosol-1.0.7/LICENSE.txt` & `nfa_aerosol-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NFA_Aerosol-1.0.7/PKG-INFO` & `nfa_aerosol-1.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NFA_Aerosol
-Version: 1.0.7
+Version: 1.0.8
 Summary: Data handling for Aerosol Instruments at NFA
 Author: NRCWE community
 Project-URL: Homepage, https://github.com/NRCWE/NFA_Aerosol
 Keywords: Aerosol,Particle,Instrument,Gas Analyzer,Dust,data analysis,numpy,python,scipy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,11 @@
 Requires-Dist: matplotlib>=3.1.3
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: pandas>=1.5.3
 
 # NFA_Aerosol
 A package of usefull functions when working with particle data at NFA
+
+The package is available for installation via pip:
+
+pip install NFA_Aerosol
```

### Comparing `NFA_Aerosol-1.0.7/pyproject.toml` & `nfa_aerosol-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NFA_Aerosol"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
     {name = "NRCWE community"},
     ]
 description = "Data handling for Aerosol Instruments at NFA"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `NFA_Aerosol-1.0.7/src/NFA_Aerosol/Instrument_Lib.py` & `nfa_aerosol-1.0.8/src/NFA_Aerosol/Instrument_Lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -679,14 +679,89 @@
     
     return Data_return, Bin_edges, Header
 
 ###############################################################################
 ###############################################################################
 ###############################################################################
 
+def Load_OPCN3_PM(file, start=0, end=0):
+    """
+    Function to load data from a .csv datafile generated by the OPCN3 and 
+    extract relevant data for plotting.
+    
+    Parameters
+    ----------
+    file : str
+        Path to a .csv file generated by the OPCN3
+    start : datetime, optional
+        Specify starting time to plot by setting a datetime value e.g.
+        datetime.datetime(2023,01,28,15,00,00). The default is 0.
+    end : datetime, optional
+        Specify end time to plot by setting a datetime value e.g.
+        datetime.datetime(2023,01,28,15,00,00). The default is 0.
+
+    Returns
+    -------
+    Data_return : numpy.array
+        Array containing PM1, PM2.5 and PM10 data from the OPC including a column
+        of Datetime values for easy plotting.
+    Header : list
+        A list containing the header for all columns in the Data_return variable
+
+    Creators JBL and JOT
+    """
+ 
+    # Load data
+    PM_data=np.genfromtxt(file,delimiter=",",skip_header=1)[:,-4:-1]
+    time_s=np.genfromtxt(file,delimiter=",",skip_header=1, dtype=str)[:,0]
+    
+    # Define header
+    Header=["Time","PM1(ug/m3)","PM2.5(ug/m3)","PM10(ug/m3)"]
+    
+    # Extract dates from the time
+    Date=np.array([i.split("T")[0]  for i in time_s])
+    
+    #Correction due to "\00X" error in some lines
+    for i in range(0,len(Date)):
+        Date[i]=Date[i][-10:]
+    
+    # Extract times
+    Time=np.array([i.split("T")[1].split(".")[0]  for i in time_s])
+    Ms=np.array(["0."+i.split(".")[1].split("+")[0]  for i in time_s])
+    
+    # Combine date and time in correct format
+    DateTime=np.array([Date[i]+" "+Time[i] for i in range(len(Time))])
+      
+    # Convert to datetime format
+    DateTime=np.array([datetime.strptime(i, '%Y-%m-%d %H:%M:%S') for i in DateTime])
+    
+    # Add ms data
+    for i in range(0,len(DateTime)):
+        DateTime[i] = DateTime[i]+timedelta(0,float(Ms[i]))
+        
+    # Select data within specified time interval if specified
+    if (start != 0) or (end != 0):
+        if (start != 0) & (end == 0):
+            index = DateTime>start
+        elif (start == 0) & (end != 0):
+            index = DateTime<end
+        else:
+            index = (DateTime>start) & (DateTime<end)
+        DateTime = DateTime[index]
+        PM_data = PM_data[index]
+    
+    # Combine time with PM data
+    PM_Data=np.column_stack((DateTime,PM_data))
+
+    return PM_Data, Header
+
+###############################################################################
+###############################################################################
+###############################################################################
+
 def Load_OPS(file, start=0, end=0):
         """
         Function to load data from comma seperated .txt datafile generated by 
         the OPS and extract relevant data for plotting.
         
         Parameters
         ----------
@@ -986,39 +1061,67 @@
 ###############################################################################
 ###############################################################################
 ###############################################################################
 
 def Get_Bin_Mids(bin_edges):
     """
     Function to get bin_mids from bin_edges
-    
     Creator: PLF 
+    
+    Parameters
+    ----------
+    bin_edges : np.array
+        Array of sizebin edges as returned by the load instrument functions.
+
+    Returns
+    -------
+    bin_mids : np.array
+        An array of the midpoints of each sizebin. Note that the array length 
+        is len(bin_edges)-1
 
     """
-    bin_mids = [(bin_edges[i] + bin_edges[i+1]) / 2 for i in range(len(bin_edges) - 1)]    
+    
+    bin_mids = np.array([(bin_edges[i] + bin_edges[i+1]) / 2 for i in range(len(bin_edges) - 1)])    
+    
     return bin_mids
 
 ###############################################################################
 ###############################################################################
 ###############################################################################
 
 def load_data_from_folder(folder_path, load_function, file_extension, year=None, month=None):
     """
     Generic function to load data from a folder.
-
-    Parameters:
-    - folder_path: Path to the folder containing the data files.
-    - load_function: Function to use for loading the data.
-    - file_extension: File extension of the data files.
-    - year: Year parameter for load_function (optional). -- FMPS
-    - month: Month parameter for load_function (optional). -- FMPS
     
     Creator: PLF 
     
+    Parameters
+    ----------
+    folder_path : str
+        Path to the folder containing the data files.
+    load_function : function
+        Function to use for loading the data..
+    file_extension : str
+        File extension of the data files to load.
+    year : int, optional
+        Year parameter for load_function if Load_FMPS_1 is used. The default is None.
+    month : TYPE, optional
+        Month parameter for load_function if Load_FMPS_1 is used. The default is None.
+
+    Returns
+    -------
+    sorted_data : list
+        List of the loaded data.
+    bin_edges : np.array
+        Array of sizebin edges.
+    Header : list
+        List of all the column headers of the loaded dataset.
+
     """
+    
     all_data = []
     for file_name in os.listdir(folder_path):
         if file_name.endswith(file_extension):
             file_path = os.path.join(folder_path, file_name)
             data, bin_edges, Header = load_function(file_path, year, month, start=0, end=0) if year and month \
                                       else load_function(file_path, start=0, end=0)
             bin_mids = [(bin_edges[i] + bin_edges[i+1]) / 2 for i in range(len(bin_edges) - 1)]
@@ -1162,8 +1265,8 @@
     Data_return = np.column_stack([FMPS_datetime,FMPS_Total,FMPS_data])
     Header = ["Datetime","Total"] + list(Bin_mids)
     
     return Data_return, Bin_edges, Header
 
 ###############################################################################
 ###############################################################################
-###############################################################################
+###############################################################################
```

### Comparing `NFA_Aerosol-1.0.7/src/NFA_Aerosol/Plot_Lib.py` & `nfa_aerosol-1.0.8/src/NFA_Aerosol/Plot_Lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -984,15 +984,15 @@
     
     return fig, ax
 
 ###############################################################################
 ###############################################################################
 ###############################################################################
   
-def Plot_PSD_1(*data_in, labels=None, ylog=True, xlog=True, y_lim=(0, 0), datatype="number"):
+def Plot_PSD_different_instruments(*data_in, labels=None, ylog=True, xlog=True, y_lim=(0, 0), datatype="number"):
     """
     Similar to Plot_PSD only this function can plot the PSDs for multiple instruments
     that have different bin mids. 
 
     Parameters
     ----------
     *data_in : list of tuples
@@ -1047,8 +1047,8 @@
     # Adjust y-axis limits if specified
     if y_lim != (0, 0):
         ax.set_ylim(y_lim)
 
     if labels:
         ax.legend()
 
-    return fig, ax
+    return fig, ax
```

### Comparing `NFA_Aerosol-1.0.7/src/NFA_Aerosol/Utility_Lib.py` & `nfa_aerosol-1.0.8/src/NFA_Aerosol/Utility_Lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -364,14 +364,126 @@
     
     return Dep_HA,Dep_TB,Dep_AL,Dep_TT
 
 ###############################################################################
 ###############################################################################
 ###############################################################################
 
+def MPS_Ceff(Pdiam,flowrate=0.6):
+    """
+    Function to estimate the collection efficiency of the mini particle sampler (MPS)
+    as a function of particle size and flowrate. It should be noted, that the 
+    expression is only valid up untill a particle diamter of 1 um, from where 
+    a collection efficiency of 1 can be used. 
+    
+    The function assumes that 1.2/1.3 Quantfoil grids were used when sampling.
+    
+    Parameters
+    ----------
+    Pdiam : np.array()
+        Array of particle diameters in um from which to determine the collection
+        efficiency.
+    flowrate : float, optional
+        Flowrate used during sampling in lpm. The default is 0.6 lpm.
+
+    Returns
+    -------
+    E_total : np.array
+        Overall collection efficiency of the MPS at the given size and flow.
+    E_impaction : np.array
+        Collection efficiency from impaction alone at the given size and flow.
+    E_diffusion : np.array
+        Collection efficiency from diffusion to a flat surface alone at the given size and flow.
+    E_interception : np.array
+        Collection efficiency from interception alone at the given size and flow.
+    E_edge : np.array
+        Collection efficiency from diffusion to pore edges alone at the given size and flow.
+
+    """
+    ###########################################################################
+    "Constants and conversions , units        , Descriptions" 
+    rP = (Pdiam/2) * 1e-6      # m            ; Particle radius
+    rhop = 1000                # kg/m3        ; Particle density
+    lambda1 = 0.069 * 1e-6     # m            ; Molecule mean free path
+    Lf = 0.02 * 1e-6           # m            ; Filter thickness
+    N0 = 16003913722018.367    # #            ; Number of pores per surface unit of the carbon film
+    r0 = 0.6 * 1e-6            # m            ; Pore radius
+    A0 = np.pi*(r0**2)         # m2           ; Area of a single pore
+    P  = A0*N0/100             # unitless     ; Porosity
+    rc = r0/np.sqrt(P)         # m            ; Cylindrical aerosol stream passed through a unitary pore
+    df = 2 * 1e-3              # m            ; TEM grid diameter
+    Q  = flowrate/60 * 1e-3    # m3/s         ; Flowrate through the MPS
+    U0 = Q / ((np.pi/4)*df**2) # m/s          ; Flow velocity
+    nu = 1.85e-5               # kg/(m*s)     ; Fluid dynamic viscosity
+    Kb = 1.381e-23             # kg*m2/(s2*K) ; Boltzmann constant
+    T  = 300                   # K            ; Temperature
+    Kn = lambda1 / rP          # unitless     ; Knudsen number
+    Cc = 1 + Kn *(1.165 + 0.483*
+         np.exp(-0.997/Kn))    # unitless     ; Cunningham slipfactor correction
+    D = (Kb*T*Cc)/(6*np.pi*
+                   nu*rP)      # m2/s         ; Diffusion coefficient    
+    
+    ############################## Interception ###############################
+    # Calculate collection efficiency resulting from interception of particles
+    lg = 1.126 * lambda1       # m            ; slip length
+    Ng = lg/r0                 # unitless     ; Slip parameter
+    NG = Ng*(1+Ng/2)           # unitless     ; Parameter
+    Nr = rP/r0                 # unitless     ; Particle radius normalized for pore radius
+    NR = Nr * (1-Nr/2)         # unitless     ; Parameter
+    
+    # Collection efficiency via interception
+    E_interception = ((4*NR**2)/(1+4*NG))*(1+2*(NG/NR)) 
+    
+    ####################### Diffusion to pore edge ############################
+    # Calculate collection efficiency resulting from particles diffusing to the pore edges
+    Pe = U0 / (np.pi*Lf * D * 
+               N0)             # unitless     ; Peclets number
+    
+    # Collection efficiency from pore edges calculated for different flow regimes
+    E_edge = np.ones_like(Pe)
+    E_edge[Pe > 25] = 2.56*Pe[Pe > 25]**(-2/3) -1.2*Pe[Pe > 25]**(-1)-0.177*Pe[Pe > 25]**(-4/3)
+    E_edge[Pe <= 25] =  (1 - 0.81904*np.exp(-3.6568*Pe[Pe <= 25]**(-1)) - 0.09752*
+                np.exp(-22.3045*Pe[Pe <= 25]**(-1))-0.03248*np.exp(-56.95*Pe[Pe <= 25]**(-1)) -
+                0.0157*np.exp(-107.6*Pe[Pe <= 25]**(-1)))
+    
+    ######################### Diffusion to surface ############################
+    # Calculate collection efficiency resulting from particles diffusing to flat filter surfaces
+    alpha2 = 4.5                # unitless    ; Parameter
+    Ds = D/ (rc*U0)             # unitless    ; Normalized diffusion coefficient
+    alpha1 = (4.57-6.46*P
+              +4.58*P**2)       # unitless    ; Parameter
+    
+    # Collection efficiency of filter via diffusion
+    E_diffusion = 1-np.exp(-(alpha1*(Ds**(2/3)))/(1+(alpha1/alpha2)*Ds**(7/15))) 
+
+    ############################## Impaction ##################################
+    # Calculate collection efficiency resulting from impaction
+    stk = (2*Cc*U0*rP**2*rhop
+          )/(9*nu*r0)           # unitless     ; Stokes number
+    eta = np.sqrt(P)/(1-
+          np.sqrt(P))           # unitless     ; Parameter
+    ei = (2*stk *np.sqrt(eta)+ 
+          2 * (stk**2)*eta * 
+          np.exp(-1/(stk*
+          np.sqrt(eta)))-2*
+          (stk**2)*eta)         # unitless     ; Parameter
+    
+    # Collection efficiency via impaction
+    E_impaction = (2 *ei) / (1+eta) - (ei / (1 + eta))**2
+    
+    ############################## Overall Ceff ###############################
+    # Calculate overall collection efficiency of the MPS
+    E_total = 1 - (1-E_impaction)*(1-E_diffusion)*(1-E_interception)*(1-E_edge)
+    
+    return E_total, E_impaction, E_diffusion, E_interception, E_edge
+
+###############################################################################
+###############################################################################
+###############################################################################
+
 def Normalize_dndlogdp(data_in,bin_edges):
     """
     Function to normalize an array of particle xxx concentrations (xxx can be
     mass, volume, surface area, and number), going from dxxx values to 
     dxxx/dlogDp.
 
     Parameters
@@ -560,14 +672,59 @@
     
     return Data_return
     
 ###############################################################################
 ###############################################################################
 ###############################################################################
 
+def Partector_Ceff(Psize):
+    """
+    Function to estimate the collection efficiency of the partectorTEM at the
+    specified particle size in nm. The collection efficiency as a fraction is 
+    returned and can be multiplied with the measured concentration to get a 
+    corrected concentration.
+    
+    It should be noted, that the expression for the collection efficiency has
+    only been validated for NaCl and Ag particles in the size range from 3 to
+    320 nm, and may therefore not be accurate at um sizes!
+    
+    Reference: Fierz, M., Kaegi, R., and Burtscher, H.;"Theoretical and 
+    Experimental Evaluation of a Portable Electrostatic TEM Sampler", Aerosol
+    Science and Technology, 41, issue 5, 2007.
+
+    Parameters
+    ----------
+    Psize : float or np.array
+        Either a single particle size given as a float, or an array of particle
+        sizes to be used for calculating the collection efficiency.
+
+    Returns
+    -------
+    Collection_efficiency : float or np.array
+        The calculated collection efficiency of the PartectorTEM at the specified
+        particle size/sizes specified as a fraction (0-1).
+
+    """
+    Collection_efficiency = (1700*Psize**(-1.78))/100
+    
+    def is_array(param):
+        return type(param) is np.ndarray
+
+    if is_array(Psize):
+        Collection_efficiency[Psize <= 10] = 1
+    else:
+        if Psize <= 10:
+            Collection_efficiency = 1
+            
+    return Collection_efficiency 
+    
+###############################################################################
+###############################################################################
+###############################################################################
+
 def PM_calc(data_in,bin_edges,*PM):
     """
     Function to calculate PM from size bins from an array similar to those
     returned from Load_xxx functions. 
     
     Note that the data should already be converted to mass e.g. ug/m3 as the
     output of this function will maintain the same units as the input.
@@ -1020,30 +1177,7 @@
         Created by: PLF
     """
     filtered_data = data[(data[:, 0] >= start_time) & (data[:, 0] <= end_time)]
     if len(filtered_data) > 0:
         return np.mean(filtered_data[:, 1])
     else:
         return np.nan  # Return NaN if no data is available in the time span
-
-def filter_data(data, start_time, end_time):
-    """
-    Function to filter data for a specific time span
-
-    Parameters
-    ----------
-    data : numpy.array
-        A 2D array where the first column contains datetime objects and the 
-        second column contains numerical values for which the average is to be calculated.
-    start_time : datetime
-        The start time for the period over which to calculate the average.
-    end_time : datetime
-        The end time for the period over which to calculate the average.
-
-    Returns
-    -------
-    data : numpy.array
-        
-        Created by: PLF
-    """
-    filtered_data = data[(data[:, 0] >= start_time) & (data[:, 0] <= end_time)]
-    return filtered_data
```

### Comparing `NFA_Aerosol-1.0.7/src/NFA_Aerosol.egg-info/PKG-INFO` & `nfa_aerosol-1.0.8/src/NFA_Aerosol.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NFA_Aerosol
-Version: 1.0.7
+Version: 1.0.8
 Summary: Data handling for Aerosol Instruments at NFA
 Author: NRCWE community
 Project-URL: Homepage, https://github.com/NRCWE/NFA_Aerosol
 Keywords: Aerosol,Particle,Instrument,Gas Analyzer,Dust,data analysis,numpy,python,scipy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,11 @@
 Requires-Dist: matplotlib>=3.1.3
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: pandas>=1.5.3
 
 # NFA_Aerosol
 A package of usefull functions when working with particle data at NFA
+
+The package is available for installation via pip:
+
+pip install NFA_Aerosol
```

