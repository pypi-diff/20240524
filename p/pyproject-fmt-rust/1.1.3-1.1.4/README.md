# Comparing `tmp/pyproject_fmt_rust-1.1.3.tar.gz` & `tmp/pyproject_fmt_rust-1.1.4.tar.gz`

## Comparing `pyproject_fmt_rust-1.1.3.tar` & `pyproject_fmt_rust-1.1.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.3/Cargo.toml
--rw-r--r--   0     1001      127       36 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.github/FUNDING.yml
--rw-r--r--   0     1001      127      365 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.github/SECURITY.md
--rw-r--r--   0     1001      127      117 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.github/dependabot.yml
--rw-r--r--   0     1001      127       76 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.github/release.yml
--rw-r--r--   0     1001      127     2248 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.github/workflows/check.yml
--rw-r--r--   0     1001      127     3720 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.github/workflows/release.yml
--rw-r--r--   0     1001      127      158 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.gitignore
--rw-r--r--   0     1001      127      973 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      240 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127       16 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/.rustfmt.toml
--rw-r--r--   0     1001      127     3256 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1023 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/LICENSE.txt
--rw-r--r--   0     1001      127      861 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/README.md
--rw-r--r--   0     1001      127     3185 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/build_system.rs
--rw-r--r--   0     1001      127      309 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/data/ruff-21.expected.toml
--rw-r--r--   0     1001      127      295 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/data/ruff-21.start.toml
--rw-r--r--   0     1001      127     3447 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/data/ruff-order.expected.toml
--rw-r--r--   0     1001      127     3281 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/data/ruff-order.start.toml
--rw-r--r--   0     1001      127     3755 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/global.rs
--rw-r--r--   0     1001      127     8859 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/helpers/array.rs
--rw-r--r--   0     1001      127     4406 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/helpers/create.rs
--rw-r--r--   0     1001      127       78 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/helpers/mod.rs
--rw-r--r--   0     1001      127     4595 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/helpers/pep508.rs
--rw-r--r--   0     1001      127     1531 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/helpers/string.rs
--rw-r--r--   0     1001      127    12012 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/helpers/table.rs
--rw-r--r--   0     1001      127     8018 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/main.rs
--rw-r--r--   0     1001      127    29842 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/project.rs
--rw-r--r--   0     1001      127     8547 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust/src/ruff.rs
--rw-r--r--   0     1001      127       29 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/rust-toolchain.toml
--rw-r--r--   0     1001      127      161 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/src/pyproject_fmt_rust/__init__.py
--rw-r--r--   0     1001      127      638 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/src/pyproject_fmt_rust/_lib.pyi
--rw-r--r--   0     1001      127        0 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/src/pyproject_fmt_rust/py.typed
--rw-r--r--   0     1001      127      991 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/tests/test_main.py
--rw-r--r--   0     1001      127     2081 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/tox.ini
--rw-r--r--   0     1001      127    26478 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/Cargo.lock
--rw-r--r--   0     1001      127     3299 2024-05-21 01:37:44.000000 pyproject_fmt_rust-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.4/Cargo.toml
+-rw-r--r--   0     1001      127       36 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      365 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.github/SECURITY.md
+-rw-r--r--   0     1001      127      117 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.github/dependabot.yml
+-rw-r--r--   0     1001      127       76 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.github/release.yml
+-rw-r--r--   0     1001      127     2248 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.github/workflows/check.yml
+-rw-r--r--   0     1001      127     3720 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      158 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.gitignore
+-rw-r--r--   0     1001      127      973 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      240 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127       16 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/.rustfmt.toml
+-rw-r--r--   0     1001      127     3256 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1305 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/CONTRIBUTING.md
+-rw-r--r--   0     1001      127     1023 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/LICENSE.txt
+-rw-r--r--   0     1001      127      861 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/README.md
+-rw-r--r--   0     1001      127     3185 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/build_system.rs
+-rw-r--r--   0     1001      127      309 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/data/ruff-21.expected.toml
+-rw-r--r--   0     1001      127      295 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/data/ruff-21.start.toml
+-rw-r--r--   0     1001      127     3447 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/data/ruff-order.expected.toml
+-rw-r--r--   0     1001      127     3281 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/data/ruff-order.start.toml
+-rw-r--r--   0     1001      127     3755 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/global.rs
+-rw-r--r--   0     1001      127    10085 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/helpers/array.rs
+-rw-r--r--   0     1001      127     4406 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/helpers/create.rs
+-rw-r--r--   0     1001      127       78 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/helpers/mod.rs
+-rw-r--r--   0     1001      127     4595 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/helpers/pep508.rs
+-rw-r--r--   0     1001      127     1531 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/helpers/string.rs
+-rw-r--r--   0     1001      127    12012 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/helpers/table.rs
+-rw-r--r--   0     1001      127     8018 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/main.rs
+-rw-r--r--   0     1001      127    29842 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/project.rs
+-rw-r--r--   0     1001      127     8547 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust/src/ruff.rs
+-rw-r--r--   0     1001      127       29 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/rust-toolchain.toml
+-rw-r--r--   0     1001      127      161 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/src/pyproject_fmt_rust/__init__.py
+-rw-r--r--   0     1001      127      638 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/src/pyproject_fmt_rust/_lib.pyi
+-rw-r--r--   0     1001      127        0 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/src/pyproject_fmt_rust/py.typed
+-rw-r--r--   0     1001      127      991 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/tests/test_main.py
+-rw-r--r--   0     1001      127     2081 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/tox.ini
+-rw-r--r--   0     1001      127    26478 2024-05-24 02:37:48.000000 pyproject_fmt_rust-1.1.4/Cargo.lock
+-rw-r--r--   0     1001      127     3299 2024-05-24 02:37:34.000000 pyproject_fmt_rust-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.4/PKG-INFO
```

### Comparing `pyproject_fmt_rust-1.1.3/Cargo.toml` & `pyproject_fmt_rust-1.1.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyproject-fmt-rust"
-version = "1.1.3"
+version = "1.1.4"
 description = "Format pyproject.toml files"
 repository = "https://github.com/tox-dev/pyproject-fmt"
 readme = "README.md"
 license = "MIT"
 edition = "2021"
 
 [lib]
```

### Comparing `pyproject_fmt_rust-1.1.3/.github/workflows/check.yml` & `pyproject_fmt_rust-1.1.4/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/.github/workflows/release.yml` & `pyproject_fmt_rust-1.1.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/.pre-commit-config.yaml` & `pyproject_fmt_rust-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/CODE_OF_CONDUCT.md` & `pyproject_fmt_rust-1.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/LICENSE.txt` & `pyproject_fmt_rust-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/README.md` & `pyproject_fmt_rust-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/build_system.rs` & `pyproject_fmt_rust-1.1.4/rust/src/build_system.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/data/ruff-order.expected.toml` & `pyproject_fmt_rust-1.1.4/rust/src/data/ruff-order.expected.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/data/ruff-order.start.toml` & `pyproject_fmt_rust-1.1.4/rust/src/data/ruff-order.start.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/global.rs` & `pyproject_fmt_rust-1.1.4/rust/src/global.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/helpers/array.rs` & `pyproject_fmt_rust-1.1.4/rust/src/helpers/array.rs`

 * *Files 12% similar despite different names*

```diff
@@ -19,49 +19,48 @@
                     update_content(array_entry.as_node().unwrap(), transform);
                 }
             }
         }
     }
 }
 
+#[allow(clippy::range_plus_one, clippy::too_many_lines)]
 pub fn sort<F>(node: &SyntaxNode, transform: F)
 where
     F: Fn(&str) -> String,
 {
     for array in node.children_with_tokens() {
         if array.kind() == ARRAY {
             let array_node = array.as_node().unwrap();
+            let has_trailing_comma = array_node
+                .children_with_tokens()
+                .map(|x| x.kind())
+                .filter(|x| *x == COMMA || *x == VALUE)
+                .last()
+                == Some(COMMA);
             let mut value_set = Vec::<Vec<SyntaxElement>>::new();
             let entry_set = RefCell::new(Vec::<SyntaxElement>::new());
             let mut key_to_pos = HashMap::<String, usize>::new();
 
             let mut add_to_value_set = |entry: String| {
                 let mut entry_set_borrow = entry_set.borrow_mut();
                 if !entry_set_borrow.is_empty() {
                     key_to_pos.insert(entry, value_set.len());
                     value_set.push(entry_set_borrow.clone());
                     entry_set_borrow.clear();
                 }
             };
             let mut entries = Vec::<SyntaxElement>::new();
             let mut has_value = false;
-            let mut previous_is_value = false;
             let mut previous_is_bracket_open = false;
             let mut entry_value = String::new();
             let mut count = 0;
 
             for entry in array_node.children_with_tokens() {
                 count += 1;
-                if previous_is_value {
-                    // make sure ends with trailing comma
-                    previous_is_value = false;
-                    if entry.kind() != COMMA {
-                        entry_set.borrow_mut().push(make_comma());
-                    }
-                }
                 if previous_is_bracket_open {
                     // make sure ends with trailing comma
                     if entry.kind() == NEWLINE || entry.kind() == WHITESPACE {
                         continue;
                     }
                     previous_is_bracket_open = false;
                 }
@@ -96,37 +95,48 @@
                             }
                         }
                         if !found_string {
                             // abort if not correct types
                             return;
                         }
                         entry_set.borrow_mut().push(entry);
-                        previous_is_value = true;
+                        entry_set.borrow_mut().push(make_comma());
                     }
                     NEWLINE => {
                         entry_set.borrow_mut().push(entry);
                         if has_value {
                             add_to_value_set(entry_value.clone());
                             has_value = false;
                         }
                     }
+                    COMMA => {}
                     _ => {
                         entry_set.borrow_mut().push(entry);
                     }
                 }
             }
 
             let mut order: Vec<String> = key_to_pos.clone().into_keys().collect();
             order.string_sort_unstable(natural_lexical_cmp);
             let end = entries.split_off(2);
             for key in order {
                 entries.extend(value_set[key_to_pos[&key]].clone());
             }
             entries.extend(end);
             array_node.splice_children(0..count, entries);
+            if !has_trailing_comma {
+                if let Some((i, _)) = array_node
+                    .children_with_tokens()
+                    .enumerate()
+                    .filter(|(_, x)| x.kind() == COMMA)
+                    .last()
+                {
+                    array_node.splice_children(i..i + 1, vec![]);
+                }
+            }
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use indoc::indoc;
@@ -207,38 +217,31 @@
 
     #[rstest]
     #[case::empty(
         indoc ! {r"
     a = []
     "},
         indoc ! {r"
-    a = [
-    ]
+    a = []
     "}
     )]
     #[case::single(
         indoc ! {r#"
     a = ["A"]
     "#},
         indoc ! {r#"
-    a = [
-      "A",
-    ]
+    a = ["A"]
     "#}
     )]
     #[case::newline_single(
         indoc ! {r#"
-    a = [
-      "A"
-    ]
+    a = ["A"]
     "#},
         indoc ! {r#"
-    a = [
-      "A",
-    ]
+    a = ["A"]
     "#}
     )]
     #[case::newline_single_comment(
         indoc ! {r#"
     a = [ # comment
       "A"
     ]
@@ -246,14 +249,22 @@
         indoc ! {r#"
     a = [
       # comment
       "A",
     ]
     "#}
     )]
+    #[case::double(
+        indoc ! {r#"
+    a = ["A", "B"]
+    "#},
+        indoc ! {r#"
+    a = ["A", "B"]
+    "#}
+    )]
     #[case::increasing(
         indoc ! {r#"
     a=["B", "D",
        # C comment
        "C", # C trailing
        # A comment
        "A" # A trailing
@@ -280,14 +291,35 @@
                     if entry.kind() == VALUE {
                         sort(entry.as_node().unwrap(), str::to_lowercase);
                     }
                 }
             }
         }
         let opt = Options {
-            column_width: 1,
+            column_width: 120,
             ..Options::default()
         };
         let res = format_syntax(root_ast, opt);
         assert_eq!(res, expected);
     }
+
+    #[rstest]
+    #[case::reorder_no_trailing_comma(
+        indoc ! {r#"a=["B","A"]"#},
+        indoc ! {r#"a=["A","B"]"#}
+    )]
+    fn test_reorder_no_trailing_comma(#[case] start: &str, #[case] expected: &str) {
+        let root_ast = parse(start).into_syntax().clone_for_update();
+        for children in root_ast.children_with_tokens() {
+            if children.kind() == ENTRY {
+                for entry in children.as_node().unwrap().children_with_tokens() {
+                    if entry.kind() == VALUE {
+                        sort(entry.as_node().unwrap(), str::to_lowercase);
+                    }
+                }
+            }
+        }
+        let mut res = root_ast.to_string();
+        res.retain(|x| !x.is_whitespace());
+        assert_eq!(res, expected);
+    }
 }
```

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/helpers/create.rs` & `pyproject_fmt_rust-1.1.4/rust/src/helpers/create.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/helpers/pep508.rs` & `pyproject_fmt_rust-1.1.4/rust/src/helpers/pep508.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/helpers/string.rs` & `pyproject_fmt_rust-1.1.4/rust/src/helpers/string.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/helpers/table.rs` & `pyproject_fmt_rust-1.1.4/rust/src/helpers/table.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/main.rs` & `pyproject_fmt_rust-1.1.4/rust/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/project.rs` & `pyproject_fmt_rust-1.1.4/rust/src/project.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/rust/src/ruff.rs` & `pyproject_fmt_rust-1.1.4/rust/src/ruff.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/src/pyproject_fmt_rust/_lib.pyi` & `pyproject_fmt_rust-1.1.4/src/pyproject_fmt_rust/_lib.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/tests/test_main.py` & `pyproject_fmt_rust-1.1.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/tox.ini` & `pyproject_fmt_rust-1.1.4/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/Cargo.lock` & `pyproject_fmt_rust-1.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyproject-fmt-rust"
-version = "1.1.3"
+version = "1.1.4"
 dependencies = [
  "indoc",
  "lexical-sort",
  "pep440_rs",
  "pep508_rs",
  "pyo3",
  "regex",
```

### Comparing `pyproject_fmt_rust-1.1.3/pyproject.toml` & `pyproject_fmt_rust-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.3/PKG-INFO` & `pyproject_fmt_rust-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt-rust
-Version: 1.1.3
+Version: 1.1.4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

