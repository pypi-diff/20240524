# Comparing `tmp/cacoepy-1.0.0.tar.gz` & `tmp/cacoepy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacoepy-1.0.0.tar", last modified: Mon May 20 04:50:28 2024, max compression
+gzip compressed data, was "cacoepy-1.1.0.tar", last modified: Fri May 24 06:04:18 2024, max compression
```

## Comparing `cacoepy-1.0.0.tar` & `cacoepy-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-20 04:50:28.858721 cacoepy-1.0.0/
--rw-r--r--   0 brono      (501) staff       (20)     2979 2024-05-20 04:50:28.858379 cacoepy-1.0.0/PKG-INFO
--rw-r--r--   0 brono      (501) staff       (20)     2524 2024-05-15 17:16:16.000000 cacoepy-1.0.0/README.md
--rw-r--r--   0 brono      (501) staff       (20)       38 2024-05-20 04:50:28.858781 cacoepy-1.0.0/setup.cfg
--rw-r--r--   0 brono      (501) staff       (20)      938 2024-05-12 07:09:03.000000 cacoepy-1.0.0/setup.py
-drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-20 04:50:28.853624 cacoepy-1.0.0/src/
-drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-20 04:50:28.854268 cacoepy-1.0.0/src/cacoepy/
--rw-r--r--   0 brono      (501) staff       (20)        0 2024-05-11 02:37:34.000000 cacoepy-1.0.0/src/cacoepy/__init__.py
--rw-r--r--   0 brono      (501) staff       (20)     3642 2024-05-20 04:46:41.000000 cacoepy-1.0.0/src/cacoepy/aligner.py
-drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-20 04:50:28.856629 cacoepy-1.0.0/src/cacoepy/core/
--rw-r--r--   0 brono      (501) staff       (20)     3141 2024-05-20 04:46:41.000000 cacoepy-1.0.0/src/cacoepy/core/ARPAbet_similarity_matrix.py
--rw-r--r--   0 brono      (501) staff       (20)    10946 2024-05-20 04:46:41.000000 cacoepy-1.0.0/src/cacoepy/core/Needleman_Wunsch.py
--rw-r--r--   0 brono      (501) staff       (20)        0 2024-05-12 04:30:56.000000 cacoepy-1.0.0/src/cacoepy/core/__init__.py
--rw-r--r--   0 brono      (501) staff       (20)     2401 2024-05-20 04:46:41.000000 cacoepy-1.0.0/src/cacoepy/core/aligner_tools.py
--rw-r--r--   0 brono      (501) staff       (20)      764 2024-05-20 04:46:41.000000 cacoepy-1.0.0/src/cacoepy/core/exceptions.py
--rw-r--r--   0 brono      (501) staff       (20)     1515 2024-05-15 08:47:15.000000 cacoepy-1.0.0/src/cacoepy/core/utils.py
-drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-20 04:50:28.858033 cacoepy-1.0.0/src/cacoepy.egg-info/
--rw-r--r--   0 brono      (501) staff       (20)     2979 2024-05-20 04:50:28.000000 cacoepy-1.0.0/src/cacoepy.egg-info/PKG-INFO
--rw-r--r--   0 brono      (501) staff       (20)      530 2024-05-20 04:50:28.000000 cacoepy-1.0.0/src/cacoepy.egg-info/SOURCES.txt
--rw-r--r--   0 brono      (501) staff       (20)        1 2024-05-20 04:50:28.000000 cacoepy-1.0.0/src/cacoepy.egg-info/dependency_links.txt
--rw-r--r--   0 brono      (501) staff       (20)        6 2024-05-20 04:50:28.000000 cacoepy-1.0.0/src/cacoepy.egg-info/requires.txt
--rw-r--r--   0 brono      (501) staff       (20)        8 2024-05-20 04:50:28.000000 cacoepy-1.0.0/src/cacoepy.egg-info/top_level.txt
-drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-20 04:50:28.857696 cacoepy-1.0.0/tests/
--rw-r--r--   0 brono      (501) staff       (20)     1530 2024-05-15 11:32:57.000000 cacoepy-1.0.0/tests/test_align_ARPAbet.py
--rw-r--r--   0 brono      (501) staff       (20)      330 2024-05-20 04:46:41.000000 cacoepy-1.0.0/tests/test_def align_prediction_to_annotation_and_target.py
+drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-24 06:04:18.943843 cacoepy-1.1.0/
+-rw-r--r--   0 brono      (501) staff       (20)     3566 2024-05-24 06:04:18.943605 cacoepy-1.1.0/PKG-INFO
+-rw-r--r--   0 brono      (501) staff       (20)     3068 2024-05-24 05:56:55.000000 cacoepy-1.1.0/README.md
+-rw-r--r--   0 brono      (501) staff       (20)       38 2024-05-24 06:04:18.943901 cacoepy-1.1.0/setup.cfg
+-rw-r--r--   0 brono      (501) staff       (20)      980 2024-05-24 06:03:13.000000 cacoepy-1.1.0/setup.py
+drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-24 06:04:18.938525 cacoepy-1.1.0/src/
+drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-24 06:04:18.939638 cacoepy-1.1.0/src/cacoepy/
+-rw-r--r--   0 brono      (501) staff       (20)        0 2024-05-11 02:37:34.000000 cacoepy-1.1.0/src/cacoepy/__init__.py
+-rw-r--r--   0 brono      (501) staff       (20)     5350 2024-05-24 05:40:41.000000 cacoepy-1.1.0/src/cacoepy/aligner.py
+drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-24 06:04:18.941852 cacoepy-1.1.0/src/cacoepy/core/
+-rw-r--r--   0 brono      (501) staff       (20)     3629 2024-05-24 05:40:41.000000 cacoepy-1.1.0/src/cacoepy/core/ARPAbet_similarity_matrix.py
+-rw-r--r--   0 brono      (501) staff       (20)    12613 2024-05-24 05:40:41.000000 cacoepy-1.1.0/src/cacoepy/core/Needleman_Wunsch.py
+-rw-r--r--   0 brono      (501) staff       (20)        0 2024-05-12 04:30:56.000000 cacoepy-1.1.0/src/cacoepy/core/__init__.py
+-rw-r--r--   0 brono      (501) staff       (20)     2583 2024-05-24 05:40:41.000000 cacoepy-1.1.0/src/cacoepy/core/aligner_tools.py
+-rw-r--r--   0 brono      (501) staff       (20)      952 2024-05-24 05:40:41.000000 cacoepy-1.1.0/src/cacoepy/core/exceptions.py
+-rw-r--r--   0 brono      (501) staff       (20)     1515 2024-05-15 08:47:15.000000 cacoepy-1.1.0/src/cacoepy/core/utils.py
+-rw-r--r--   0 brono      (501) staff       (20)     3837 2024-05-24 05:40:41.000000 cacoepy-1.1.0/src/cacoepy/metric.py
+drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-24 06:04:18.943333 cacoepy-1.1.0/src/cacoepy.egg-info/
+-rw-r--r--   0 brono      (501) staff       (20)     3566 2024-05-24 06:04:18.000000 cacoepy-1.1.0/src/cacoepy.egg-info/PKG-INFO
+-rw-r--r--   0 brono      (501) staff       (20)      586 2024-05-24 06:04:18.000000 cacoepy-1.1.0/src/cacoepy.egg-info/SOURCES.txt
+-rw-r--r--   0 brono      (501) staff       (20)        1 2024-05-24 06:04:18.000000 cacoepy-1.1.0/src/cacoepy.egg-info/dependency_links.txt
+-rw-r--r--   0 brono      (501) staff       (20)        6 2024-05-24 06:04:18.000000 cacoepy-1.1.0/src/cacoepy.egg-info/requires.txt
+-rw-r--r--   0 brono      (501) staff       (20)        8 2024-05-24 06:04:18.000000 cacoepy-1.1.0/src/cacoepy.egg-info/top_level.txt
+drwxr-xr-x   0 brono      (501) staff       (20)        0 2024-05-24 06:04:18.943078 cacoepy-1.1.0/tests/
+-rw-r--r--   0 brono      (501) staff       (20)     1530 2024-05-15 11:32:57.000000 cacoepy-1.1.0/tests/test_align_ARPAbet.py
+-rw-r--r--   0 brono      (501) staff       (20)      330 2024-05-24 05:40:41.000000 cacoepy-1.1.0/tests/test_def_align_prediction_to_annotation_and_target.py
+-rw-r--r--   0 brono      (501) staff       (20)     1387 2024-05-24 05:40:41.000000 cacoepy-1.1.0/tests/test_mdd_phoneme_metrics.py
```

### Comparing `cacoepy-1.0.0/PKG-INFO` & `cacoepy-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cacoepy
-Version: 1.0.0
-Summary: A Python module for aligning mispronounced phonemes.
+Version: 1.1.0
+Summary: A small collection of tools related to mispronunciation detection and diagnosis (MDD) systems.
 Home-page: https://github.com/Brono25/cacoepy.git
 Author: Bronston Ashford
 Author-email: bronston.a@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -14,51 +14,84 @@
 
 # cacoepy
 cacoepy is a small collection of tools related to mispronunciation detection and diagnosis (MDD) systems.
 
 ___
 
 ## Installation
-Download this repository and then run:
-`pip install .`
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install cacopey.
 
+```bash
+pip install cacoepy
+```
 
-## Phoneme Alignment
-The `AlignARPAbet2` class is used to align two sequences of ARPAbet phonemes, taking into account phoneme similarities. Typically sequence aligners focus on identifying matches and mismatches. However, for a more realistic alignment of phonemes in mispronounced speech versus the intended phonemes, it is important to consider the similarity between phoneme pairs.
 
-### Usage
+## Usage
+### AlignARPAbet2
+The `AlignARPAbet2` class is used to align two sequences of ARPAbet phonemes, taking into account phoneme similarities. Typically sequence aligners focus on identifying matches and mismatches. However, for a more realistic alignment of phonemes in mispronounced speech versus the intended phonemes, it is important to consider the similarity between phoneme pairs.
+<br>
 When creating the instance, specify a gap penalty. A more negative value discourages the insertion of gaps.
 ```python
 from cacoepy.aligner import AlignARPAbet2
+from cacoepy.core.utils import pretty_sequences
 
 aligner = AlignARPAbet2(gap_penalty=-4)
 target_phonemes = "th er m aa m ah t er".split(" ")
 mispronounced_phonemes = "uw ao m eh d er".split(" ")
 
 aligned_mispronounced, aligned_target, score = aligner(mispronounced_phonemes, target_phonemes)
-
+pretty_sequences(aligned_target, aligned_mispronounced)
 ```
 
-**Resulting Alignment**:
-```
+**Output**:
+```bash
 th  er  m  aa  m  ah  t  er
 -   uw  -  ao  m  eh  d  er
 ```
 In this example, many of the phonemes are substituted or deleted in this child’s transcription of “thermometer.” Despite this, the `AlignARPAbet2` has found a good alignment by factoring in the similarities between pairs such as *er* and *uw*. For comparison, the Python package `Levenshtein editops` alignment of the same sequences was:
 
 ```
 th  er  m  aa  m  ah  t  er
 uw  ao  m  eh  d  -   -  er
 ```
-Where it only aligns based on exact matches.
+Where it only aligns based on exact matches. Further implementation details can be found [here](docs/similarity_matrix.md).
+
+### align_prediction_to_annotation_and_target
+Given three sets of phoneme sequences:
+- `target`: The phonemes the speaker is attempting to say.
+- `annotation`: The annotation of how the speaker pronounced the target.
+- `prediction`: The output of an MDD system predicting what the speaker said.
+<br>
+This function aligns the prediction sequence to the annotation sequence while preserving the existing alignment between annotation and target.
+
+```python
+from cacoepy.aligner import align_prediction_to_annotation_and_target
+from cacoepy.core.utils import pretty_sequences
+
+target = "th er m aa m ah t er".split(" ")
+annotation = "- uw - ao m eh d er".split(" ")
+prediction = "uw aa ao m eh d uh er".split(" ")
+
+aligned_pred, aligned_ann, aligned_tar = align_prediction_to_annotation_and_target(
+    target_aligned_with_annotation=target,
+    annotation_aligned_with_target=annotation,
+    prediction=prediction,
+)
+pretty_sequences(aligned_tar, aligned_ann, aligned_pred)
+```
+**Output**
+```bash
+th  er  m   aa  m  ah  t  -   er
+-   uw  -   ao  m  eh  d  -   er
+-   uw  aa  ao  m  eh  d  uh  er
+```
 
+## Future Features
+- `AlignARPAbet3` - Aligns 3 sets of phonemes.
+- `mdd_phoneme_metrics` - Evaluation metrics for MDD systems.
 
-### Implementation
-The `AlignARPAbet2` uses the **Needleman-Wunsch** algorithm with a custom similarity matrix for assigning scores to phoneme pairs. To generate the similarity matrix, the phonemes are broken down into their 35 attributes, which describe how they are articulated. Each phoneme may have several attributes each (see `data/ARPAbet_mapping.json` for the breakdown). By signifying which attributes are present or not, each phoneme is represented as a vector in a 35-dimensional attribute space. Then, the cosine similarity is calculated between each pair of phoneme vectors and placed into a lookup table to be used to inform the **Needleman-Wunsch** algorithm during alignment.
-A visual representation of the similarity matrix is shown below. The clear separation of consonants and vowels is apparent in the sub-squares.
 
 
 
-<div align="center">
-    <img src="assets/ARPAbet_similarity_matrix_darkmode.png" alt="SimilarityMatrix" width="700" height="600">
-</div>
+## License
 
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `cacoepy-1.0.0/setup.py` & `cacoepy-1.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 README = (ROOT / "README.md").read_text()
 
 with open(ROOT / "requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="cacoepy",
-    version="1.0.0",
-    description="A Python module for aligning mispronounced phonemes.",
+    version="1.1.0",
+    description="A small collection of tools related to mispronunciation detection and diagnosis (MDD) systems.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Bronston Ashford",
     author_email="bronston.a@gmail.com",
     url="https://github.com/Brono25/cacoepy.git",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `cacoepy-1.0.0/src/cacoepy/core/ARPAbet_similarity_matrix.py` & `cacoepy-1.1.0/src/cacoepy/core/ARPAbet_similarity_matrix.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import numpy as np
 import json
 
 
 def arpabet_similarity_matrix():
+    """
+    Generates a similarity matrix for ARPAbet phonemes based on their attributes.
 
+    This function constructs a phoneme similarity matrix by loading phoneme data from a JSON file,
+    creating binary vectors for each phoneme based on their attributes, and then calculating similarity
+    scores between each pair of phonemes using the cosine similarity method.
+
+    Returns:
+        dict: A dictionary where keys are phoneme pairs and values are their similarity scores.
+    """
     def build_scoring_matrix():
         def load_phoneme_data(file):
             with open(file, "r") as file:
                 data = json.load(file)
             return data
 
         def create_phoneme_vectors(attributes, phoneme_attribute_map):
```

### Comparing `cacoepy-1.0.0/src/cacoepy/core/Needleman_Wunsch.py` & `cacoepy-1.1.0/src/cacoepy/core/Needleman_Wunsch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,35 @@
+from typing import Callable, Dict, Union, List, Tuple
 import inspect
-
 from cacoepy.core.utils import pretty_matrices
 from cacoepy.core.exceptions import InvalidSimilarityError, TracebackIndexError
 
 
 class NeedlemanWunschConfig:
-    def __init__(self, similarity, gap_penalty):
+    def __init__(
+            self, 
+            similarity: Union[Callable[[str, str], float], Dict[str, Dict[str, float]]], 
+            gap_penalty:float
+        ) -> None:
+        """
+        Configuration class for the Needleman-Wunsch algorithm.
+
+        This class handles the configuration for the Needleman-Wunsch algorithm,
+        including the similarity scoring and gap penalty.
+
+        Args:
+            similarity (Union[Callable[[str, str], float], Dict[str, Dict[str, float]]]): 
+                A function or a 2D dictionary to compute similarity scores between characters.
+            gap_penalty (float): The penalty score for introducing gaps in the alignment.
+
+        Raises:
+            InvalidSimilarityError: If the similarity parameter is neither a callable nor a 2D 
+            dictionary. InvalidSimilarityError: If the similarity function does not have 
+            exactly two arguments.
+        """
         self.gap_penalty = gap_penalty
         if callable(similarity):
             self._validate_callable(similarity)
             self.scoring_function = similarity
             self.scoring_matrix = None
         elif isinstance(similarity, dict):
             self.scoring_function = None
@@ -32,31 +52,54 @@
         elif self.scoring_matrix:
             return self.scoring_matrix.get(char_a, {}).get(char_b, 0)
         else:
             raise InvalidSimilarityError("No valid scoring method available.")
 
 
 class NeedlemanWunsch2D:
+    """
+    Performs sequence alignment using the Needleman-Wunsch algorithm with a given configuration.
+
+    Args:
+        config (NeedlemanWunschConfig): Configuration object containing the scoring function 
+        or matrix and gap penalty.
+    """
     def __init__(self, config: NeedlemanWunschConfig):
         self.LEFT = "←"
         self.UP = "↑"
         self.DIAG = "↖"
         self.DONE = "X"
         self.GAP = "-"
         self.config = config
         self._path_idx = []
 
-    def __call__(self, seq1, seq2):
+    def __call__(
+            self, 
+            seq1: List[str], 
+            seq2: List[str]
+        ) -> Tuple[List[str], List[str], float]:
+        """
+        Aligns two sequences using the Needleman-Wunsch algorithm.
+
+        Args:
+            seq1 (str): The first sequence to align.
+            seq2 (str): The second sequence to align.
+
+        Returns:
+            Tuple[List[str], List[str], float]: A tuple containing the aligned 
+            first sequence, aligned second sequence, and the alignment score.
+        """
         self.left_seq = [""] + seq1
         self.top_seq = [""] + seq2
         self.N_col = len(self.top_seq)
         self.N_row = len(self.left_seq)
         self.score_matrix, self.trace_matrix = self._init_score_and_trace_matrix() 
         self._fill_score_matrix()
-        return self._traceback()
+        aligned_left_seq, aligned_top_seq, score = self._traceback()
+        return aligned_left_seq, aligned_top_seq, score
 
     def _init_score_and_trace_matrix(self):
         score_matrix = [[0] * self.N_col for _ in range(self.N_row)]
         trace_matrix = [[0] * self.N_col for _ in range(self.N_row)]
         gap = 0
         for i in range(self.N_row):
             score_matrix[i][0] = gap
@@ -86,15 +129,14 @@
             self.UP: self.score_matrix[i - 1][j] + self.config.gap_penalty,
             self.LEFT: self.score_matrix[i][j - 1] + self.config.gap_penalty,
         }
         max_score, direction = self._choose_path(score)
         return max_score, direction
 
     def _choose_path(self, score):
-        """Choose among paths with equal scores by following a predefined priority: diagonal, left, then up."""
         max_value = max(score.values())
         max_keys = [key for key, value in score.items() if value == max_value]
         if self.UP in max_keys:
             return max_value, self.UP
         elif self.LEFT in max_keys:
             return max_value, self.LEFT
         return max_value, self.DIAG
```

### Comparing `cacoepy-1.0.0/src/cacoepy/core/aligner_tools.py` & `cacoepy-1.1.0/src/cacoepy/core/aligner_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from cacoepy.core.exceptions import AlignSequencePairError
+from typing import List, Tuple
 
-def align_sequence_pairs(ref_a, partner_a, ref_b, partner_b, gap_char="-"):
+def align_sequence_pairs(
+        ref_a: List[str], 
+        partner_a: List[str], 
+        ref_b: List[str], 
+        partner_b: List[str], 
+        gap_char: str ="-"
+        ) -> Tuple[List[str], List[str], List[str]]:
     """
-    Align two pairs of sequences where ref_a and ref_b are the same sequence with different padding.
+    Align two pairs of sequences where ref_a and ref_b are the same sequence 
+    with different padding.
 
     Parameters:
         ref_a (list): The reference sequence aligned with partner_a.
         partner_a (list): The sequence aligned to ref_a.
         ref_b (list): The reference sequence aligned with partner_b.
         partner_b (list): The sequence aligned to ref_b.
         gap_char (str): Character used to represent gaps in the alignments, default is '-'.
```

### Comparing `cacoepy-1.0.0/src/cacoepy/core/exceptions.py` & `cacoepy-1.1.0/src/cacoepy/core/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 class ElementNotInVocabError(Exception):
-    """Exception raised when a sequence element is not found in the vocabulary of the Similarity matrix."""
+    """
+    Exception raised when a sequence element is not found in the 
+    vocabulary of the Similarity matrix.
+    """
     def __init__(self, message):
         super().__init__(message)
 
 
 class InvalidSimilarityError(Exception):
     """Exception raised for invalid similarity inputs in NeedlemanWunschConfig."""
     def __init__(self, message):
@@ -16,7 +19,13 @@
         super().__init__(message)
 
 
 class AlignSequencePairError(Exception):
     """Exception raised for errors associated with align_sequence_pairs"""
     def __init__(self, message):
         super().__init__(message)
+
+
+class PhonemeSequenceError(Exception):
+    """Base exception for errors related to phoneme sequences."""
+    def __init__(self, message):
+        super().__init__(message)
```

### Comparing `cacoepy-1.0.0/src/cacoepy/core/utils.py` & `cacoepy-1.1.0/src/cacoepy/core/utils.py`

 * *Files identical despite different names*

### Comparing `cacoepy-1.0.0/src/cacoepy.egg-info/PKG-INFO` & `cacoepy-1.1.0/src/cacoepy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cacoepy
-Version: 1.0.0
-Summary: A Python module for aligning mispronounced phonemes.
+Version: 1.1.0
+Summary: A small collection of tools related to mispronunciation detection and diagnosis (MDD) systems.
 Home-page: https://github.com/Brono25/cacoepy.git
 Author: Bronston Ashford
 Author-email: bronston.a@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -14,51 +14,84 @@
 
 # cacoepy
 cacoepy is a small collection of tools related to mispronunciation detection and diagnosis (MDD) systems.
 
 ___
 
 ## Installation
-Download this repository and then run:
-`pip install .`
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install cacopey.
 
+```bash
+pip install cacoepy
+```
 
-## Phoneme Alignment
-The `AlignARPAbet2` class is used to align two sequences of ARPAbet phonemes, taking into account phoneme similarities. Typically sequence aligners focus on identifying matches and mismatches. However, for a more realistic alignment of phonemes in mispronounced speech versus the intended phonemes, it is important to consider the similarity between phoneme pairs.
 
-### Usage
+## Usage
+### AlignARPAbet2
+The `AlignARPAbet2` class is used to align two sequences of ARPAbet phonemes, taking into account phoneme similarities. Typically sequence aligners focus on identifying matches and mismatches. However, for a more realistic alignment of phonemes in mispronounced speech versus the intended phonemes, it is important to consider the similarity between phoneme pairs.
+<br>
 When creating the instance, specify a gap penalty. A more negative value discourages the insertion of gaps.
 ```python
 from cacoepy.aligner import AlignARPAbet2
+from cacoepy.core.utils import pretty_sequences
 
 aligner = AlignARPAbet2(gap_penalty=-4)
 target_phonemes = "th er m aa m ah t er".split(" ")
 mispronounced_phonemes = "uw ao m eh d er".split(" ")
 
 aligned_mispronounced, aligned_target, score = aligner(mispronounced_phonemes, target_phonemes)
-
+pretty_sequences(aligned_target, aligned_mispronounced)
 ```
 
-**Resulting Alignment**:
-```
+**Output**:
+```bash
 th  er  m  aa  m  ah  t  er
 -   uw  -  ao  m  eh  d  er
 ```
 In this example, many of the phonemes are substituted or deleted in this child’s transcription of “thermometer.” Despite this, the `AlignARPAbet2` has found a good alignment by factoring in the similarities between pairs such as *er* and *uw*. For comparison, the Python package `Levenshtein editops` alignment of the same sequences was:
 
 ```
 th  er  m  aa  m  ah  t  er
 uw  ao  m  eh  d  -   -  er
 ```
-Where it only aligns based on exact matches.
+Where it only aligns based on exact matches. Further implementation details can be found [here](docs/similarity_matrix.md).
+
+### align_prediction_to_annotation_and_target
+Given three sets of phoneme sequences:
+- `target`: The phonemes the speaker is attempting to say.
+- `annotation`: The annotation of how the speaker pronounced the target.
+- `prediction`: The output of an MDD system predicting what the speaker said.
+<br>
+This function aligns the prediction sequence to the annotation sequence while preserving the existing alignment between annotation and target.
+
+```python
+from cacoepy.aligner import align_prediction_to_annotation_and_target
+from cacoepy.core.utils import pretty_sequences
+
+target = "th er m aa m ah t er".split(" ")
+annotation = "- uw - ao m eh d er".split(" ")
+prediction = "uw aa ao m eh d uh er".split(" ")
+
+aligned_pred, aligned_ann, aligned_tar = align_prediction_to_annotation_and_target(
+    target_aligned_with_annotation=target,
+    annotation_aligned_with_target=annotation,
+    prediction=prediction,
+)
+pretty_sequences(aligned_tar, aligned_ann, aligned_pred)
+```
+**Output**
+```bash
+th  er  m   aa  m  ah  t  -   er
+-   uw  -   ao  m  eh  d  -   er
+-   uw  aa  ao  m  eh  d  uh  er
+```
 
+## Future Features
+- `AlignARPAbet3` - Aligns 3 sets of phonemes.
+- `mdd_phoneme_metrics` - Evaluation metrics for MDD systems.
 
-### Implementation
-The `AlignARPAbet2` uses the **Needleman-Wunsch** algorithm with a custom similarity matrix for assigning scores to phoneme pairs. To generate the similarity matrix, the phonemes are broken down into their 35 attributes, which describe how they are articulated. Each phoneme may have several attributes each (see `data/ARPAbet_mapping.json` for the breakdown). By signifying which attributes are present or not, each phoneme is represented as a vector in a 35-dimensional attribute space. Then, the cosine similarity is calculated between each pair of phoneme vectors and placed into a lookup table to be used to inform the **Needleman-Wunsch** algorithm during alignment.
-A visual representation of the similarity matrix is shown below. The clear separation of consonants and vowels is apparent in the sub-squares.
 
 
 
-<div align="center">
-    <img src="assets/ARPAbet_similarity_matrix_darkmode.png" alt="SimilarityMatrix" width="700" height="600">
-</div>
+## License
 
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `cacoepy-1.0.0/src/cacoepy.egg-info/SOURCES.txt` & `cacoepy-1.1.0/src/cacoepy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 README.md
 setup.py
 src/cacoepy/__init__.py
 src/cacoepy/aligner.py
+src/cacoepy/metric.py
 src/cacoepy.egg-info/PKG-INFO
 src/cacoepy.egg-info/SOURCES.txt
 src/cacoepy.egg-info/dependency_links.txt
 src/cacoepy.egg-info/requires.txt
 src/cacoepy.egg-info/top_level.txt
 src/cacoepy/core/ARPAbet_similarity_matrix.py
 src/cacoepy/core/Needleman_Wunsch.py
 src/cacoepy/core/__init__.py
 src/cacoepy/core/aligner_tools.py
 src/cacoepy/core/exceptions.py
 src/cacoepy/core/utils.py
 tests/test_align_ARPAbet.py
-tests/test_def align_prediction_to_annotation_and_target.py
+tests/test_def_align_prediction_to_annotation_and_target.py
+tests/test_mdd_phoneme_metrics.py
```

### Comparing `cacoepy-1.0.0/tests/test_align_ARPAbet.py` & `cacoepy-1.1.0/tests/test_align_ARPAbet.py`

 * *Files identical despite different names*

