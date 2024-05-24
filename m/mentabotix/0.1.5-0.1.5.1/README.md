# Comparing `tmp/mentabotix-0.1.5.tar.gz` & `tmp/mentabotix-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.5.tar", last modified: Wed May 22 07:21:18 2024, max compression
+gzip compressed data, was "mentabotix-0.1.5.1.tar", last modified: Thu May 23 15:57:33 2024, max compression
```

## Comparing `mentabotix-0.1.5.tar` & `mentabotix-0.1.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1066 2024-05-22 07:20:54.962264 mentabotix-0.1.5/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-22 07:20:54.962264 mentabotix-0.1.5/README.md
--rw-r--r--   0        0        0      611 2024-05-22 07:21:18.590028 mentabotix-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1135 2024-05-22 07:20:54.962264 mentabotix-0.1.5/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    73298 2024-05-22 07:20:54.962264 mentabotix-0.1.5/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-22 07:20:54.966264 mentabotix-0.1.5/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-22 07:20:54.966264 mentabotix-0.1.5/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-22 07:20:54.966264 mentabotix-0.1.5/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     9471 2024-05-22 07:20:54.966264 mentabotix-0.1.5/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-22 07:20:54.966264 mentabotix-0.1.5/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0        0 2024-05-22 07:20:54.966264 mentabotix-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-22 07:20:54.966264 mentabotix-0.1.5/tests/find_tests.py
--rw-r--r--   0        0        0    15660 2024-05-22 07:20:54.966264 mentabotix-0.1.5/tests/test_botix.py
--rw-r--r--   0        0        0    10196 2024-05-22 07:20:54.966264 mentabotix-0.1.5/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-22 07:20:54.966264 mentabotix-0.1.5/tests/test_menta.py
--rw-r--r--   0        0        0     9251 2024-05-22 07:20:54.966264 mentabotix-0.1.5/tests/test_moving_state.py
--rw-r--r--   0        0        0     6505 2024-05-22 07:20:54.966264 mentabotix-0.1.5/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24150 1970-01-01 00:00:00.000000 mentabotix-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-23 15:57:09.334616 mentabotix-0.1.5.1/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-23 15:57:09.334616 mentabotix-0.1.5.1/README.md
+-rw-r--r--   0        0        0      613 2024-05-23 15:57:33.814744 mentabotix-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1135 2024-05-23 15:57:09.334616 mentabotix-0.1.5.1/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    73476 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0    15498 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/tests/find_tests.py
+-rw-r--r--   0        0        0    15660 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/tests/test_botix.py
+-rw-r--r--   0        0        0    11417 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/tests/test_menta.py
+-rw-r--r--   0        0        0     9251 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/tests/test_moving_state.py
+-rw-r--r--   0        0        0     6505 2024-05-23 15:57:09.338616 mentabotix-0.1.5.1/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.1/PKG-INFO
```

### Comparing `mentabotix-0.1.5/LICENSE` & `mentabotix-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/README.md` & `mentabotix-0.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/pyproject.toml` & `mentabotix-0.1.5.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.5"
+version = "0.1.5.1"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.5/src/mentabotix/__init__.py` & `mentabotix-0.1.5.1/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/src/mentabotix/modules/botix.py` & `mentabotix-0.1.5.1/src/mentabotix/modules/botix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1503,14 +1503,16 @@
                         to_state_alias: str = name_gen()
                         used_state[to_state] = to_state_alias
                         lines.insert(0, f'state "{to_state}" as {to_state_alias}\n')
                     else:
                         to_state_alias = used_state.get(to_state)
                     lines.append(f"{from_state_alias} --> {to_state_alias}\n")
                 else:
+                    if not callable(transition.breaker):
+                        raise ValueError("The break function must be callable. Since branch must need a valid breaker.")
                     break_node_name: str = break_gen()
                     lines.insert(0, f"state {break_node_name} <<choice>>\n")
                     lines.insert(
                         1, f"note right of {break_node_name}: {get_function_annotations(transition.breaker)}\n"
                     )
                     lines.append(f"{from_state_alias} --> {break_node_name}\n")
                     for case_name, to_state in transition.to_states.items():
```

### Comparing `mentabotix-0.1.5/src/mentabotix/modules/logger.py` & `mentabotix-0.1.5.1/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/src/mentabotix/modules/menta.py` & `mentabotix-0.1.5.1/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/src/mentabotix/tools/generators.py` & `mentabotix-0.1.5.1/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/tests/find_tests.py` & `mentabotix-0.1.5.1/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/tests/test_botix.py` & `mentabotix-0.1.5.1/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/tests/test_composer.py` & `mentabotix-0.1.5.1/tests/test_composer.py`

 * *Files 3% similar despite different names*

```diff
@@ -271,10 +271,42 @@
         self.assertEqual(turn_transition.duration, turn_duration)
 
     def test_invalid_turn_speed(self):
         # 测试无效的 turn_speed 输入
         with self.assertRaises(ValueError):
             random_lr_turn_branch(MovingState(0), MovingState(20), 2.0, -1, 1.5, 1.5)  # Invalid turn_speed
 
+    def test_seq_add(self):
+        # Test adding correct unit types
+        state = MovingState(1)
+        pre_val = 1
+        transition = MovingTransition(pre_val)
+        # Test adding incorrect unit type
+        dur = 5
+        lead_time = 0.05
+        chain_pack = straight_chain(1000, 5000, dur, interval=1.25, lead_time=lead_time)
+
+        print(chain_pack)
+        self.moving_chain_composer.init_container().add(state).add(transition).concat(*chain_pack)
+        pack = self.moving_chain_composer.export_structure()[1]
+        self.assertAlmostEqual(pre_val + dur - lead_time, sum(t.duration for t in pack))
+        Botix.export_structure("seq_add.puml", pack)
+
+        def _a() -> bool:
+            return True
+
+        chain_pack = straight_chain(
+            1000,
+            5000,
+            dur,
+            interval=1.25,
+            lead_time=lead_time,
+            breaker=_a,
+        )
+        self.moving_chain_composer.init_container().add(state).add(transition).concat(*chain_pack)
+        pack = self.moving_chain_composer.export_structure()[1]
+        self.assertAlmostEqual(pre_val + dur - lead_time, sum(t.duration for t in pack))
+        Botix.export_structure("seq_add_breaker.puml", pack)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.5/tests/test_menta.py` & `mentabotix-0.1.5.1/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/tests/test_moving_state.py` & `mentabotix-0.1.5.1/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/tests/test_moving_transition.py` & `mentabotix-0.1.5.1/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5/PKG-INFO` & `mentabotix-0.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: terminaltables>=3.1.10
```

