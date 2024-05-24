# Comparing `tmp/sagepy-0.2.8.tar.gz` & `tmp/sagepy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagepy-0.2.8.tar", max compression
+gzip compressed data, was "sagepy-0.2.9.tar", max compression
```

## Comparing `sagepy-0.2.8.tar` & `sagepy-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     7031 2024-05-06 13:07:33.029336 sagepy-0.2.8/README.md
--rw-r--r--   0        0        0      348 2024-05-06 13:07:33.029336 sagepy-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/__init__.py
--rw-r--r--   0        0        0      372 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/__init__.py
--rw-r--r--   0        0        0    18115 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/database.py
--rw-r--r--   0        0        0     6904 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/enzyme.py
--rw-r--r--   0        0        0      894 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/fasta.py
--rw-r--r--   0        0        0     1607 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/fdr.py
--rw-r--r--   0        0        0     3103 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/ion_series.py
--rw-r--r--   0        0        0     8954 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/lfq.py
--rw-r--r--   0        0        0     3438 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/mass.py
--rw-r--r--   0        0        0        0 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/ml/__init__.py
--rw-r--r--   0        0        0     2275 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/modification.py
--rw-r--r--   0        0        0     4251 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/peptide.py
--rw-r--r--   0        0        0    28587 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/scoring.py
--rw-r--r--   0        0        0    14105 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/spectrum.py
--rw-r--r--   0        0        0     4178 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/core/tmt.py
--rw-r--r--   0        0        0        0 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/qfdr/__init__.py
--rw-r--r--   0        0        0     2128 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/qfdr/tdc.py
--rw-r--r--   0        0        0     1676 2024-05-06 13:07:33.029336 sagepy-0.2.8/sagepy/utility.py
--rw-r--r--   0        0        0     7534 1970-01-01 00:00:00.000000 sagepy-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     7031 2024-05-16 13:11:50.154589 sagepy-0.2.9/README.md
+-rw-r--r--   0        0        0      348 2024-05-16 13:11:50.154589 sagepy-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/__init__.py
+-rw-r--r--   0        0        0      372 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/__init__.py
+-rw-r--r--   0        0        0    18115 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/database.py
+-rw-r--r--   0        0        0     6904 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/enzyme.py
+-rw-r--r--   0        0        0      894 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/fasta.py
+-rw-r--r--   0        0        0     1607 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/fdr.py
+-rw-r--r--   0        0        0     3103 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/ion_series.py
+-rw-r--r--   0        0        0     8954 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/lfq.py
+-rw-r--r--   0        0        0     3438 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/mass.py
+-rw-r--r--   0        0        0        0 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/ml/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/modification.py
+-rw-r--r--   0        0        0     4251 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/peptide.py
+-rw-r--r--   0        0        0    35129 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/scoring.py
+-rw-r--r--   0        0        0    14575 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/spectrum.py
+-rw-r--r--   0        0        0     4178 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/core/tmt.py
+-rw-r--r--   0        0        0        0 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/qfdr/__init__.py
+-rw-r--r--   0        0        0     2936 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/qfdr/tdc.py
+-rw-r--r--   0        0        0     5339 2024-05-16 13:11:50.154589 sagepy-0.2.9/sagepy/utility.py
+-rw-r--r--   0        0        0     7534 1970-01-01 00:00:00.000000 sagepy-0.2.9/PKG-INFO
```

### Comparing `sagepy-0.2.8/README.md` & `sagepy-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/database.py` & `sagepy-0.2.9/sagepy/core/database.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/enzyme.py` & `sagepy-0.2.9/sagepy/core/enzyme.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/fasta.py` & `sagepy-0.2.9/sagepy/core/fasta.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/fdr.py` & `sagepy-0.2.9/sagepy/core/fdr.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/ion_series.py` & `sagepy-0.2.9/sagepy/core/ion_series.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/lfq.py` & `sagepy-0.2.9/sagepy/core/lfq.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/mass.py` & `sagepy-0.2.9/sagepy/core/mass.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/modification.py` & `sagepy-0.2.9/sagepy/core/modification.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/peptide.py` & `sagepy-0.2.9/sagepy/core/peptide.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/core/scoring.py` & `sagepy-0.2.9/sagepy/core/scoring.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,65 @@
-from typing import Optional, List, Union, Tuple
+from typing import Optional, List, Union, Tuple, Dict
 
 import pandas as pd
 import sagepy_connector
 from .spectrum import ProcessedSpectrum
 
 psc = sagepy_connector.py_scoring
+psc_utils = sagepy_connector.py_utility
 from .ion_series import IonType
 from .mass import Tolerance
 from .database import PeptideIx, IndexedDatabase
 
 
 class PeptideSpectrumMatch:
     def __init__(self,
                  spec_idx: str,
                  peptide_idx: int,
                  proteins: List[str],
                  decoy: bool,
                  hyper_score: float,
                  rank: int,
                  mono_mass_observed: Union[None, float],
+                 isotope_error: Union[None, int],
+                 average_ppm: Union[None, float],
+                 delta_next: Union[None, float],
+                 delta_best: Union[None, float],
+                 matched_peaks: Union[None, int],
+                 longest_b: Union[None, int],
+                 longest_y: Union[None, int],
+                 longest_y_pct: Union[None, float],
+                 missed_cleavages: Union[None, int],
+                 matched_intensity_pct: Union[None, float],
+                 scored_candidates: Union[None, int],
+                 poisson: Union[None, float],
                  sequence: Union[None, str],
                  charge: Union[None, int],
                  retention_time_observed: Union[None, float],
                  retention_time_predicted: Union[None, float],
                  inverse_mobility_observed: Union[None, float],
                  inverse_mobility_predicted: Union[None, float],
                  intensity_ms1: Union[None, float],
                  intensity_ms2: Union[None, float],
                  q_value: Union[None, float],
                  collision_energy: Union[None, float],
+                 collision_energy_calibrated: Union[None, float],
                  fragments: Union[None, 'Fragments'] = None,
+                 re_score: Union[None, float] = None,
+                 cosine_similarity: Union[None, float] = None,
+                 file_name: Union[None, str] = None,
                  ):
         self.__py_ptr = psc.PyPeptideSpectrumMatch(
-            spec_idx, peptide_idx, proteins, decoy, hyper_score, rank, mono_mass_observed, sequence, charge,
+            spec_idx, peptide_idx, proteins, decoy, hyper_score, rank, mono_mass_observed,
+            isotope_error, average_ppm, delta_next, delta_best, matched_peaks, longest_b, longest_y,
+            longest_y_pct, missed_cleavages, matched_intensity_pct, scored_candidates, poisson,
+            sequence, charge,
             retention_time_observed, retention_time_predicted, inverse_mobility_observed, inverse_mobility_predicted,
-            intensity_ms1, intensity_ms2, q_value, collision_energy, fragments.get_py_ptr()
+            intensity_ms1, intensity_ms2, q_value, collision_energy, collision_energy_calibrated, fragments.get_py_ptr(),
+            re_score, cosine_similarity, file_name,
         )
 
     @property
     def spec_idx(self):
         return self.__py_ptr.spec_idx
 
     @property
@@ -58,34 +79,90 @@
         return self.__py_ptr.hyper_score
 
     @hyper_score.setter
     def hyper_score(self, value):
         self.__py_ptr.hyper_score = value
 
     @property
+    def re_score(self):
+        return self.__py_ptr.re_score
+
+    @re_score.setter
+    def re_score(self, value):
+        self.__py_ptr.re_score = value
+
+    @property
     def rank(self):
         return self.__py_ptr.rank
 
     @property
     def charge(self):
         return self.__py_ptr.charge
 
     @property
+    def mono_mass_observed(self):
+        return self.__py_ptr.mono_mass_observed
+
+    @property
+    def isotope_error(self):
+        return self.__py_ptr.isotope_error
+
+    @property
+    def average_ppm(self):
+        return self.__py_ptr.average_ppm
+
+    @property
+    def delta_next(self):
+        return self.__py_ptr.delta_next
+
+    @property
+    def delta_best(self):
+        return self.__py_ptr.delta_best
+
+    @property
+    def matched_peaks(self):
+        return self.__py_ptr.matched_peaks
+
+    @property
+    def longest_b(self):
+        return self.__py_ptr.longest_b
+
+    @property
+    def longest_y(self):
+        return self.__py_ptr.longest_y
+
+    @property
+    def longest_y_pct(self):
+        return self.__py_ptr.longest_y_pct
+
+    @property
+    def missed_cleavages(self):
+        return self.__py_ptr.missed_cleavages
+
+    @property
+    def matched_intensity_pct(self):
+        return self.__py_ptr.matched_intensity_pct
+
+    @property
+    def scored_candidates(self):
+        return self.__py_ptr.scored_candidates
+
+    @property
+    def poisson(self):
+        return self.__py_ptr.poisson
+
+    @property
     def sequence(self):
         return self.__py_ptr.peptide_sequence
 
     @property
     def mono_mz_calculated(self):
         return self.__py_ptr.mono_mz_calculated
 
     @property
-    def mono_mass_observed(self):
-        return self.__py_ptr.mono_mass_observed
-
-    @property
     def mono_mass_calculated(self):
         return self.__py_ptr.mono_mass_calculated
 
     @property
     def retention_time_observed(self):
         return self.__py_ptr.retention_time_observed
 
@@ -121,50 +198,95 @@
     def q_value(self):
         return self.__py_ptr.q_value
 
     @property
     def collision_energy(self):
         return self.__py_ptr.collision_energy
 
+    @collision_energy.setter
+    def collision_energy(self, value):
+        self.__py_ptr.collision_energy = value
+
+    @property
+    def collision_energy_calibrated(self):
+        return self.__py_ptr.collision_energy_calibrated
+
+    @collision_energy_calibrated.setter
+    def collision_energy_calibrated(self, value):
+        self.__py_ptr.collision_energy_calibrated = value
+
     @property
     def cosine_similarity(self):
         return self.__py_ptr.cosine_similarity
 
     @property
+    def file_name(self):
+        return self.__py_ptr.file_name
+
+    @file_name.setter
+    def file_name(self, value):
+        self.__py_ptr.file_name = value
+
+    @property
     def fragments_observed(self) -> Union[None, 'Fragments']:
         return Fragments.from_py_fragments(self.__py_ptr.fragments_observed)
 
     @property
     def fragments_predicted(self) -> Union[None, 'Fragments']:
+        if self.__py_ptr.fragments_predicted is None:
+            return None
         return Fragments.from_py_fragments(self.__py_ptr.fragments_predicted)
 
     @classmethod
     def from_py_ptr(cls, py_ptr: psc.PyPeptideSpectrumMatch):
         instance = cls.__new__(cls)
         instance.__py_ptr = py_ptr
         return instance
 
+    @staticmethod
+    def from_json(json_str: str) -> 'PeptideSpectrumMatch':
+        psm = psc.psm_from_json(json_str)
+        return PeptideSpectrumMatch.from_py_ptr(psm)
+
     def get_py_ptr(self) -> psc.PyPeptideSpectrumMatch:
         return self.__py_ptr
 
     def associate_fragment_ions_with_prosit_predicted_intensities(self, flat_intensities: List[float]):
         self.__py_ptr.associate_fragment_ions_with_prosit_predicted_intensities(flat_intensities)
 
     def match_observed_predicted_intensities(self) -> Tuple[Optional['Fragments'], Optional[List[float]]]:
         maybe_fragment, flat_intensities = self.__py_ptr.match_observed_predicted_intensities()
         if maybe_fragment is not None:
             return Fragments.from_py_fragments(maybe_fragment), flat_intensities
         return None, None
 
+    def to_json(self) -> str:
+        return self.__py_ptr.to_json()
+
     def __repr__(self):
-        return f"PeptideSpectrumMatch({self.spec_idx}, {self.peptide_idx}, {self.proteins}, {self.decoy}, " \
-               f"{self.hyper_score}, {self.rank} {self.charge}, {self.sequence}, {self.mono_mass_observed}, " \
-               f"{self.mono_mass_calculated}, {self.retention_time_observed}, {self.retention_time_predicted}, " \
-               f"{self.inverse_mobility_observed}, {self.inverse_mobility_predicted}, {self.intensity_ms1}, " \
-               f"{self.intensity_ms2}, {self.q_value}, {self.collision_energy}, {self.cosine_similarity})"
+       return (f"PeptideSpectrumMatch(spec_idx: {self.spec_idx}, match_idx: {self.peptide_idx}, "
+               f"proteins: {self.proteins}, decoy: {self.decoy}, hyper_score: {self.hyper_score}, "
+               f"rank: {self.rank}, mono_mass_observed: {self.mono_mass_observed}, "
+               f"isotope_error: {self.isotope_error}, average_ppm: {self.average_ppm}, "
+               f"delta_next: {self.delta_next}, delta_best: {self.delta_best}, "
+               f"matched_peaks: {self.matched_peaks}, longest_b: {self.longest_b}, "
+               f"longest_y: {self.longest_y}, longest_y_pct: {self.longest_y_pct}, "
+               f"missed_cleavages: {self.missed_cleavages}, matched_intensity_pct: {self.matched_intensity_pct}, "
+               f"scored_candidates: {self.scored_candidates}, poisson: {self.poisson}, "
+               f"sequence: {self.sequence}, charge: {self.charge}, "
+               f"retention_time_observed: {self.retention_time_observed}, "
+               f"retention_time_predicted: {self.retention_time_predicted}, "
+               f"inverse_mobility_observed: {self.inverse_mobility_observed}, "
+               f"inverse_mobility_predicted: {self.inverse_mobility_predicted}, "
+               f"intensity_ms1: {self.intensity_ms1}, intensity_ms2: {self.intensity_ms2}, "
+               f"q_value: {self.q_value}, collision_energy: {self.collision_energy}, "
+               f"collision_energy_calibrated: {self.collision_energy_calibrated}, "
+               f"fragments_observed: {self.fragments_observed if self.fragments_predicted is not None else None}, "
+               f"fragments_predicted: {self.fragments_predicted if self.fragments_observed is not None else None}, "
+               f"re_score: {self.re_score})")
 
 
 class Fragments:
     def __int__(self, charges: List[int], ion_types: List[IonType], fragment_ordinals: List[int],
                 intensities: List[float], mz_calculated: List[float], mz_experimental: List[float]):
         kinds = [x.get_py_ptr() for x in ion_types]
 
@@ -343,20 +465,26 @@
                 result.append(score[0])
             else:
                 result.append(None)
 
         return result
 
     def score_collection_psm(self, db: IndexedDatabase, spectrum_collection: List[Optional[ProcessedSpectrum]],
-                             num_threads: int = 4) -> List[PeptideSpectrumMatch]:
+                             num_threads: int = 4) -> Dict[str, List[PeptideSpectrumMatch]]:
+
         py_psms = self.__scorer_ptr.score_collection_to_psm_collection(db.get_py_ptr(),
                                                                        [spec.get_py_ptr() for spec in
                                                                         spectrum_collection],
                                                                        num_threads)
-        return [PeptideSpectrumMatch.from_py_ptr(psm) for psm in py_psms]
+
+        ret_dict = {}
+        for key, values in py_psms.items():
+            ret_dict[key] = [PeptideSpectrumMatch.from_py_ptr(psm) for psm in values]
+
+        return ret_dict
 
     def score_collection_psm_pandas(self, db: IndexedDatabase, spectrum_collection: List[Optional[ProcessedSpectrum]],
                                     num_threads: int = 4) -> pd.DataFrame:
 
         py_psms = self.__scorer_ptr.score_collection_to_psm_collection(db.get_py_ptr(),
                                                                        [spec.get_py_ptr() for spec in
                                                                         spectrum_collection],
@@ -667,15 +795,15 @@
                 f"ms2 intensity: {self.ms2_intensity}), "
                 f"fragments: {self.fragments})")
 
     def get_py_ptr(self):
         return self.__feature_ptr
 
 
-def associate_fragment_ions_with_prosit_predicted_intensities_par(
+def associate_fragment_ions_with_prosit_predicted_intensities(
         psms: List[PeptideSpectrumMatch],
         flat_intensities: List[List[float]], num_threads: int = 16) -> List['PeptideSpectrumMatch']:
     """Associate fragment ions with prosit predicted intensities in parallel
 
     Args:
         psms (List[PeptideSpectrumMatch]): The peptide spectrum matches
         flat_intensities (List[List[float]]): The flat intensities
@@ -716,20 +844,76 @@
             "proteins": match.proteins,
             "decoy": match.decoy,
             "score": match.hyper_score,
             "rank": match.rank,
             "mono_mz_calculated": match.mono_mz_calculated,
             "mono_mass_observed": match.mono_mass_observed,
             "mono_mass_calculated": match.mono_mass_calculated,
-            "sequence": match.sequence,
+            "sequence": match.peptide_sequence,
             "charge": match.charge,
             "retention_time_observed": match.retention_time_observed,
             "retention_time_predicted": match.retention_time_predicted,
             "inverse_mobility_observed": match.inverse_mobility_observed,
             "inverse_mobility_predicted": match.inverse_mobility_predicted,
             "intensity_ms1": match.intensity_ms1,
             "intensity_ms2": match.intensity_ms2,
             "q_value": match.q_value,
             "collision_energy": match.collision_energy,
             "cosine_similarity": match.cosine_similarity,
         })
     return pd.DataFrame(row_list)
+
+
+def json_bin_to_psms(json_bin: bytes) -> List[PeptideSpectrumMatch]:
+    """ Convert a binary JSON string to a list of PeptideSpectrumMatch objects.
+
+    Args:
+        json_bin: a binary JSON string
+
+    Returns:
+        a list of PeptideSpectrumMatch objects
+    """
+    return [PeptideSpectrumMatch.from_py_ptr(json_str) for json_str in psc_utils.json_bin_to_psms(json_bin)]
+
+
+def psms_to_json(psms, num_threads: int = 4) -> List[str]:
+    """ Convert a list of PeptideSpectrumMatch objects to a JSON string.
+
+    Args:
+        psms: a list of PeptideSpectrumMatch objects
+        num_threads: the number of threads to use
+
+    Returns:
+        a JSON string
+    """
+    return psc_utils.psms_to_json([psm.get_py_ptr() for psm in psms], num_threads)
+
+
+def psms_to_json_bin(psms) -> bytes:
+    """ Convert a list of PeptideSpectrumMatch objects to a binary JSON string.
+
+    Args:
+        psms: a list of PeptideSpectrumMatch objects
+
+    Returns:
+        a binary JSON string
+    """
+    return psc_utils.psms_to_json_bin([psm.get_py_ptr() for psm in psms])
+
+
+def merge_psm_dicts(left_psms: Dict[str, List[PeptideSpectrumMatch]],
+                    right_psms: Dict[str, List[PeptideSpectrumMatch]],
+                    max_hits: int = 5) -> Dict[str, List[PeptideSpectrumMatch]]:
+    """ Merge two dictionaries of peptide spectrum matches.
+
+    Args:
+        left_psms: the left dictionary of peptide spectrum matches
+        right_psms: the right dictionary of peptide spectrum matches
+        max_hits: the maximum number of hits
+
+    Returns:
+        a dictionary of peptide spectrum matches
+    """
+    left_map = {key: [psm.get_py_ptr() for psm in value] for key, value in left_psms.items()}
+    right_map = {key: [psm.get_py_ptr() for psm in value] for key, value in right_psms.items()}
+    result = psc.merge_psm_maps(left_map, right_map, max_hits)
+    return {key: [PeptideSpectrumMatch.from_py_ptr(psm) for psm in value] for key, value in result.items()}
```

### Comparing `sagepy-0.2.8/sagepy/core/spectrum.py` & `sagepy-0.2.9/sagepy/core/spectrum.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,16 +146,16 @@
 
     def __repr__(self):
         return (f"Precursor(mz: {np.round(self.mz, 2)}, "
                 f"intensity: {self.intensity}, "
                 f"charge: {self.charge}, "
                 f"spectrum_ref: {self.spectrum_ref}, "
                 f"isolation_window: {self.isolation_window}), "
-                f"inverse_ion_mobility: {np.round(self.inverse_ion_mobility, 2)}, "
-                f"collision_energy: {np.round(self.collision_energy, 2)})")
+                f"inverse_ion_mobility: {np.round(self.inverse_ion_mobility, 2) if self.inverse_ion_mobility is not None else self.inverse_ion_mobility}, "
+                f"collision_energy: {np.round(self.collision_energy, 2) if self.collision_energy is not None else self.collision_energy})")
 
 
 class Representation:
     def __init__(self, representation: str = 'centroid'):
         """Representation class
 
         Args:
@@ -241,25 +241,30 @@
     def peaks(self):
         return [Peak.from_py_peak(p) for p in self.__processed_spectrum_ptr.peaks]
 
     @property
     def total_ion_current(self):
         return self.__processed_spectrum_ptr.total_ion_current
 
+    @property
+    def collision_energies(self):
+        return self.__processed_spectrum_ptr.collision_energies
+
     def get_py_ptr(self):
         return self.__processed_spectrum_ptr
 
     def __repr__(self):
         return (f"ProcessedSpectrum(level: {self.level}, "
                 f"id: {self.id}, "
                 f"file_id: {self.file_id}, "
                 f"scan_start_time: {np.round(self.scan_start_time, 2)}, "
                 f"ion_injection_time: {np.round(self.ion_injection_time, 2)}, "
                 f"num_precursors: {len(self.precursors)}, "
                 f"num_peaks: {len(self.peaks)}, "
+                f"collision_energies: {self.collision_energies},"
                 f"total_ion_current: {self.total_ion_current})")
 
 
 class RawSpectrum:
     def __init__(self,
                  file_id: int,
                  spec_id: str,
@@ -331,14 +336,17 @@
     @property
     def intensity(self) -> NDArray[float]:
         return self.__raw_spectrum_ptr.intensity
 
     def get_py_ptr(self):
         return self.__raw_spectrum_ptr
 
+    def filter_top_n_peaks(self, n: int) -> 'RawSpectrum':
+        return RawSpectrum.from_py_raw_spectrum(self.__raw_spectrum_ptr.filter_top_n_peaks(n))
+
     def __repr__(self):
         return (f"RawSpectrum(ms_level: {self.ms_level}, "
                 f"id: {self.id}, "
                 f"precursors: {self.precursors}, "
                 f"representation: {self.representation}, "
                 f"scan_start_time: {self.scan_start_time}, "
                 f"ion_injection_time: {self.ion_injection_time}, "
```

### Comparing `sagepy-0.2.8/sagepy/core/tmt.py` & `sagepy-0.2.9/sagepy/core/tmt.py`

 * *Files identical despite different names*

### Comparing `sagepy-0.2.8/sagepy/qfdr/tdc.py` & `sagepy-0.2.9/sagepy/qfdr/tdc.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,34 +21,61 @@
     def get_py_ptr(self) -> psc.PyTDCMethod:
         return self.__py_ptr
 
     def __repr__(self):
         return f"TDCMethod({self.__py_ptr.to_str()})"
 
 
-def target_decoy_competition(method: str, spectra_idx: List[str], match_idx: List[int], decoy: List[bool],
-                             scores: List[float]) -> Tuple[List[str], List[int], List[bool], List[float], List[float]]:
+def target_decoy_competition(
+        spectra_idx: List[str],
+        match_idx: List[str],
+        decoy: List[bool],
+        scores: List[float],
+        method: str = "peptide_psm_peptide") -> Tuple[List[str], List[str], List[bool], List[float], List[float]]:
+    """ Perform target-decoy competition.
+
+    Args:
+        spectra_idx: a list of spectrum indices
+        match_idx: a list of match indices
+        decoy: a list of decoy flags
+        scores: a list of scores
+        method: the method to use, allowed values are: psm, peptide_psm_only, peptide_peptide_only, peptide_psm_peptide
+
+    Returns:
+        a tuple of spectrum indices, match indices, decoy flags, scores, and q-values
+    """
     tdc_method = TDCMethod(method)
     spec_idx, match_idx, decoy, scores, q_values = psc.target_decoy_competition(
         tdc_method.get_py_ptr(), spectra_idx,
         match_idx, decoy, scores)
     return spec_idx, match_idx, decoy, scores, q_values
 
 
-def target_decoy_competition_pandas(method: str, df: pd.DataFrame) -> pd.DataFrame:
+def target_decoy_competition_pandas(
+        df: pd.DataFrame,
+        method: str = "peptide_psm_peptide") -> pd.DataFrame:
+    """ Perform target-decoy competition on a pandas DataFrame.
+
+    Args:
+        df: a pandas DataFrame
+        method: the method to use, allowed values are: psm, peptide_psm_only, peptide_peptide_only, peptide_psm_peptide
+
+    Returns:
+        a pandas DataFrame with q-values
+    """
     assert 'spec_idx' in df.columns, "spec_idx column not found"
     assert 'match_idx' in df.columns, "match_idx column not found"
     assert 'decoy' in df.columns, "decoy column not found"
     assert 'score' in df.columns, "score column not found"
 
     spec_idx, match_idx, target, scores = (df['spec_idx'].tolist(),
                                            df['match_idx'].tolist(), df['decoy'].tolist(), df['score'].tolist())
 
-    spec_idx, match_idx, target, scores, q_values = target_decoy_competition(method, spec_idx,
-                                                                             match_idx, target, scores)
+    spec_idx, match_idx, target, scores, q_values = target_decoy_competition(spec_idx,
+                                                                             match_idx, target, scores, method)
 
     return pd.DataFrame({
         'spec_idx': spec_idx,
         'match_idx': match_idx,
         'decoy': target,
         'score': scores,
         'q_value': q_values
```

### Comparing `sagepy-0.2.8/PKG-INFO` & `sagepy-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sagepy
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: theGreatHerrLebert
 Author-email: davidteschner@googlemail.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.21.2)
 Requires-Dist: pandas (>=1.3.3)
-Requires-Dist: sagepy-connector (>=0.2.8)
+Requires-Dist: sagepy-connector (>=0.2.9)
 Description-Content-Type: text/markdown
 
 # SAGEpy
 A python interface to the core [SAGE](https://github.com/lazear/sage) search engine for mass spectrometry proteomics
 
 <p align="center">
   <img src="sagepy_logo.png" alt="logo" width="250"/>
```

