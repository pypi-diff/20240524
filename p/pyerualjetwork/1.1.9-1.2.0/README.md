# Comparing `tmp/pyerualjetwork-1.1.9.tar.gz` & `tmp/pyerualjetwork-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.1.9.tar", last modified: Thu May 23 08:33:41 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.2.0.tar", last modified: Fri May 24 14:25:19 2024, max compression
```

## Comparing `pyerualjetwork-1.1.9.tar` & `pyerualjetwork-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 08:33:41.826791 pyerualjetwork-1.1.9/
--rw-rw-rw-   0        0        0      276 2024-05-23 08:33:41.826791 pyerualjetwork-1.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 08:33:41.811170 pyerualjetwork-1.1.9/plan/
--rw-rw-rw-   0        0        0      315 2024-05-23 00:45:27.000000 pyerualjetwork-1.1.9/plan/__init__.py
--rw-rw-rw-   0        0        0    40147 2024-05-23 08:32:13.000000 pyerualjetwork-1.1.9/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:33:41.826791 pyerualjetwork-1.1.9/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-23 08:33:41.000000 pyerualjetwork-1.1.9/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-23 08:33:41.000000 pyerualjetwork-1.1.9/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 08:33:41.000000 pyerualjetwork-1.1.9/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 08:33:41.000000 pyerualjetwork-1.1.9/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 08:33:41.826791 pyerualjetwork-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-23 08:33:37.000000 pyerualjetwork-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:25:19.827287 pyerualjetwork-1.2.0/
+-rw-rw-rw-   0        0        0      309 2024-05-24 14:25:19.825291 pyerualjetwork-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 14:25:19.805913 pyerualjetwork-1.2.0/plan/
+-rw-rw-rw-   0        0        0      315 2024-05-23 00:45:28.000000 pyerualjetwork-1.2.0/plan/__init__.py
+-rw-rw-rw-   0        0        0    40179 2024-05-24 14:21:37.000000 pyerualjetwork-1.2.0/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:25:19.824331 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      309 2024-05-24 14:25:19.000000 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-24 14:25:19.000000 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 14:25:19.000000 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-24 14:25:19.000000 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 14:25:19.827287 pyerualjetwork-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      485 2024-05-24 14:24:44.000000 pyerualjetwork-1.2.0/setup.py
```

### Comparing `pyerualjetwork-1.1.9/plan/plan.py` & `pyerualjetwork-1.2.0/plan/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         Neurons (list[num]): List of neuron counts for each layer.
         ThresholdSigns (list[str]): List of threshold signs.
         ThresholdValues (list[num]): List of threshold values.
         Normalizations (List[str]): Whether normalization will be performed at indexed layers ("y" or "n").
         Activations (list[str]): List of activation functions.
     
     Returns:
-        list([num]): (Weight matrices list, TrainPredictions list.).
+        list([num]): (Weight matrices list, TrainPredictions list, TrainAcc).
         error handled ?: Process status ('e')
 """
         
     LastNeuron = Neurons[-1:][0]
     if LastNeuron != ClassCount:
             print(Fore.RED + "ERROR108: Last layer of neuron count must be equal class count. from: TrainPLAN",infoPLAN)
             return 'e'
@@ -241,15 +241,15 @@
     
     elif Acc < 0.6:
         print(Fore.RED+ '\nTotal Train Accuracy: ' ,Acc, '\n',Style.RESET_ALL)
     
     
     
 
-    return TrainedWs,TrainPredictions
+    return TrainedWs,TrainPredictions,Acc
         
 # FUNCTIONS -----
 
 def WeightIdentification(
     LayerCount,      # int: Number of layers in the neural network.
     ClassCount,      # int: Number of classes in the classification task.
     Neurons,         # list[num]: List of neuron counts for each layer.
@@ -553,15 +553,15 @@
 def TestPLAN(
     TestInputs,         # list[list[num]]: Test input data.
     TestLabels,         # list[num]: Test labels.
     Layers,             # list[str]: List of layer names.
     ThresholdSigns,     # list[str]: List of threshold signs for each layer.
     ThresholdValues,    # list[num]: List of threshold values for each layer.
     Normalizations,    # str: Whether normalization will be performed ("y" or "n").
-    Activation,         # str: Activation function list for the neural network.
+    Activations,         # str: Activation function list for the neural network.
     W                  # list[list[num]]: Weight matrix of the neural network.
 ) -> tuple:
     infoTestModel =  """
     Tests the neural network model with the given test data.
 
     Args:
         TestInputs (list[list[num]]): Test input data.
@@ -593,19 +593,19 @@
             Input = Input.ravel()
             UniStartTime = time.time()
             NeuralLayer = Input
             
             for index, Layer in enumerate(Layers):
                 if Normalizations[index] == 'y':
                     NeuralLayer = Normalization(NeuralLayer)
-                if Activation[index] == 'relu':
+                if Activations[index] == 'relu':
                         NeuralLayer = Relu(NeuralLayer)
-                elif Activation[index] == 'sigmoid':
+                elif Activations[index] == 'sigmoid':
                         NeuralLayer = Sigmoid(NeuralLayer)
-                elif Activation[index] == 'softmax':
+                elif Activations[index] == 'softmax':
                         NeuralLayer = Softmax(NeuralLayer)
                         
                 if Layers[index] == 'fex':
                     NeuralLayer,useless = Fex(NeuralLayer, W[index], ThresholdSigns[index], ThresholdValues[index])
                 if Layers[index] == 'cat':
                     NeuralLayer,useless = Cat(NeuralLayer, W[index], ThresholdSigns[index], ThresholdValues[index],0)
             for i, w in enumerate(Wc):
@@ -672,15 +672,15 @@
              ThresholdSigns,
              ThresholdValues,
              Normalizations,
              Activations,
              TestAcc,
              LogType,
              WeightsType,
-             WeightFormat,
+             WeightsFormat,
              SavePath,
              W
  ):
     
     infoSavePLAN = """
     Function to save a deep learning model.
 
@@ -711,15 +711,15 @@
         print(Fore.RED + "ERROR109: Save Log Type (File Extension) must be 'csv' or 'txt' or 'hdf5' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
     if WeightsType != 'txt' and  WeightsType != 'npy' and WeightsType != 'mat':
         print(Fore.RED + "ERROR110: Save Weight type (File Extension) Type must be 'txt' or 'npy' or 'mat' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
-    if WeightFormat != 'd' and  WeightFormat != 'f' and WeightFormat != 'raw':
+    if WeightsFormat != 'd' and  WeightsFormat != 'f' and WeightsFormat != 'raw':
         print(Fore.RED + "ERROR111: Weight Format Type must be 'd' or 'f' or 'raw' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
     NeuronCount = 0
     SynapseCount = 0
     try:
         for w in W:
@@ -743,15 +743,15 @@
             'NORMALIZATION': Normalizations,
             'ACTIVATIONS': Activations,
             'NEURON COUNT': NeuronCount,
             'SYNAPSE COUNT': SynapseCount,
             'TEST ACCURACY': TestAcc,
             'SAVE DATE': datetime.now(),
             'WEIGHTS TYPE': WeightsType,
-            'WEIGHTS FORMAT': WeightFormat,
+            'WEIGHTS FORMAT': WeightsFormat,
             'SAVE PATH': SavePath
             }
     try:
         
         df = pd.DataFrame(data)
         
         if  LogType == 'csv':
@@ -768,65 +768,65 @@
             
     except:
         
         print(Fore.RED + "ERROR: Model log not saved. Check the log parameters from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     try:
         
-        if WeightsType == 'txt' and WeightFormat == 'd':
+        if WeightsType == 'txt' and WeightsFormat == 'd':
             
             for i, w in enumerate(W):
                 np.savetxt(SavePath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%d')
                 
-        if WeightsType == 'txt' and WeightFormat == 'f':
+        if WeightsType == 'txt' and WeightsFormat == 'f':
              
             for i, w in enumerate(W):
                  np.savetxt(SavePath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%f')
         
-        if WeightsType == 'txt' and WeightFormat == 'raw':
+        if WeightsType == 'txt' and WeightsFormat == 'raw':
             
             for i, w in enumerate(W):
                 np.savetxt(SavePath + ModelName +  str(i+1) + 'w.txt' ,  w)
             
                 
         ###
         
         
-        if WeightsType == 'npy' and WeightFormat == 'd':
+        if WeightsType == 'npy' and WeightsFormat == 'd':
             
             for i, w in enumerate(W):
                 np.save(SavePath + ModelName + str(i+1) + 'w.npy', w.astype(int))
         
-        if WeightsType == 'npy' and WeightFormat == 'f':
+        if WeightsType == 'npy' and WeightsFormat == 'f':
              
             for i, w in enumerate(W):
                  np.save(SavePath + ModelName +  str(i+1) + 'w.npy' ,  w, w.astype(float))
         
-        if WeightsType == 'npy' and WeightFormat == 'raw':
+        if WeightsType == 'npy' and WeightsFormat == 'raw':
             
             for i, w in enumerate(W):
                 np.save(SavePath + ModelName +  str(i+1) + 'w.npy' ,  w)
                 
            
         ###
         
          
-        if WeightsType == 'mat' and WeightFormat == 'd':
+        if WeightsType == 'mat' and WeightsFormat == 'd':
             
             for i, w in enumerate(W):
                 w = {'w': w.astype(int)}
                 io.savemat(SavePath + ModelName + str(i+1) + 'w.mat', w)
     
-        if WeightsType == 'mat' and WeightFormat == 'f':
+        if WeightsType == 'mat' and WeightsFormat == 'f':
              
             for i, w in enumerate(W):
                 w = {'w': w.astype(float)}
                 io.savemat(SavePath + ModelName + str(i+1) + 'w.mat', w)
         
-        if WeightsType == 'mat' and WeightFormat == 'raw':
+        if WeightsType == 'mat' and WeightsFormat == 'raw':
             
             for i, w in enumerate(W):
                 w = {'w': w}
                 io.savemat(SavePath + ModelName + str(i+1) + 'w.mat', w)
             
     except:
         
@@ -904,15 +904,15 @@
            W[i] = np.load(LoadPath + ModelName + str(i+1) + 'w.npy')
    elif WeightType == 'mat':
        for i in range(LayerCount):  
            W[i] = sio.loadmat(LoadPath + ModelName + str(i+1) + 'w.mat')
    else:
         raise ValueError(Fore.RED + "Incorrect weight type value. Value must be 'txt', 'npy' or 'mat' from: LoadPLAN."  + infoLoadPLAN + Style.RESET_ALL)
    print(Fore.GREEN + "Model loaded succesfully" + Style.RESET_ALL)     
-   return W,Layers,ThresholdSigns,ThresholdValues,Normalization,Activations,df
+   return W,Layers,ThresholdSigns,ThresholdValues,Normalizations,Activations,df
 
 def PredictFromDiscPLAN(Input,ModelName,ModelPath,LogType):
     infoPredictFromDİscPLAN = """
     Function to make a prediction using a divided pruning deep learning neural network (PLAN).
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
```

