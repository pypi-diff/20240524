# Comparing `tmp/daalab-0.7.tar.gz` & `tmp/daalab-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daalab-0.7.tar", last modified: Thu May 23 17:14:18 2024, max compression
+gzip compressed data, was "daalab-0.8.tar", last modified: Fri May 24 03:13:56 2024, max compression
```

## Comparing `daalab-0.7.tar` & `daalab-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 17:14:18.185375 daalab-0.7/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 17:14:18.185206 daalab-0.7/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.7/README.md
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 17:14:18.184199 daalab-0.7/daalab/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    32333 2024-05-23 17:13:13.000000 daalab-0.7/daalab/__init__.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    23663 2024-05-23 14:30:55.000000 daalab-0.7/daalab/codes.py
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       28 2024-05-23 17:12:47.000000 daalab-0.7/daalab/testing.py
-drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-23 17:14:18.185028 daalab-0.7/daalab.egg-info/
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-23 17:14:18.000000 daalab-0.7/daalab.egg-info/PKG-INFO
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-23 17:14:18.000000 daalab-0.7/daalab.egg-info/SOURCES.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-23 17:14:18.000000 daalab-0.7/daalab.egg-info/dependency_links.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-23 17:14:18.000000 daalab-0.7/daalab.egg-info/top_level.txt
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-23 17:14:18.185427 daalab-0.7/setup.cfg
--rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-23 17:13:34.000000 daalab-0.7/setup.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-24 03:13:56.298195 daalab-0.8/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-24 03:13:56.298066 daalab-0.8/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      568 2024-05-23 10:49:22.000000 daalab-0.8/README.md
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-24 03:13:56.297270 daalab-0.8/daalab/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    32333 2024-05-23 17:13:13.000000 daalab-0.8/daalab/__init__.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)    25107 2024-05-24 03:12:46.000000 daalab-0.8/daalab/codes.py
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)     1363 2024-05-24 02:29:40.000000 daalab-0.8/daalab/testing.py
+drwxr-xr-x   0 mohammedimaduddin   (501) staff       (20)        0 2024-05-24 03:13:56.297865 daalab-0.8/daalab.egg-info/
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      211 2024-05-24 03:13:56.000000 daalab-0.8/daalab.egg-info/PKG-INFO
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      191 2024-05-24 03:13:56.000000 daalab-0.8/daalab.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        1 2024-05-24 03:13:56.000000 daalab-0.8/daalab.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)        7 2024-05-24 03:13:56.000000 daalab-0.8/daalab.egg-info/top_level.txt
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)       38 2024-05-24 03:13:56.298250 daalab-0.8/setup.cfg
+-rw-r--r--   0 mohammedimaduddin   (501) staff       (20)      269 2024-05-24 03:12:52.000000 daalab-0.8/setup.py
```

### Comparing `daalab-0.7/README.md` & `daalab-0.8/README.md`

 * *Files identical despite different names*

### Comparing `daalab-0.7/daalab/__init__.py` & `daalab-0.8/daalab/__init__.py`

 * *Files identical despite different names*

### Comparing `daalab-0.7/daalab/codes.py` & `daalab-0.8/daalab/codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,20 +206,20 @@
         return self.graph[vertex]
 
 def graph_coloring(graph):
     colors = {}
     vertices = graph.get_vertices()
     for vertex in vertices:
         neighbors = graph.get_neighbors(vertex)
-        available_colors = set(range(len(vertices)))  # All colors available initially
+        available_colors = set(range(len(vertices))) 
         for neighbor in neighbors:
             if neighbor in colors:
-                available_colors.discard(colors[neighbor])  # Remove color of neighbor if it's already assigned
+                available_colors.discard(colors[neighbor])  
         if available_colors:
-            colors[vertex] = min(available_colors)  # Assign the minimum available color
+            colors[vertex] = min(available_colors) 
         else:
             raise ValueError("No available colors for vertex: " + str(vertex))
     return colors
 
 def main():
     graph = Graph()
     
@@ -240,37 +240,79 @@
 if __name__ == "__main__":
     main()'''
     print(code)
 
 
 def print_matrixchain():
     code = '''import sys
+from typing import List
 
-def matrix_chain_order(p, i, j):
+def matrix_chain_order(p: List[int], n: int) -> tuple[List[List[int]], List[List[int]]]:
+    """
+    Compute the minimum number of scalar multiplications needed to compute the matrix
+    chain product A[i]A[i+1]...A[j] and the optimal order of multiplication.
+
+    Args:
+        p (List[int]): List of dimensions of the matrices.
+        n (int): Number of matrices.
+
+    Returns:
+        Tuple[List[List[int]], List[List[int]]]: m and s matrices, where m[i][j] stores the minimum
+        number of scalar multiplications needed to compute the matrix chain product A[i]A[i+1]...A[j],
+        and s[i][j] stores the index of the optimal split point in the subproblem.
+    """
+    m = [[0 for x in range(n)] for y in range(n)]
+    s = [[0 for x in range(n)] for y in range(n)]
+
+    for length in range(2, n):
+        for i in range(1, n - length + 1):
+            j = i + length - 1
+            m[i][j] = sys.maxsize
+
+            for k in range(i, j):
+                q = m[i][k] + m[k + 1][j] + p[i - 1] * p[k] * p[j]
+                if q < m[i][j]:
+                    m[i][j] = q
+                    s[i][j] = k
+
+    return m, s
+
+def print_optimal_order(s: List[List[int]], i: int, j: int) -> None:
+    """
+    Print the optimal order of matrix multiplication for A[i]A[i+1]...A[j].
+
+    Args:
+        s (List[List[int]]): The s matrix computed by matrix_chain_order function.
+        i (int): Start index of the matrix chain.
+        j (int): End index of the matrix chain.
+    """
     if i == j:
-        return 0
+        print(f"A{i}", end="")
+    else:
+        print("(", end="")
+        print_optimal_order(s, i, s[i][j])
+        print_optimal_order(s, s[i][j] + 1, j)
+        print(")", end="")
 
-    min_cost = sys.maxsize
-    
-    for k in range(i, j):
-        count = (matrix_chain_order(p, i, k) +
-                 matrix_chain_order(p, k + 1, j) +
-                 p[i-1] * p[k] * p[j])
-
-        if count < min_cost:
-            min_cost = count
-    
-    return min_cost
+# Input number of matrices
+n = int(input("Enter the number of matrices: ")) + 1
 
-n = int(input("Enter the number of matrices: "))
+# Input the dimensions of matrices
 matrix_dims = list(map(int, input("Enter the dimensions of matrices separated by spaces: ").split()))
 
-min_multiplications = matrix_chain_order(matrix_dims, 0, n - 1)
+# Get the order and the minimum number of multiplications
+m, s = matrix_chain_order(matrix_dims, n)
+
+print("Minimum number of multiplications is", m[1][n - 1])
+print("Optimal order of multiplication is: ", end="")
+print_optimal_order(s, 1, n - 1)
+print()
+
 
-print("Minimum number of multiplications is", min_multiplications)'''
+mcm code'''
     print(code)
 
 
 def print_tspbb():
     code = '''# Python3 program to solve
 # Traveling Salesman Problem using
 # Branch and Bound.
@@ -823,15 +865,15 @@
         break
     temp = edge.split()
     if len(temp) == 3:
         u, v, w = temp
     elif len(temp) == 1:
         graph[temp[0]] = {}
     w = int(w)
-   if u not in graph:
+    if u not in graph:
         graph[u] = {}
     if v not in graph:
         graph[v] = {}
     graph[u][v] = w
 print(graph)
 source = input("enter source - ")
```

