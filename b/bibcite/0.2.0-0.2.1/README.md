# Comparing `tmp/bibcite-0.2.0.tar.gz` & `tmp/bibcite-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibcite-0.2.0.tar", last modified: Thu May 23 18:17:33 2024, max compression
+gzip compressed data, was "bibcite-0.2.1.tar", last modified: Thu May 23 22:18:20 2024, max compression
```

## Comparing `bibcite-0.2.0.tar` & `bibcite-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 18:17:33.500467 bibcite-0.2.0/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      905 2024-05-23 18:17:33.500467 bibcite-0.2.0/PKG-INFO
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 18:17:33.500467 bibcite-0.2.0/bibcite/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-05-23 17:02:29.000000 bibcite-0.2.0/bibcite/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      919 2024-05-23 18:16:53.000000 bibcite-0.2.0/bibcite/cli.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5223 2024-05-23 18:13:37.000000 bibcite-0.2.0/bibcite/work.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 18:17:33.500467 bibcite-0.2.0/bibcite.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      905 2024-05-23 18:17:33.000000 bibcite-0.2.0/bibcite.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      280 2024-05-23 18:17:33.000000 bibcite-0.2.0/bibcite.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-23 18:17:33.000000 bibcite-0.2.0/bibcite.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-05-23 18:17:33.000000 bibcite-0.2.0/bibcite.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-05-23 18:17:33.000000 bibcite-0.2.0/bibcite.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2024-05-23 18:17:33.000000 bibcite-0.2.0/bibcite.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      393 2024-05-23 18:16:47.000000 bibcite-0.2.0/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      585 2024-05-23 18:16:35.000000 bibcite-0.2.0/readme.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       27 2024-05-23 17:01:23.000000 bibcite-0.2.0/requirements.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-05-23 18:17:33.500467 bibcite-0.2.0/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 22:18:20.490246 bibcite-0.2.1/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      905 2024-05-23 22:18:20.490246 bibcite-0.2.1/PKG-INFO
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 22:18:20.490246 bibcite-0.2.1/bibcite/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-05-23 17:02:29.000000 bibcite-0.2.1/bibcite/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      919 2024-05-23 18:16:53.000000 bibcite-0.2.1/bibcite/cli.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5252 2024-05-23 22:17:15.000000 bibcite-0.2.1/bibcite/work.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-23 22:18:20.490246 bibcite-0.2.1/bibcite.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      905 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      280 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2024-05-23 22:18:20.000000 bibcite-0.2.1/bibcite.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      393 2024-05-23 22:18:05.000000 bibcite-0.2.1/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      585 2024-05-23 18:16:35.000000 bibcite-0.2.1/readme.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       27 2024-05-23 17:01:23.000000 bibcite-0.2.1/requirements.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-05-23 22:18:20.490246 bibcite-0.2.1/setup.cfg
```

### Comparing `bibcite-0.2.0/PKG-INFO` & `bibcite-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibcite
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate bibtex citations from command line and instantly copies them to clipboard
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pyperclip
 Requires-Dist: tabulate
```

### Comparing `bibcite-0.2.0/bibcite/cli.py` & `bibcite-0.2.1/bibcite/cli.py`

 * *Files identical despite different names*

### Comparing `bibcite-0.2.0/bibcite/work.py` & `bibcite-0.2.1/bibcite/work.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,28 @@
         if work_type:
             relevant_papers = [p for p in relevant_papers if p['type'] == work_type]
         if author:
             relevant_papers = [p for p in relevant_papers if author in cls.get_author(p)]
         if len(relevant_papers) == 0:
             raise ValueError(f"No papers found with title {title} and author {author}")
 
-        paper_doi = relevant_papers[0]['doi']
-
         # print(f'Crossref item = {cls.get_crossref_item(paper_doi)}')
-
-        crossref_item = cls.get_crossref_item(paper_doi=paper_doi)
+        crossref_item = cls.get_crossref_item(paper_doi=relevant_papers[0]['doi'])
         journal_item = crossref_item.get('container-title')
         if journal_item:
             journal = journal_item[0]
         else:
             journal = None
 
         # print(f'Found crossref item = {crossref_item}')
 
         new_work = Work(title= crossref_item['title'][0],
                         authors= crossref_item['author'],
                         year=crossref_item['published']['date-parts'][0][0],
-                        doi=paper_doi,
+                        doi=crossref_item['DOI'],
                         url= crossref_item['URL'],
                         work_type= crossref_item['type'],
                         journal=journal,
                         pages= crossref_item.get('page'),
                         volume= crossref_item.get('volume'))
         return new_work
 
@@ -137,13 +134,14 @@
 
 if __name__ == "__main__":
     # Error titles: Titles for which currently no citation can be generated
     # -> t1: Missing author
     # -> t2: DOI not found in Crossref
     t1 = "Fundamentals of Powder Diffraction and Structural Characterization of Materials"
     t2 = "Attention is all you need"
-    introd_work = Work.from_query(title=t1)
+    t3 = 'Supernova limits on muonic dark forces'
+    introd_work = Work.from_query(title=t3)
     print(f'Paper doi is {introd_work.doi}')
     print(f'Intro work bibtext = \n{introd_work.to_bibtex()}')
     # print(Work.get_crossref_item(paper_doi='10.1063/1.2807734'))
```

### Comparing `bibcite-0.2.0/bibcite.egg-info/PKG-INFO` & `bibcite-0.2.1/bibcite.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibcite
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate bibtex citations from command line and instantly copies them to clipboard
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pyperclip
 Requires-Dist: tabulate
```

### Comparing `bibcite-0.2.0/readme.md` & `bibcite-0.2.1/readme.md`

 * *Files identical despite different names*

