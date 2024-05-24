# Comparing `tmp/anoprimer-1.0.1.tar.gz` & `tmp/anoprimer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoprimer-1.0.1.tar", max compression
+gzip compressed data, was "anoprimer-1.0.2.tar", max compression
```

## Comparing `anoprimer-1.0.1.tar` & `anoprimer-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    48094 2024-02-14 20:56:55.421526 anoprimer-1.0.1/AnoPrimer/AnoPrimer.py
--rw-r--r--   0        0        0       64 2024-02-14 20:56:55.421526 anoprimer-1.0.1/AnoPrimer/__init__.py
--rw-r--r--   0        0        0     1079 2024-02-14 20:56:55.421526 anoprimer-1.0.1/LICENSE
--rw-r--r--   0        0        0     1786 2024-02-14 20:56:55.421526 anoprimer-1.0.1/README.md
--rw-r--r--   0        0        0      908 2024-02-14 20:56:55.465526 anoprimer-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 anoprimer-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    48239 2024-05-24 19:19:18.379202 anoprimer-1.0.2/AnoPrimer/AnoPrimer.py
+-rw-r--r--   0        0        0       64 2024-05-24 19:19:18.379202 anoprimer-1.0.2/AnoPrimer/__init__.py
+-rw-r--r--   0        0        0     1079 2024-05-24 19:19:18.379202 anoprimer-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1786 2024-05-24 19:19:18.379202 anoprimer-1.0.2/README.md
+-rw-r--r--   0        0        0      908 2024-05-24 19:19:18.427202 anoprimer-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 anoprimer-1.0.2/PKG-INFO
```

### Comparing `anoprimer-1.0.1/AnoPrimer/AnoPrimer.py` & `anoprimer-1.0.2/AnoPrimer/AnoPrimer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,24 @@
 import pandas as pd
 import plotly.graph_objects as go
 import primer3
 import seaborn as sns
 from matplotlib import patches
 from plotly.subplots import make_subplots
 
-ag3 = malariagen_data.Ag3(url="gs://vo_agam_release/", pre=True)
-af1 = malariagen_data.Af1(url="gs://vo_afun_release/", pre=True)
-
 
 def retrieve_data_resource(species):
     assert species in [
         "gambiae_sl",
         "funestus",
     ], f"species {species} not recognised, please use 'gambiae_sl' or 'funestus'"
     if species == "gambiae_sl":
-        data_resource = ag3
+        data_resource = malariagen_data.Ag3(url="gs://vo_agam_release/", pre=True)
     elif species == "funestus":
-        data_resource = af1
+        data_resource = malariagen_data.Af1(url="gs://vo_afun_release/", pre=True)
     return data_resource
 
 
 def prepare_gDNA_sequence(
     target_loc,
     amplicon_size_range,
     genome_seq,
@@ -601,15 +598,17 @@
             # manually define a new patch
         patch = patches.Patch(color=pal[pair], label=f"pair {pair}")
         # handles is a list, so append manual patch
         handles.append(patch)
     # plot the legend
     plt.legend(handles=handles, loc=legend_loc)
     if out_dir:
-        fig.savefig(f"{out_dir}/{assay_name}_primer_locs.png", dpi=300)
+        fig.savefig(
+            f"{out_dir}/{assay_name}_primer_locs.png", dpi=300, bbox_inches="tight"
+        )
 
 
 def gget_blat_genome(primer_df, assay_type, assembly="anoGam3"):
     """
     Aligns primers to the AgamP3 genome with BLAT.
 
     PARAMETERS
@@ -1252,29 +1251,32 @@
         print(f"No hit for {sequence}")
         return
 
     contig, start, end = blat_df.loc[0, ["chromosome", "start", "end"]]
     contig = contig.replace("chr", "")
     region_span = f"{contig}:{start}-{end}"
     print("plotting frequencies in ag3 data")
+
     fig = plot_sequence_frequencies(
+        data_resource=malariagen_data.Ag3(url="gs://vo_agam_release/", pre=True),
         region=region_span,
         sample_sets=sample_sets,
         sample_query=sample_query,
         width=width,
         height=height,
     )
+    return fig
 
 
 def plot_sequence_frequencies(
-    region, sample_sets=None, sample_query=None, width=700, height=400
+    data_resource, region, sample_sets=None, sample_query=None, width=700, height=400
 ):
     """Retrieve frequencies"""
 
-    snps = ag3.snp_calls(
+    snps = data_resource.snp_calls(
         region=region, sample_sets=sample_sets, sample_query=sample_query
     )
     ref_alt_arr = snps["variant_allele"].compute().values.astype(str)
     freq_arr = (
         allel.GenotypeArray(snps["call_genotype"]).count_alleles().to_frequencies()
     )
     pos = snps["variant_position"].compute().values
```

### Comparing `anoprimer-1.0.1/LICENSE` & `anoprimer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anoprimer-1.0.1/README.md` & `anoprimer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `anoprimer-1.0.1/pyproject.toml` & `anoprimer-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AnoPrimer"
-version = "1.0.1"
+version = "1.0.2"
 description = "A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data"
 readme = "README.md"
 documentation = "https://sanjaynagi.github.io/anoprimer/latest/"
 repository = "https://github.com/sanjaynagi/anoprimer"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
```

### Comparing `anoprimer-1.0.1/PKG-INFO` & `anoprimer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnoPrimer
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data
 Home-page: https://github.com/sanjaynagi/anoprimer
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

