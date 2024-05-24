# Comparing `tmp/clar_cloc-0.1.0.tar.gz` & `tmp/clar_cloc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clar_cloc-0.1.0.tar", last modified: Wed May 22 20:22:21 2024, max compression
+gzip compressed data, was "clar_cloc-0.1.1.tar", last modified: Fri May 24 14:16:42 2024, max compression
```

## Comparing `clar_cloc-0.1.0.tar` & `clar_cloc-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2024-05-22 20:22:21.678663 clar_cloc-0.1.0/
--rw-r--r--   0 chris      (502) staff       (20)      972 2024-05-22 20:22:21.678455 clar_cloc-0.1.0/PKG-INFO
--rw-r--r--   0 chris      (502) staff       (20)      444 2024-05-22 19:59:45.000000 clar_cloc-0.1.0/README.md
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2024-05-22 20:22:21.676859 clar_cloc-0.1.0/clar_cloc/
--rw-r--r--   0 chris      (502) staff       (20)        0 2024-05-22 14:29:45.000000 clar_cloc-0.1.0/clar_cloc/__init__.py
--rw-r--r--   0 chris      (502) staff       (20)      487 2024-05-22 20:20:11.000000 clar_cloc-0.1.0/clar_cloc/cli.py
--rw-r--r--   0 chris      (502) staff       (20)     3570 2024-05-22 19:52:09.000000 clar_cloc-0.1.0/clar_cloc/count.py
-drwxr-xr-x   0 chris      (502) staff       (20)        0 2024-05-22 20:22:21.678196 clar_cloc-0.1.0/clar_cloc.egg-info/
--rw-r--r--   0 chris      (502) staff       (20)      972 2024-05-22 20:22:21.000000 clar_cloc-0.1.0/clar_cloc.egg-info/PKG-INFO
--rw-r--r--   0 chris      (502) staff       (20)      276 2024-05-22 20:22:21.000000 clar_cloc-0.1.0/clar_cloc.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (502) staff       (20)        1 2024-05-22 20:22:21.000000 clar_cloc-0.1.0/clar_cloc.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (502) staff       (20)       49 2024-05-22 20:22:21.000000 clar_cloc-0.1.0/clar_cloc.egg-info/entry_points.txt
--rw-r--r--   0 chris      (502) staff       (20)       26 2024-05-22 20:22:21.000000 clar_cloc-0.1.0/clar_cloc.egg-info/requires.txt
--rw-r--r--   0 chris      (502) staff       (20)       10 2024-05-22 20:22:21.000000 clar_cloc-0.1.0/clar_cloc.egg-info/top_level.txt
--rw-r--r--   0 chris      (502) staff       (20)       38 2024-05-22 20:22:21.678700 clar_cloc-0.1.0/setup.cfg
--rw-r--r--   0 chris      (502) staff       (20)      836 2024-05-22 20:21:36.000000 clar_cloc-0.1.0/setup.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2024-05-24 14:16:42.367341 clar_cloc-0.1.1/
+-rw-r--r--   0 chris      (502) staff       (20)      972 2024-05-24 14:16:42.366820 clar_cloc-0.1.1/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)      444 2024-05-22 19:59:45.000000 clar_cloc-0.1.1/README.md
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2024-05-24 14:16:42.365554 clar_cloc-0.1.1/clar_cloc/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2024-05-22 14:29:45.000000 clar_cloc-0.1.1/clar_cloc/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)      770 2024-05-24 13:15:50.000000 clar_cloc-0.1.1/clar_cloc/cli.py
+-rw-r--r--   0 chris      (502) staff       (20)     5110 2024-05-24 14:14:45.000000 clar_cloc-0.1.1/clar_cloc/count.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2024-05-24 14:16:42.366625 clar_cloc-0.1.1/clar_cloc.egg-info/
+-rw-r--r--   0 chris      (502) staff       (20)      972 2024-05-24 14:16:42.000000 clar_cloc-0.1.1/clar_cloc.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)      276 2024-05-24 14:16:42.000000 clar_cloc-0.1.1/clar_cloc.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (502) staff       (20)        1 2024-05-24 14:16:42.000000 clar_cloc-0.1.1/clar_cloc.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (502) staff       (20)       49 2024-05-24 14:16:42.000000 clar_cloc-0.1.1/clar_cloc.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (502) staff       (20)       26 2024-05-24 14:16:42.000000 clar_cloc-0.1.1/clar_cloc.egg-info/requires.txt
+-rw-r--r--   0 chris      (502) staff       (20)       10 2024-05-24 14:16:42.000000 clar_cloc-0.1.1/clar_cloc.egg-info/top_level.txt
+-rw-r--r--   0 chris      (502) staff       (20)       38 2024-05-24 14:16:42.367384 clar_cloc-0.1.1/setup.cfg
+-rw-r--r--   0 chris      (502) staff       (20)      836 2024-05-24 14:16:37.000000 clar_cloc-0.1.1/setup.py
```

### Comparing `clar_cloc-0.1.0/PKG-INFO` & `clar_cloc-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clar-cloc
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI tool to count lines in Clarity (.clar) files
 Home-page: https://github.com/yourusername/clar_cloc
 Author: Kristian Apostolov
 Author-email: kristianapostolovcontacts@gmail.com
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clar_cloc-0.1.0/clar_cloc/count.py` & `clar_cloc-0.1.1/clar_cloc/count.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 
 from typing import List, Tuple, Optional
 
 # Types:
 Total = Tuple[int, int, int] # source, blank, comment
 Totals = Tuple[int, int, int, int]  # source, blank, comment, count
 Results = List[List] # relative path, source, blank, comment
+ResultTables = Tuple[str, str]
 
 # Constants:
 #  -> Clarity:
 BLANK: str = ""
 COMMENT: str = ";;"
 FILE_EXTENSION: str = ".clar"
 
 #  -> Output:
-TABLE_HEADERS: List[str] = ["File", "Source lines", "Blank lines", "Comment lines"]
+TABLE_HEADERS: List[str] = ["File", "Source", "Blank", "Comment"]
 TABLE_FORMAT: str = "rounded_grid"
+MD_TABLE_FORMAT: str = "github"
 
 # -> Errors:
 ERROR_DIRECTORY_NOT_FOUND: str = "Directory not found"
 ERROR_FILE_NOT_FOUND: str = "File not found"
 ERROR_READING_DIRECTORY: str = "An error occurred while reading directory"
 ERROR_READING_FILE: str = "An error occurred while reading file"
+ERROR_WRITING_FILE: str = "An error occurred while writing to file"
 ERROR_NO_FILES_FOUND: str = f"No {FILE_EXTENSION} files found"
 
 
 def error(message: str, var: Optional[str] = None) -> None:
     """
         Raise an exception with a formatted error message.
     """
@@ -44,49 +47,78 @@
         """
             Clojure function to identify the line type and increment the corresponding counter.
         """
         nonlocal source, blank, comment
         if line == BLANK: blank += 1
         elif line.startswith(COMMENT): comment += 1
         else: source += 1
-    
-    for file in open(path, "r"): _count_line(file.strip())
+
+    for line in open(path, "r"): _count_line(line.strip())
 
     return source, blank, comment
 
 def count_lines(path: str) -> Total:
     """
         Wrapper function to return the file's data or raise an appropriate error.
     """
     try: return _count_lines(path)
     
     except FileNotFoundError: error(ERROR_FILE_NOT_FOUND, path)
     except IOError: error(ERROR_READING_FILE, path)
 
+def generate_tables(results: Results, totals: Totals, format: str) -> ResultTables:
+    """
+        Generate the tables for the console output.
+    """
+    file_results: str = tabulate(results, headers=TABLE_HEADERS, tablefmt=format)
+    totals_row = [["Total", totals[0], totals[1], totals[2]]]
+    totals_results: str = tabulate(totals_row, headers=TABLE_HEADERS, tablefmt=format)
+    
+    return file_results, totals_results
+
 def log(results: Results, totals: Totals) -> None:
     """
         Function to output the directory's metrics, or raise an error if no files were found.
     """
     
     if not results: error(ERROR_NO_FILES_FOUND)
+    
+    file_results, totals_results = generate_tables(results, totals, TABLE_FORMAT)
+    
+    # Log to console
+    print(file_results, totals_results, f"Total files processed: {totals[3]}", sep="\n\n")
+    
+def log_scope(files: List[str], tables: ResultTables, markdown: str, include_breakdowns: bool) -> None:
+    """
+        Log the scope of the project to a markdown file.
+    """
+    
+    # Log to markdown file
+    try:
+        md = open(markdown, "w")
+        md.write(f"clar-cloc Report\n\n")
+        if include_breakdowns:
+            md.write(f"Files\n\n{tables[0]}\n\n")
+            md.write(f"Totals\n\n{tables[1]}\n\n")
+        else:
+            plain_table: str = tabulate([files], [TABLE_HEADERS[0]], tablefmt=MD_TABLE_FORMAT)
+            md.write(f"Files\n\n{plain_table}\n\n")
+            
+        md.write(f"Total files processed: {len(files)}\n")
         
-    print(tabulate(results, headers=TABLE_HEADERS, tablefmt=TABLE_FORMAT))
-
-    totals_row = [["Total", totals[0], totals[1], totals[2]]]
-    print(tabulate(totals_row, headers=TABLE_HEADERS, tablefmt=TABLE_FORMAT))
-    print(f"Total files processed: {totals[3]}")
+    except IOError: error(ERROR_WRITING_FILE, markdown)
     
-
-def process_directory(path: str, exclude: List[str]) -> None:
+def process_directory(path: str, exclude: List[str], markdown: str, include_breakdowns: bool) -> None:
     """
         Process the directory and its subdirectories, counting the lines of each file.
     """
     
     totals: Totals = (0, 0, 0, 0)
     results: Results = []
+    _files: List[str] = []
 
     try:
         for root, dirs, files in walk(path):
             # Skip directories that are in the exclude list
             dirs[:] = [d for d in dirs if join(root, d) not in exclude]
 
             for file in files:
@@ -100,11 +132,22 @@
                     totals[0] + counts[0],
                     totals[1] + counts[1],
                     totals[2] + counts[2],
                     totals[3] + 1
                 )
                 
                 results.append([relative, *counts])
+                _files.append(relative)
+                
         log(results, totals)
         
+        if not markdown: return None
+        
+        log_scope(
+            _files,
+            generate_tables(results, totals, MD_TABLE_FORMAT),
+            markdown,
+            include_breakdowns
+        )
+        
     except FileNotFoundError: error(ERROR_DIRECTORY_NOT_FOUND, path)
     except IOError: error(ERROR_READING_DIRECTORY, path)
```

### Comparing `clar_cloc-0.1.0/clar_cloc.egg-info/PKG-INFO` & `clar_cloc-0.1.1/clar_cloc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clar-cloc
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI tool to count lines in Clarity (.clar) files
 Home-page: https://github.com/yourusername/clar_cloc
 Author: Kristian Apostolov
 Author-email: kristianapostolovcontacts@gmail.com
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clar_cloc-0.1.0/setup.py` & `clar_cloc-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clar-cloc",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "click",
         "tabulate",
         "setuptools"
     ],
     entry_points={
```

