# Comparing `tmp/lottokit-1.1.tar.gz` & `tmp/lottokit-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lottokit-1.1.tar", last modified: Sun May  5 07:35:03 2024, max compression
+gzip compressed data, was "lottokit-1.2.tar", last modified: Fri May 24 07:28:08 2024, max compression
```

## Comparing `lottokit-1.1.tar` & `lottokit-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-05 07:35:03.756945 lottokit-1.1/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-1.1/LICENSE
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-05 07:35:03.756829 lottokit-1.1/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-04-15 06:05:32.000000 lottokit-1.1/README.md
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-05 07:35:03.755363 lottokit-1.1/lottokit/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-1.1/lottokit/__init__.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    69087 2024-05-05 07:33:47.000000 lottokit-1.1/lottokit/daletou.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    85918 2024-05-05 05:42:52.000000 lottokit-1.1/lottokit/util.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-05 07:35:03.756439 lottokit-1.1/lottokit.egg-info/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/requires.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/top_level.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-1.1/pyproject.toml
--rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-05-05 07:35:03.756990 lottokit-1.1/setup.cfg
--rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-05-05 07:33:54.000000 lottokit-1.1/setup.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-05 07:35:03.756546 lottokit-1.1/tests/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-1.1/tests/test.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-24 07:28:08.372195 lottokit-1.2/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-1.2/LICENSE
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-24 07:28:08.372089 lottokit-1.2/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-04-15 06:05:32.000000 lottokit-1.2/README.md
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-24 07:28:08.370642 lottokit-1.2/lottokit/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-1.2/lottokit/__init__.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    73989 2024-05-24 07:16:45.000000 lottokit-1.2/lottokit/daletou.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    85918 2024-05-05 05:42:52.000000 lottokit-1.2/lottokit/util.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-24 07:28:08.371667 lottokit-1.2/lottokit.egg-info/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/requires.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-05-24 07:28:08.000000 lottokit-1.2/lottokit.egg-info/top_level.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-1.2/pyproject.toml
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-05-24 07:28:08.372234 lottokit-1.2/setup.cfg
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-05-24 07:26:55.000000 lottokit-1.2/setup.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-24 07:28:08.371792 lottokit-1.2/tests/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-1.2/tests/test.py
```

### Comparing `lottokit-1.1/LICENSE` & `lottokit-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lottokit-1.1/PKG-INFO` & `lottokit-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 1.1
+Version: 1.2
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.9
```

### Comparing `lottokit-1.1/lottokit/daletou.py` & `lottokit-1.2/lottokit/daletou.py`

 * *Files 3% similar despite different names*

```diff
@@ -672,52 +672,138 @@
             next_weekday (int, optional): The next weekday number. If None, it's calculated.
 
         Returns:
             Tuple[Set[int], Set[int]]: A tuple containing two sets of kill numbers for front and back sequences.
         """
         front_sequences = [self.calculate_front(d) for d in data]
         back_sequences = [self.calculate_back(d) for d in data]
+
         next_weekday = next_weekday or self.get_next_weekday()
         next_period = next_period or self.get_next_period()
 
         front_kill_numbers = self.calculate_front_kills(front_sequences, next_period, next_weekday)
         back_kill_numbers = self.calculate_back_kills(back_sequences, next_weekday)
 
         # Ensure numbers are within the valid range
         front_kill_numbers = {num for num in front_kill_numbers if 1 <= num <= self.front_vocab_size}
         back_kill_numbers = {num for num in back_kill_numbers if 1 <= num <= self.back_vocab_size}
 
         return front_kill_numbers, back_kill_numbers
 
+    @staticmethod
+    def get_same_number_index(pre_data, cur_data):
+        same_number_index = []
+        for ind, num in enumerate(pre_data):
+            if num in cur_data:
+                same_number_index.append(ind + 1)
+        return same_number_index
+
+    @staticmethod
+    def get_edge_number_index(pre_data, cur_data):
+        edge_info = []
+        for ind, num in enumerate(pre_data):
+            edge_nums = set(num + i for i in [-1, 1])
+            plead_edge = set(cur_data).intersection(edge_nums)
+            if len(plead_edge) > 0:
+                edge_info.append(ind + 1)
+        return edge_info
+
     def calculate_front_kills(self, sequences: List[List[int]], next_period: int, next_weekday: int) -> Set[int]:
         """Helper function to calculate front kill numbers based on the last sequence."""
+
+        def train_predict(chunk, func_name, chunk_size=1):
+            train_data = [result
+                          for c, n in self.get_chunks_with_next(chunk, chunk_size)
+                          for result in func_name(c[-1], n)]
+            return (
+                {self.exponential_moving_average_next_value(train_data),
+                 self.linear_regression_next_value_by_index(train_data),
+                 self.harmonic_regression_next_value_by_index(train_data)}
+                if len(train_data) > 2 else {}
+            )
+
         last_sequence = sequences[-1]
         a1, a2, a3, a4, a5 = last_sequence
         fb = abs(a5 - a3 - a1)
         fc = a4 - a2
         average = sum(last_sequence) // self.front_size
 
         kills = {fb + t for t in [0, 1, 3, 6] if abs(t) != next_weekday}
         if fb == 0:
             kills.update({a1, a3, a5})
         kills.update({fc, (fc + next_period) % self.front_vocab_size, abs(fc - next_period) % self.front_vocab_size})
         kills.update({average, sum([a1, a2, a3]) // 3})
         kills.update({(a1 + a2) - (a3 + a4) - a5, a1 + a2 + a3 + a4 - a5})
+
+        # odd_even_ratio = [n - 1 if n != 0 else n for n in set(self.calculate_odd_even_ratio(sequences[-1]))]
+        zone_ratio = [n - 1 if n != 0 else n for n in set(self.calculate_zone_ratio(sequences[-1],
+                                                                                    self.front_zone_ranges))]
+        span = self.calculate_span(sequences[-1])
+        edge_index = train_predict(sequences, self.get_edge_number_index)
+        same_index = train_predict(sequences, self.get_edge_number_index)
+        kills.update({
+            abs(sequences[-1][zone_ratio[0]] - sequences[-1][zone_ratio[-1]]),
+            (sequences[-1][zone_ratio[0]] + sequences[-1][zone_ratio[-1]]) % 35,
+            abs(sequences[-1][-zone_ratio[0]] - sequences[-1][-zone_ratio[-1]]),
+            (sequences[-1][-zone_ratio[0]] + sequences[-1][-zone_ratio[-1]]) % 35,
+            abs(sequences[-1][0] - span),
+            (sequences[-1][-1] + span) % 35,
+            span
+        })
+        if edge_index:
+            kills.update(sequences[-1][edge - 1] + i for edge in edge_index if edge - 1 in range(5) for i in [-1, 1])
+
+        if same_index:
+            kills.update(sequences[-1][same - 1] for same in same_index if same - 1 in range(5))
+
         return kills
 
     def calculate_back_kills(self, sequences: List[List[int]], next_weekday: int) -> Set[int]:
         """Helper function to calculate back kill numbers based on the last sequence."""
+
+        def train_predict(chunk, func_name, chunk_size=1):
+            train_data = [result
+                          for c, n in self.get_chunks_with_next(chunk, chunk_size)
+                          for result in func_name(c[-1], n)]
+            return (
+                {self.exponential_moving_average_next_value(train_data),
+                 self.linear_regression_next_value_by_index(train_data),
+                 self.harmonic_regression_next_value_by_index(train_data)}
+                if len(train_data) > 2 else {}
+            )
+
         last_sequence = sequences[-1]
         b1, b2 = last_sequence
         bb = abs(b1 - b2)
         kills = {bb + t for t in [0, 1, 3, 6] if abs(t) != next_weekday}
         kills.update(sequences[-2])
         if bb == 0:
             kills.update({b1, b2})
         kills.update({sum(last_sequence) // self.back_size})
+
+        # odd_even_ratio = [n - 1 if n != 0 else n for n in set(self.calculate_odd_even_ratio(sequences[-1]))]
+        zone_ratio = [n - 1 if n != 0 else n for n in set(self.calculate_zone_ratio(sequences[-1],
+                                                                                    self.back_zone_ranges))]
+        span = self.calculate_span(sequences[-1])
+        edge_index = train_predict(sequences, self.get_edge_number_index)
+        same_index = train_predict(sequences, self.get_edge_number_index)
+        kills.update({
+            abs(sequences[-1][zone_ratio[0]] - sequences[-1][zone_ratio[-1]]),
+            (sequences[-1][zone_ratio[0]] + sequences[-1][zone_ratio[-1]]) % 35,
+            abs(sequences[-1][-zone_ratio[0]] - sequences[-1][-zone_ratio[-1]]),
+            (sequences[-1][-zone_ratio[0]] + sequences[-1][-zone_ratio[-1]]) % 35,
+            abs(sequences[-1][0] - span),
+            (sequences[-1][-1] + span) % 35,
+            span
+        })
+        if edge_index:
+            kills.update(sequences[-1][edge - 1] + i for edge in edge_index if edge - 1 in range(5) for i in [-1, 1])
+
+        if same_index:
+            kills.update(sequences[-1][same - 1] for same in same_index if same - 1 in range(5))
         return kills
 
     def get_banker_numbers(self, data: List[Any], next_period: int = None, next_weekday: int = None) -> Tuple[
         Set[int], Set[int]]:
         """
         Calculate and return sets of 'banker numbers' for both front and back sequences based on provided data.
 
@@ -1287,16 +1373,16 @@
         # use model predict combinations and handle number set
         predict_data = self.model_predict(next_period=next_period, next_weekday=next_weekday,
                                           show_details=False, window_size=window_size)
         predict_front_set, predict_back_set = set(), set()
         for data in predict_data:
             predict_front_set.update(self.calculate_front(data))
             predict_back_set.update(self.calculate_back(data))
-        exclude_front_set = predict_front_set.difference(set(range(1, self.front_vocab_size + 1)))
-        exclude_back_set = predict_back_set.difference(set(range(1, self.back_vocab_size + 1)))
+        exclude_front_set = set(range(1, self.front_vocab_size + 1)).difference(predict_front_set)
+        exclude_back_set = set(range(1, self.back_vocab_size + 1)).difference(predict_back_set)
 
         # generate kill and banker numbers
         history_data = self.get_previous_history_data(next_period=next_period)
         period_data = self.get_previous_period_data(next_period=next_period)
         weekday_data = self.get_previous_weekday_data(next_period=next_period, next_weekday=next_weekday)
         front_kill_numbers, back_kill_numbers = self.get_kill_numbers(history_data, next_period=next_period,
                                                                       next_weekday=next_weekday)
@@ -1310,29 +1396,38 @@
         available_back_numbers = back_kill_numbers & back_banker_numbers
 
         # Convert sets to lists for sampling
         available_front_numbers = list(available_front_numbers)
         available_back_numbers = list(available_back_numbers)
 
         predictions = []
-
+        random.seed(self.calculate_sum_total(self.calculate_front(history_data[-1])))
         # Generate a prediction if there are enough numbers to sample from
         if len(available_front_numbers) >= 5 and len(available_back_numbers) >= 2:
-            predictions.append(
-                sorted(random.sample(available_front_numbers, 5)) + sorted(random.sample(available_back_numbers, 2)))
+            fd = sorted(available_front_numbers) if len(available_front_numbers) == 5 else sorted(
+                random.sample(list(available_front_numbers), 5))
+            bd = sorted(available_back_numbers) if len(available_back_numbers) == 2 else sorted(
+                random.sample(list(available_back_numbers), 2))
+            predictions.append(fd + bd)
 
         # Generate prediction from kill numbers if there are enough
         if len(front_kill_numbers) >= 5 and len(available_back_numbers) >= 2:
-            predictions.append(
-                sorted(random.sample(front_kill_numbers, 5)) + sorted(random.sample(available_back_numbers, 2)))
+            fd = sorted(front_kill_numbers) if len(front_kill_numbers) == 5 else sorted(
+                random.sample(list(front_kill_numbers), 5))
+            bd = sorted(available_back_numbers) if len(available_back_numbers) == 2 else sorted(
+                random.sample(list(available_back_numbers), 2))
+            predictions.append(fd + bd)
 
         # Generate prediction from banker numbers if there are enough
         if len(front_banker_numbers) >= 5 and len(available_back_numbers) >= 2:
-            predictions.append(
-                sorted(random.sample(front_banker_numbers, 5)) + sorted(random.sample(available_back_numbers, 2)))
+            fd = sorted(front_banker_numbers) if len(front_banker_numbers) == 5 else sorted(
+                random.sample(list(front_banker_numbers), 5))
+            bd = sorted(available_back_numbers) if len(available_back_numbers) == 2 else sorted(
+                random.sample(list(available_back_numbers), 2))
+            predictions.append(fd + bd)
 
         # Combine front and back combinations
         if show_details is True:
             self.app_log.info("The following is a preliminary forecast of the data analysis : ")
             self.app_log.info(f"available front numbers: {available_front_numbers}")
             self.app_log.info(f"available back numbers: {available_back_numbers}")
             self.app_log.info(f"front kill numbers: {front_kill_numbers}")
```

### Comparing `lottokit-1.1/lottokit/util.py` & `lottokit-1.2/lottokit/util.py`

 * *Files identical despite different names*

### Comparing `lottokit-1.1/lottokit.egg-info/PKG-INFO` & `lottokit-1.2/lottokit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 1.1
+Version: 1.2
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.9
```

### Comparing `lottokit-1.1/setup.py` & `lottokit-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lottokit',
-    version='1.1',
+    version='1.2',
     keywords=['lottokit', 'lottery'],
     packages=find_packages(),
     package_data={"": ["LICENSE", "NOTICE"]},
     include_package_data=True,
     author="nickdecodes",
     author_email="nickdecodes@163.com",
     description="Lotto Kit Package",
```

