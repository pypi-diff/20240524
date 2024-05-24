# Comparing `tmp/orf_tools-0.0.1.tar.gz` & `tmp/orf_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orf_tools-0.0.1.tar", last modified: Fri Aug  4 14:12:15 2023, max compression
+gzip compressed data, was "orf_tools-0.0.3.tar", last modified: Thu May 23 16:21:34 2024, max compression
```

## Comparing `orf_tools-0.0.1.tar` & `orf_tools-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 14:12:15.318674 orf_tools-0.0.1/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      806 2023-08-04 14:12:15.318674 orf_tools-0.0.1/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      361 2023-08-04 14:09:57.000000 orf_tools-0.0.1/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2023-08-04 14:00:57.000000 orf_tools-0.0.1/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      830 2023-08-04 14:12:15.318674 orf_tools-0.0.1/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2023-08-04 14:00:57.000000 orf_tools-0.0.1/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 14:12:15.314674 orf_tools-0.0.1/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 14:12:15.318674 orf_tools-0.0.1/src/orf_tools/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       71 2023-08-04 14:03:04.000000 orf_tools-0.0.1/src/orf_tools/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-08-04 14:03:15.000000 orf_tools-0.0.1/src/orf_tools/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    15489 2023-08-04 14:02:52.000000 orf_tools-0.0.1/src/orf_tools/extend_orfs.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 14:12:15.318674 orf_tools-0.0.1/src/orf_tools.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      806 2023-08-04 14:12:15.000000 orf_tools-0.0.1/src/orf_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      308 2023-08-04 14:12:15.000000 orf_tools-0.0.1/src/orf_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-08-04 14:12:15.000000 orf_tools-0.0.1/src/orf_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       59 2023-08-04 14:12:15.000000 orf_tools-0.0.1/src/orf_tools.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       10 2023-08-04 14:12:15.000000 orf_tools-0.0.1/src/orf_tools.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-23 16:21:34.617241 orf_tools-0.0.3/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)      925 2024-05-23 16:21:34.617241 orf_tools-0.0.3/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      361 2023-08-04 14:09:57.000000 orf_tools-0.0.3/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2023-08-04 14:00:57.000000 orf_tools-0.0.3/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      830 2024-05-23 16:21:34.617241 orf_tools-0.0.3/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2023-08-04 14:00:57.000000 orf_tools-0.0.3/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-23 16:21:34.617241 orf_tools-0.0.3/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-23 16:21:34.617241 orf_tools-0.0.3/src/orf_tools/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       71 2023-08-04 14:03:04.000000 orf_tools-0.0.3/src/orf_tools/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2024-05-23 16:20:04.000000 orf_tools-0.0.3/src/orf_tools/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    16313 2024-05-23 16:14:06.000000 orf_tools-0.0.3/src/orf_tools/extend_orfs.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-23 16:21:34.617241 orf_tools-0.0.3/src/orf_tools.egg-info/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)      925 2024-05-23 16:21:34.000000 orf_tools-0.0.3/src/orf_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      308 2024-05-23 16:21:34.000000 orf_tools-0.0.3/src/orf_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2024-05-23 16:21:34.000000 orf_tools-0.0.3/src/orf_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       59 2024-05-23 16:21:34.000000 orf_tools-0.0.3/src/orf_tools.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       10 2024-05-23 16:21:34.000000 orf_tools-0.0.3/src/orf_tools.egg-info/top_level.txt
```

### Comparing `orf_tools-0.0.1/PKG-INFO` & `orf_tools-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: orf_tools
-Version: 0.0.1
+Version: 0.0.3
 Summary: Tools to work with open reading frames (ORFs)
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti and Joan Pallares
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: pyfaidx>=0.7.2
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: easyterm>=1.0.0
+Requires-Dist: numpy>=1.17.0
 
 # orf_tools
 
 Package to manipulate open reading frames (ORFs).
 
 Dependent on pandas.
```

### Comparing `orf_tools-0.0.1/setup.cfg` & `orf_tools-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `orf_tools-0.0.1/src/orf_tools/extend_orfs.py` & `orf_tools-0.0.3/src/orf_tools/extend_orfs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,133 +2,25 @@
 from pyfaidx import Fasta
 import pandas as pd, numpy as np
 from easyterm import write
 
 ## Joan Pallares started this function
 #  Marco Mariotti later optimized it, made it independent from pyranges
 
-# MM # efficients methods to work inplace. All methods with df as input have one row per CDS group
-def extend_df(df, direction, extension, selector):
-    """Inplace"""
-    if direction == "5":
-        df.loc[selector & (df.Strand == "+"), ["Start"]] -= extension
-        df.loc[selector & (df.Strand == "-"), ["End"]] += extension
-    elif direction == "3":
-        df.loc[selector & (df.Strand == "-"), ["Start"]] -= extension
-        df.loc[selector & (df.Strand == "+"), ["End"]] += extension
-
-def extend_groups(dfg, cds_id):
-    """In place, dfg may contain multiple exons"""
-    first_exon_indices=dfg.groupby(cds_id).apply(lambda x: x.index[0]).reset_index(drop=True)
-    last_exon_indices=dfg.groupby(cds_id).apply(lambda x: x.index[-1]).reset_index(drop=True)
-    sp = (dfg.Strand == "+")
-    sm = (dfg.Strand == "-")
-
-    dfg.loc[ sp[first_exon_indices], 'Start'] -= dfg.loc[ sp[first_exon_indices], '__extension_up']
-    dfg.loc[ sp[last_exon_indices], 'End'] += dfg.loc[ sp[last_exon_indices], '__extension_down']
-    dfg.loc[ sm[first_exon_indices], 'End'] += dfg.loc[ sm[first_exon_indices], '__extension_up']
-    dfg.loc[ sm[last_exon_indices], 'Start'] -= dfg.loc[ sm[last_exon_indices], '__extension_down']
-
-def get_seqs(df, fs, selector):
-    """ Creates/updates column __seq"""
-    seqs = []
-    d = df[selector]
-    for start, end, strand, chrom in zip(d.Start, d.End, d.Strand, d.Chromosome):
-        _fasta = fs[chrom]
-        if strand == "-":
-            seqs.append((-_fasta[start:end]).seq.upper())  # reverse complement
-        elif strand == "+":
-            seqs.append(_fasta[start:end].seq.upper())
-        else:
-            raise Exception()
-    df.loc[selector, "__seq"] = seqs
-
-def correct_bounds(df, adjust=None):
-    """ Like pyranges genome_bounds, inplace; but also:
-    adjust the 5' or 3' end of intervals so they are multiples of 3
-    and set boolean attribute __out_of_bounds"""
-    out_end = df["End"] > df["__chromsize"]
-    df.loc[out_end, "End"] = df.loc[out_end, ["End", "__chromsize"]].min(axis=1)
-    out_start = df["Start"] < 0
-    df.loc[out_start, "Start"] = 0
-
-    sp = (df.Strand == "+")
-    sm = (df.Strand == "-")
-
-    if adjust=='5':
-        df.loc[out_start & sp, "Start"] += (df.loc[out_start & sp, "End"] - df.loc[out_start & sp, "Start"]).mod(3)
-        df.loc[out_end & sm, "End"] -= (df.loc[out_end & sm, "End"] - df.loc[out_end & sm, "Start"]).mod(3)
-
-    elif adjust=='3':
-        df.loc[out_end & sp, "End"] -= (df.loc[out_end & sp, "End"] - df.loc[out_end & sp, "Start"]).mod(3)
-        df.loc[out_start & sm, "Start"] += (df.loc[out_start & sm, "End"] - df.loc[out_start & sm, "Start"]).mod(3)
-
-    df.loc[(out_end | out_start), '__out_of_bounds']= True
-
-def subseq_df(df, from_end, amount, selector):
-    """ Similar to pyranges subseq but inplace """
-    sp = selector & (df.Strand == "+")
-    sm = selector & (df.Strand == "-")
-    if from_end == "5":
-        df.loc[sp, "End"] = df.loc[sp, "Start"] + amount
-        df.loc[sm, "Start"] = df.loc[sm, "End"] - amount
-    elif from_end == "3":
-        df.loc[sp, "Start"] = df.loc[sp, "End"] - amount
-        df.loc[sm, "End"] = df.loc[sm, "Start"] + amount
-    else:
-        raise Exception()
-
-def find_rightmost_stop(seq, motifs):
-    """ Returns the distance from the end of the string
-       of the first codon position of the rightmost stop; e.g. 3 is for last codon"""
-    for i in range(len(seq)-3, -1, -3):
-        if seq[i:i+3] in motifs:
-            return len(seq)-i
-    return -1
-
-def find_leftmost_start(row, motifs, chunk_size):
-    """ Returns the distance from the end of the string
-    of the first codon position of the leftmost start AFTER the position in column __up_stop_dist"""
-    seq=row['__seq']
-    stop_pos=row['__up_stop_dist']
-    start_search=( ( 3 + len(seq)- (stop_pos % chunk_size) )
-                   if stop_pos!=-1 else 0)
-    # we search starting from the position next to the stop
-    for i in range(start_search,
-                   len(seq), 3):
-        if seq[i:i+3] in motifs:
-            return len(seq)-i
-    return -1
-
-def find_leftmost_stop(seq, motifs):
-    """ Returns the position (distance from the start of the string) 
-    of the third codon position of the leftmost stop; e.g. 3 is for the first codon """
-    for i in range(0, len(seq), 3):
-        if seq[i:i+3] in motifs:
-            return i+3
-    return -1
-
-def sort_intervals_by_5(df):
-    def select_column(row):
-        return row['Start'] if (row['Strand']=='+') else -(row['End'])
-
-    new_order=df.apply(select_column, axis=1).sort_values().index
-    df.iloc[:] = df.iloc[new_order]
-
 def extend_orfs(
-        p,
-        fasta_path,
-        group_id=None,
-        starts=["ATG"],
-        stops=["TAG", "TGA", "TAA"],
-        keep_off_bounds=False,
-        direction=["up", "down"],
-        chunk_size=900,
-        record_extensions=False,
-        verbose=False
+    p,
+    fasta_path,
+    group_id=None,
+    starts=["ATG"],
+    stops=["TAG", "TGA", "TAA"],
+    keep_off_bounds=False,
+    direction=["up", "down"],
+    chunk_size=900,
+    record_extensions=False,
+    verbose=False,
 ):
     """Extends PyRanges intervals to their next Start codon upstream
     and/or to their next Stop codon downstream.
 
     Parameters
     ----------
 
@@ -154,35 +46,39 @@
 
     direction : whether the extension should be upstream ('up'), downstream
         ('down') or both. Default ['up', 'down']
 
     chunk_size : the amount of nucleotides to be extended on each iteration.
         Default 900.
 
-    record_extensions : if True, add columns extension_up and extension_down 
+    record_extensions : if True, add columns extension_up and extension_down
         with the extensions amounts. Default: False
 
     verbose : prints messages
     """
+
     def pverbose(msg, how=None):
         if verbose:
             write(msg, how=how)
 
     # Sanity Checks
-    assert (chunk_size %3)==0 , "Chunk size must be a multiple of three."
-    assert all([len(pattern)==3 for pattern in starts + stops]), "Ensure that all patterns have a length of 3 nt."
-    p.Strand=pd.Categorical(p.Strand)
-    assert p.Strand.cat.categories.isin(['+', '-']).all(), \
-            "Intervals must be stranded! Ensure that the strand column exists and all values are + or -"
+    assert (chunk_size % 3) == 0, "Chunk size must be a multiple of three."
+    assert all(
+        [len(pattern) == 3 for pattern in starts + stops]
+    ), "Ensure that all patterns have a length of 3 nt."
+    p.Strand = pd.Categorical(p.Strand)
+    assert p.Strand.cat.categories.isin(
+        ["+", "-"]
+    ).all(), "Intervals must be stranded! Ensure that the strand column exists and all values are + or -"
 
     if group_id is None:
         cds_id = "Custom_ID"
         p[cds_id] = np.arange(len(p))  # Generates a New Column
     else:
-        cds_id=group_id
+        cds_id = group_id
 
     ##################
     # Show a warning if some transcript lengths are not divisible by 3:
     p["__length"] = p["End"] - p["Start"]
     module_3 = p.groupby(by=cds_id).__length.sum().mod(3)
     ndv = module_3[module_3 != 0].index
     # module_3 = p_df.groupby(by=cds_id).apply(lambda x: sum(x["length"]) % 3)
@@ -212,163 +108,332 @@
                 "Start": "min",
                 "End": "max",
                 "Chromosome": "first",
             }
         )
     )
     ncds = len(minp)
-    nexons= len(p)
+    nexons = len(p)
 
     # add chromosome sizes as column
     minp = minp.merge(
         pd.DataFrame(
             {
                 "Chromosome": [chrom for chrom, _ in fs.items()],
                 "__chromsize": [len(fs[chrom]) for chrom, _ in fs.items()],
             }
         ),
         on="Chromosome",
     ).set_index(cds_id)
 
-    assert len(minp) == ncds, "ERROR some sequences were not found in the pyfaidx object"
+    assert (
+        len(minp) == ncds
+    ), "ERROR some sequences were not found in the pyfaidx object"
 
     ######################  Extend Sequence Upstream ###########################
 
     if "up" in direction or "up" == direction:
         pup = minp.copy()
-        pup['__out_of_bounds']=False
-        pup['__up_stop_dist']=-1   # -1 means not found
-        pup['__up_start_dist']=-1  # -1 means not found
-        selector=pd.Series(True, index=pup.index) # initialized as all True; keeps track of intervals with work to do
-        ic = 0  #iteration counter
+        pup["__out_of_bounds"] = False
+        pup["__up_stop_dist"] = -1  # -1 means not found
+        pup["__up_start_dist"] = -1  # -1 means not found
+        selector = pd.Series(
+            True, index=pup.index
+        )  # initialized as all True; keeps track of intervals with work to do
+        ic = 0  # iteration counter
 
         while (selector).any():
-            pverbose(f'Upstream | iteration {ic},  left to do: {selector.sum()}', how='reverse')
-            pverbose(pup[selector], how='yellow')
+            pverbose(
+                f"Upstream | iteration {ic},  left to do: {selector.sum()}",
+                how="reverse",
+            )
+            pverbose(pup[selector], how="yellow")
             # selector= ... everything which is not done nor out of bounds
             extend_df(pup, "5", chunk_size, selector)
             subseq_df(pup, "5", chunk_size, selector)
-            correct_bounds(pup, adjust='5')
-            get_seqs(pup, fs, selector) # seqs length is only selector
+            correct_bounds(pup, adjust="5")
+            get_seqs(pup, fs, selector)  # seqs length is only selector
 
             ## looking for a stop if didn't find it already
-            z=pup.loc[   selector, 
-                      '__seq'].apply(lambda x: find_rightmost_stop(x, stops))
-            found_stop_selector=selector.copy()   # made to index pup
-            found_stop_selector[found_stop_selector]=(z!=-1)
-            pup.loc[found_stop_selector, '__up_stop_dist'] = z[z!=-1] + ic*chunk_size
+            z = pup.loc[selector, "__seq"].apply(
+                lambda x: find_rightmost_stop(x, stops)
+            )
+            found_stop_selector = selector.copy()  # made to index pup
+            to_fill = (z != -1)
+            to_fill= to_fill.values[0] if len(to_fill)==1 else to_fill
+            found_stop_selector[found_stop_selector] = to_fill
+            pup.loc[found_stop_selector, "__up_stop_dist"] = (
+                z[z != -1] + ic * chunk_size
+            )
 
             if keep_off_bounds:
                 # focus on intervals that reached out of bounds in this iteration and did not find a stop:
                 #  record their max extension as up_stop_dist and __up_start_dist so they are considered whether starts was provided or not
-                # btw this means these intervals can be identified by looking at rows with __up_start_dist == __up_stop_dist            
-                no_stop_off_bounds=found_stop_selector.copy()
-                no_stop_off_bounds[no_stop_off_bounds]=(z==-1)
-                pup.loc[no_stop_off_bounds, '__up_stop_dist']=(
-                    (pup.loc[no_stop_off_bounds, 'End']-pup.loc[no_stop_off_bounds, 'Start']) + ic*chunk_size
-                    )
-                pup.loc[no_stop_off_bounds, '__up_start_dist']=pup.loc[no_stop_off_bounds, '__up_stop_dist']
+                # btw this means these intervals can be identified by looking at rows with __up_start_dist == __up_stop_dist
+                no_stop_off_bounds = found_stop_selector.copy()
+                to_fill = (z == -1)
+                to_fill = to_fill.values[0] if len(to_fill)==1 else to_fill
+                no_stop_off_bounds[no_stop_off_bounds] = to_fill
+                pup.loc[no_stop_off_bounds, "__up_stop_dist"] = (
+                    pup.loc[no_stop_off_bounds, "End"]
+                    - pup.loc[no_stop_off_bounds, "Start"]
+                ) + ic * chunk_size
+                pup.loc[no_stop_off_bounds, "__up_start_dist"] = pup.loc[
+                    no_stop_off_bounds, "__up_stop_dist"
+                ]
 
             ## looking for a start
             if starts:
-                z=pup.loc[ selector,
-                           ['__seq', '__up_stop_dist'] ].apply(lambda x:find_leftmost_start(x, starts, chunk_size), axis=1)
+                z = pup.loc[selector, ["__seq", "__up_stop_dist"]].apply(
+                    lambda x: find_leftmost_start(x, starts, chunk_size), axis=1
+                )
                 ## if start is not found now, but was found in a previous iteration, the previous will be kept (not overwriting a -1)
-                found_start_selector=selector.copy()   # made to index pup
-                found_start_selector[found_start_selector]=(z!=-1)
-                pup.loc[found_start_selector, '__up_start_dist'] = z[z!=-1] + ic*chunk_size
-
-            pup.loc[found_stop_selector, '__seq']=''  ## frees memory
-            pverbose(' ---> After iteration:')
-            pverbose(pup[selector], how='reverse,yellow')
-
-            selector= (pup.__up_stop_dist==-1) & ~(pup.__out_of_bounds)
-            ic+=1
-
-        ext_up=(pup['__up_stop_dist'].rename('extension_up')
-                if not starts else
-                pup['__up_start_dist'].rename('extension_up'))
-        ext_up[ext_up==-1]=0
+                found_start_selector = selector.copy()  # made to index pup
+                found_start_selector[found_start_selector] = z != -1
+                pup.loc[found_start_selector, "__up_start_dist"] = (
+                    z[z != -1] + ic * chunk_size
+                )
+
+            pup.loc[found_stop_selector, "__seq"] = ""  ## frees memory
+            pverbose(" ---> After iteration:")
+            pverbose(pup[selector], how="reverse,yellow")
+
+            selector = (pup.__up_stop_dist == -1) & ~(pup.__out_of_bounds)
+            ic += 1
+
+        ext_up = (
+            pup["__up_stop_dist"].rename("extension_up")
+            if not starts
+            else pup["__up_start_dist"].rename("extension_up")
+        )
+        ext_up[ext_up == -1] = 0
         del pup
 
     else:  # No extension upstream (i.e. the extension is 0)
-        ext_up=pd.Series(0, index=minp.index)
-
+        ext_up = pd.Series(0, index=minp.index)
 
     ######################  Extend Sequence Downstream #########################
     if "down" in direction or "down" == direction:
         pdo = minp.copy()
-        pdo['__out_of_bounds']=False
-        pdo['__up_stop_dist']=-1   # -1 means not found
-        selector=pd.Series(True, index=pdo.index) # initialized as all True; keeps track of intervals with work to do
-        ic = 0  #iteration counter
+        pdo["__out_of_bounds"] = False
+        pdo["__up_stop_dist"] = -1  # -1 means not found
+        selector = pd.Series(
+            True, index=pdo.index
+        )  # initialized as all True; keeps track of intervals with work to do
+        ic = 0  # iteration counter
 
         while (selector).any():
-            pverbose(f'Downstream | iteration {ic},  left to do: {selector.sum()}', how='reverse')
-            pverbose(pdo[selector], how='blue')
+            pverbose(
+                f"Downstream | iteration {ic},  left to do: {selector.sum()}",
+                how="reverse",
+            )
+            pverbose(pdo[selector], how="blue")
             # selector= ... everything which is not done nor out of bounds
             extend_df(pdo, "3", chunk_size, selector)
             subseq_df(pdo, "3", chunk_size, selector)
-            correct_bounds(pdo, adjust='3')
-            get_seqs(pdo, fs, selector) # seqs length is only selector
+            correct_bounds(pdo, adjust="3")
+            get_seqs(pdo, fs, selector)  # seqs length is only selector
 
             ## looking for a stop if didn't find it already
-            z=pdo.loc[   selector, 
-                      '__seq'].apply(lambda x: find_leftmost_stop(x, stops))
-            found_stop_selector=selector.copy()   # made to index pdo
-            found_stop_selector[found_stop_selector]=(z!=-1)
-            pdo.loc[found_stop_selector, '__up_stop_dist'] = z[z!=-1] + ic*chunk_size
+            z = pdo.loc[selector, "__seq"].apply(lambda x: find_leftmost_stop(x, stops))
+            found_stop_selector = selector.copy()  # made to index pdo
+            found_stop_selector[found_stop_selector] = z != -1
+            pdo.loc[found_stop_selector, "__up_stop_dist"] = (
+                z[z != -1] + ic * chunk_size
+            )
 
             if keep_off_bounds:
                 # focus on intervals that reached out of bounds in this iteration and did not find a stop:
-                #  record their max extension as up_stop_dist 
-                no_stop_off_bounds=found_stop_selector.copy()
-                no_stop_off_bounds[no_stop_off_bounds]=(z==-1)
-                pdo.loc[no_stop_off_bounds, '__up_stop_dist']=(
-                    (pdo.loc[no_stop_off_bounds, 'End']-pdo.loc[no_stop_off_bounds, 'Start']) + ic*chunk_size
-                    )
-
-            pdo.loc[found_stop_selector, '__seq']=''  ## frees memory
-            pverbose(' ---> After iteration:')
-            pverbose(pdo[selector], how='reverse,blue')
+                #  record their max extension as up_stop_dist
+                no_stop_off_bounds = found_stop_selector.copy()
+                no_stop_off_bounds[no_stop_off_bounds] = z == -1
+                pdo.loc[no_stop_off_bounds, "__up_stop_dist"] = (
+                    pdo.loc[no_stop_off_bounds, "End"]
+                    - pdo.loc[no_stop_off_bounds, "Start"]
+                ) + ic * chunk_size
+
+            pdo.loc[found_stop_selector, "__seq"] = ""  ## frees memory
+            pverbose(" ---> After iteration:")
+            pverbose(pdo[selector], how="reverse,blue")
 
-            selector= (pdo.__up_stop_dist==-1) & ~(pdo.__out_of_bounds)
-            ic+=1
+            selector = (pdo.__up_stop_dist == -1) & ~(pdo.__out_of_bounds)
+            ic += 1
 
-        ext_down=(pdo['__up_stop_dist'].rename('extension_down'))
-        ext_down[ext_down==-1]=0
+        ext_down = pdo["__up_stop_dist"].rename("extension_down")
+        ext_down[ext_down == -1] = 0
         del pdo
 
     else:  # No extension downstream (i.e. the extension is 0)
-        ext_down=pd.Series(0, index=minp.index)
-
+        ext_down = pd.Series(0, index=minp.index)
 
     ### Extensions have been determined. Now let's apply them to the original DF
-    p['__order']=np.arange(len(p))
-    zp=p.merge(
-        pd.DataFrame( {'__extension_up':ext_up, '__extension_down': ext_down} ),
+    p["__order"] = np.arange(len(p))
+    zp = p.merge(
+        pd.DataFrame({"__extension_up": ext_up, "__extension_down": ext_down}),
         left_on=cds_id,
-        right_index=True
+        right_index=True,
     )
-    assert len(zp)==nexons
-    p.drop(columns=['__order'], inplace=True)
-    p=zp
+    assert len(zp) == nexons
+    p.drop(columns=["__order"], inplace=True)
+    p = zp
 
     sort_intervals_by_5(p)
     extend_groups(p, cds_id)
-    p.sort_values('__order', inplace=True)     # restore order
+    p.sort_values("__order", inplace=True)  # restore order
 
     # getting ready to return
     if record_extensions:
-        p.rename(columns={'__extension_up': 'extension_up',
-                          '__extension_down': 'extension_down'
-        }, inplace=True)
-        to_drop=['__order']
+        p.rename(
+            columns={
+                "__extension_up": "extension_up",
+                "__extension_down": "extension_down",
+            },
+            inplace=True,
+        )
+        to_drop = ["__order"]
     else:
-        to_drop=['__extension_up', '__extension_down', '__order']
+        to_drop = ["__extension_up", "__extension_down", "__order"]
 
     if group_id is None:
         to_drop.append(cds_id)
     p.drop(columns=to_drop, inplace=True)
 
     return p
 
+
+
+# MM # efficients methods to work inplace. All methods with df as input have one row per CDS group
+def extend_df(df, direction, extension, selector):
+    """Inplace"""
+    if direction == "5":
+        df.loc[selector & (df.Strand == "+"), ["Start"]] -= extension
+        df.loc[selector & (df.Strand == "-"), ["End"]] += extension
+    elif direction == "3":
+        df.loc[selector & (df.Strand == "-"), ["Start"]] -= extension
+        df.loc[selector & (df.Strand == "+"), ["End"]] += extension
+
+
+def extend_groups(dfg, cds_id):
+    """In place, dfg may contain multiple exons"""
+    first_exon_indices = (
+        dfg.groupby(cds_id).apply(lambda x: x.index[0]).reset_index(drop=True)
+    )
+    last_exon_indices = (
+        dfg.groupby(cds_id).apply(lambda x: x.index[-1]).reset_index(drop=True)
+    )
+    sp = dfg.Strand == "+"
+    sm = dfg.Strand == "-"
+
+    dfg.loc[sp[first_exon_indices], "Start"] -= dfg.loc[
+        sp[first_exon_indices], "__extension_up"
+    ]
+    dfg.loc[sp[last_exon_indices], "End"] += dfg.loc[
+        sp[last_exon_indices], "__extension_down"
+    ]
+    dfg.loc[sm[first_exon_indices], "End"] += dfg.loc[
+        sm[first_exon_indices], "__extension_up"
+    ]
+    dfg.loc[sm[last_exon_indices], "Start"] -= dfg.loc[
+        sm[last_exon_indices], "__extension_down"
+    ]
+
+
+def get_seqs(df, fs, selector):
+    """Creates/updates column __seq"""
+    seqs = []
+    d = df[selector]
+    for start, end, strand, chrom in zip(d.Start, d.End, d.Strand, d.Chromosome):
+        _fasta = fs[chrom]
+        if strand == "-":
+            seqs.append((-_fasta[start:end]).seq.upper())  # reverse complement
+        elif strand == "+":
+            seqs.append(_fasta[start:end].seq.upper())
+        else:
+            raise Exception()
+    df.loc[selector, "__seq"] = seqs
+
+
+def correct_bounds(df, adjust=None):
+    """Like pyranges genome_bounds, inplace; but also:
+    adjust the 5' or 3' end of intervals so they are multiples of 3
+    and set boolean attribute __out_of_bounds"""
+    out_end = df["End"] > df["__chromsize"]
+    df.loc[out_end, "End"] = df.loc[out_end, ["End", "__chromsize"]].min(axis=1)
+    out_start = df["Start"] < 0
+    df.loc[out_start, "Start"] = 0
+
+    sp = df.Strand == "+"
+    sm = df.Strand == "-"
+
+    if adjust == "5":
+        df.loc[out_start & sp, "Start"] += (
+            df.loc[out_start & sp, "End"] - df.loc[out_start & sp, "Start"]
+        ).mod(3)
+        df.loc[out_end & sm, "End"] -= (
+            df.loc[out_end & sm, "End"] - df.loc[out_end & sm, "Start"]
+        ).mod(3)
+
+    elif adjust == "3":
+        df.loc[out_end & sp, "End"] -= (
+            df.loc[out_end & sp, "End"] - df.loc[out_end & sp, "Start"]
+        ).mod(3)
+        df.loc[out_start & sm, "Start"] += (
+            df.loc[out_start & sm, "End"] - df.loc[out_start & sm, "Start"]
+        ).mod(3)
+
+    df.loc[(out_end | out_start), "__out_of_bounds"] = True
+
+
+def subseq_df(df, from_end, amount, selector):
+    """Similar to pyranges subseq but inplace"""
+    sp = selector & (df.Strand == "+")
+    sm = selector & (df.Strand == "-")
+    if from_end == "5":
+        df.loc[sp, "End"] = df.loc[sp, "Start"] + amount
+        df.loc[sm, "Start"] = df.loc[sm, "End"] - amount
+    elif from_end == "3":
+        df.loc[sp, "Start"] = df.loc[sp, "End"] - amount
+        df.loc[sm, "End"] = df.loc[sm, "Start"] + amount
+    else:
+        raise Exception()
+
+
+def find_rightmost_stop(seq, motifs):
+    """Returns the distance from the end of the string
+    of the first codon position of the rightmost stop; e.g. 3 is for last codon"""
+    for i in range(len(seq) - 3, -1, -3):
+        if seq[i : i + 3] in motifs:
+            return len(seq) - i
+    return -1
+
+
+def find_leftmost_start(row, motifs, chunk_size):
+    """Returns the distance from the end of the string
+    of the first codon position of the leftmost start AFTER the position in column __up_stop_dist
+    """
+    seq = row["__seq"]
+    stop_pos = row["__up_stop_dist"]
+    start_search = (3 + len(seq) - (stop_pos % chunk_size)) if stop_pos != -1 else 0
+    # we search starting from the position next to the stop
+    for i in range(start_search, len(seq), 3):
+        if seq[i : i + 3] in motifs:
+            return len(seq) - i
+    return -1
+
+
+def find_leftmost_stop(seq, motifs):
+    """Returns the position (distance from the start of the string)
+    of the third codon position of the leftmost stop; e.g. 3 is for the first codon"""
+    for i in range(0, len(seq), 3):
+        if seq[i : i + 3] in motifs:
+            return i + 3
+    return -1
+
+
+def sort_intervals_by_5(df):
+    def select_column(row):
+        return row["Start"] if (row["Strand"] == "+") else -(row["End"])
+
+    new_order = df.apply(select_column, axis=1).sort_values().index
+    df.iloc[:] = df.iloc[new_order]
+
+
```

### Comparing `orf_tools-0.0.1/src/orf_tools.egg-info/PKG-INFO` & `orf_tools-0.0.3/src/orf_tools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
-Name: orf-tools
-Version: 0.0.1
+Name: orf_tools
+Version: 0.0.3
 Summary: Tools to work with open reading frames (ORFs)
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti and Joan Pallares
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: pyfaidx>=0.7.2
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: easyterm>=1.0.0
+Requires-Dist: numpy>=1.17.0
 
 # orf_tools
 
 Package to manipulate open reading frames (ORFs).
 
 Dependent on pandas.
```

