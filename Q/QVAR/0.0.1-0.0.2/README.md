# Comparing `tmp/QVAR-0.0.1.tar.gz` & `tmp/qvar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QVAR-0.0.1.tar", last modified: Thu Nov 30 20:21:05 2023, max compression
+gzip compressed data, was "qvar-0.0.2.tar", last modified: Fri May 24 12:50:26 2024, max compression
```

## Comparing `QVAR-0.0.1.tar` & `qvar-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-11-30 20:21:05.884274 QVAR-0.0.1/
--rw-r--r--   0 alessandro   (501) staff       (20)       76 2023-11-30 20:21:05.884052 QVAR-0.0.1/PKG-INFO
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-11-30 20:21:05.883222 QVAR-0.0.1/QVAR/
--rw-r--r--   0 alessandro   (501) staff       (20)       22 2023-11-30 20:11:34.000000 QVAR-0.0.1/QVAR/__init__.py
--rw-r--r--   0 alessandro   (501) staff       (20)     4277 2023-11-30 18:45:48.000000 QVAR-0.0.1/QVAR/qvar.py
--rw-r--r--   0 alessandro   (501) staff       (20)     2463 2023-11-30 18:57:20.000000 QVAR-0.0.1/QVAR/test.py
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-11-30 20:21:05.883883 QVAR-0.0.1/QVAR.egg-info/
--rw-r--r--   0 alessandro   (501) staff       (20)       76 2023-11-30 20:21:05.000000 QVAR-0.0.1/QVAR.egg-info/PKG-INFO
--rw-r--r--   0 alessandro   (501) staff       (20)      173 2023-11-30 20:21:05.000000 QVAR-0.0.1/QVAR.egg-info/SOURCES.txt
--rw-r--r--   0 alessandro   (501) staff       (20)        1 2023-11-30 20:21:05.000000 QVAR-0.0.1/QVAR.egg-info/dependency_links.txt
--rw-r--r--   0 alessandro   (501) staff       (20)        5 2023-11-30 20:21:05.000000 QVAR-0.0.1/QVAR.egg-info/top_level.txt
--rw-r--r--   0 alessandro   (501) staff       (20)     2288 2023-11-30 19:01:28.000000 QVAR-0.0.1/README.md
--rw-r--r--   0 alessandro   (501) staff       (20)       38 2023-11-30 20:21:05.884317 QVAR-0.0.1/setup.cfg
--rw-r--r--   0 alessandro   (501) staff       (20)      132 2023-11-30 20:15:38.000000 QVAR-0.0.1/setup.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2024-05-24 12:50:26.848768 qvar-0.0.2/
+-rw-r--r--   0 alessandro   (501) staff       (20)       76 2024-05-24 12:50:26.848581 qvar-0.0.2/PKG-INFO
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2024-05-24 12:50:26.847540 qvar-0.0.2/QVAR/
+-rw-r--r--   0 alessandro   (501) staff       (20)       22 2024-05-24 12:46:48.000000 qvar-0.0.2/QVAR/__init__.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     4027 2024-05-24 12:46:48.000000 qvar-0.0.2/QVAR/qvar.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     2452 2024-05-24 12:46:48.000000 qvar-0.0.2/QVAR/test.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2024-05-24 12:50:26.848413 qvar-0.0.2/QVAR.egg-info/
+-rw-r--r--   0 alessandro   (501) staff       (20)       76 2024-05-24 12:50:26.000000 qvar-0.0.2/QVAR.egg-info/PKG-INFO
+-rw-r--r--   0 alessandro   (501) staff       (20)      173 2024-05-24 12:50:26.000000 qvar-0.0.2/QVAR.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)        1 2024-05-24 12:50:26.000000 qvar-0.0.2/QVAR.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)        5 2024-05-24 12:50:26.000000 qvar-0.0.2/QVAR.egg-info/top_level.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)     2288 2023-11-30 19:01:28.000000 qvar-0.0.2/README.md
+-rw-r--r--   0 alessandro   (501) staff       (20)       38 2024-05-24 12:50:26.848812 qvar-0.0.2/setup.cfg
+-rw-r--r--   0 alessandro   (501) staff       (20)      132 2024-05-24 12:49:32.000000 qvar-0.0.2/setup.py
```

### Comparing `QVAR-0.0.1/QVAR/qvar.py` & `qvar-0.0.2/QVAR/qvar.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,69 +25,61 @@
 
 def QVAR(U, var_index=None, ps_index=None, version='FAE', delta=0.0001, max_iter=5, eval_qbits=5, shots=8192, n_h_gates=0, postprocessing=True):
 
     if var_index is None:
         var_index = [x for x in range(U.num_qubits)]
     
     i_qbits = len(var_index)
-    q_qbits = e_qbits = i_qbits
+    e_qbits = i_qbits
     u_qbits = U.num_qubits
 
     a = QuantumRegister(1,'a')
     e = QuantumRegister(e_qbits,'e')
-    q = QuantumRegister(q_qbits,'q')
     u = QuantumRegister(u_qbits, 'u')
 
     if version == 'SHOTS':
         ca = ClassicalRegister(1,'ca')
-        cq = ClassicalRegister(q_qbits,'cq')
         ce = ClassicalRegister(e_qbits,'ce')
         if ps_index is not None:
             cps = ClassicalRegister(len(ps_index), 'cps')
-            qc = QuantumCircuit(a, e, q, u, ca, cq, ce, cps)
+            qc = QuantumCircuit(a, e, u, ca, ce, cps)
         else:
-            qc = QuantumCircuit(a, e, q, u, ca, cq, ce)
+            qc = QuantumCircuit(a, e, u, ca, ce)
     
     else:
-        qc = QuantumCircuit(a, e, q, u)
+        qc = QuantumCircuit(a, e, u)
 
-    qc.append(U.to_gate(), list(range(1+e_qbits+q_qbits, qc.num_qubits)))    
+    qc.append(U.to_gate(), list(range(1+e_qbits, qc.num_qubits)))    
     
     qc.h(a)
-    qc.cx(a,e)
-    qc.x(e)
 
     for t in range(i_qbits):
-        qc.cswap(a,q[t],u[var_index[t]])
+        qc.cswap(a,e[t],u[var_index[t]])
 
+    qc.ch(a,e)
     for t in range(i_qbits):
         qc.ch(a,u[var_index[t]])
         
-    qc.ch(a,e)
+    qc.x(e)    
     qc.h(a)
 
-    qc.h(q)
-
-    qc.x(q)
-    
     if ps_index is None:
-        objective_qubits = [x for x in range(1+e_qbits+q_qbits)]
+        objective_qubits = [x for x in range(1+e_qbits)]
     else:
-        objective_qubits = [x for x in range(1+e_qbits+q_qbits)]+[qc.num_qubits-u_qbits + x for x in ps_index]
+        objective_qubits = [x for x in range(1+e_qbits)]+[qc.num_qubits-u_qbits + x for x in ps_index]
 
     if version == 'SHOTS':
         qc.measure(a, ca) 
-        qc.measure(q, cq)
         qc.measure(e, ce)
         
         if ps_index is not None:
             qc.measure(u[ps_index], cps)
-            target_conf = '1'*len(ps_index) + ' ' + '1'*e_qbits + ' ' + '1'*q_qbits + ' 1' 
+            target_conf = '1'*len(ps_index) + ' ' + '1'*e_qbits + ' 1' 
         else:
-            target_conf = '1'*e_qbits + ' ' + '1'*q_qbits + ' 1'
+            target_conf = '1'*e_qbits + ' 1'
 
         backend = BasicAer.get_backend('qasm_simulator')
         counts = execute(qc, backend, shots=shots).result().get_counts(qc)
 
         try: 
             var = (counts[target_conf])/shots
         except:
@@ -123,12 +115,12 @@
             state_preparation=qc, 
             objective_qubits=objective_qubits,
         )
         fae_result = fae.estimate(problem)
         var = fae_result.estimation
         
     
-    tot_hadamard = 2 + i_qbits + n_h_gates
+    tot_hadamard = 2 + n_h_gates
     norm_factor = 2**tot_hadamard/2**i_qbits
 
     return var*norm_factor
```

### Comparing `QVAR-0.0.1/QVAR/test.py` & `qvar-0.0.2/QVAR/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,12 @@
 
     differences = [(q-c)**2 for q,c in zip(qu, cl)]
     print("MSE: " + str(np.mean(differences)))
 
 
 if __name__ == "__main__":
 
-    
-    
-
     print("\n RANDOM UNITARY TEST \n")
     test_random_U(2)
 
     print("\n FF-QRAM TEST \n")
     test_ffqram(8)
```

### Comparing `QVAR-0.0.1/README.md` & `qvar-0.0.2/README.md`

 * *Files identical despite different names*

