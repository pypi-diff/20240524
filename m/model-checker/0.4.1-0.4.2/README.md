# Comparing `tmp/model_checker-0.4.1.tar.gz` & `tmp/model_checker-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.4.1.tar", last modified: Thu May 23 21:05:54 2024, max compression
+gzip compressed data, was "model_checker-0.4.2.tar", last modified: Thu May 23 21:29:24 2024, max compression
```

## Comparing `model_checker-0.4.1.tar` & `model_checker-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.821076 model_checker-0.4.1/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.1/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     9074 2024-05-23 21:05:54.821076 model_checker-0.4.1/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     8289 2024-05-23 21:03:42.000000 model_checker-0.4.1/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-23 21:05:51.000000 model_checker-0.4.1/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-23 21:05:54.821076 model_checker-0.4.1/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.820076 model_checker-0.4.1/src/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.820076 model_checker-0.4.1/src/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)      124 2024-05-23 21:05:51.000000 model_checker-0.4.1/src/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    13625 2024-05-23 17:20:26.000000 model_checker-0.4.1/src/model_checker/__main__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    21385 2024-05-23 19:00:33.000000 model_checker-0.4.1/src/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    26177 2024-05-23 17:40:02.000000 model_checker-0.4.1/src/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    27951 2024-05-23 18:56:17.000000 model_checker-0.4.1/src/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7836 2024-05-23 18:38:27.000000 model_checker-0.4.1/src/model_checker/syntax.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.821076 model_checker-0.4.1/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     9074 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      510 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.821076 model_checker-0.4.1/test/
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-23 04:07:12.000000 model_checker-0.4.1/test/test.py
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-23 04:07:12.000000 model_checker-0.4.1/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:29:24.275419 model_checker-0.4.2/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.2/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     9583 2024-05-23 21:29:24.275419 model_checker-0.4.2/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     8798 2024-05-23 21:28:21.000000 model_checker-0.4.2/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-23 21:29:19.000000 model_checker-0.4.2/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-23 21:29:24.275419 model_checker-0.4.2/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:29:24.274419 model_checker-0.4.2/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:29:24.274419 model_checker-0.4.2/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)      124 2024-05-23 21:29:19.000000 model_checker-0.4.2/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    13625 2024-05-23 17:20:26.000000 model_checker-0.4.2/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    21385 2024-05-23 19:00:33.000000 model_checker-0.4.2/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    26177 2024-05-23 17:40:02.000000 model_checker-0.4.2/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    27951 2024-05-23 18:56:17.000000 model_checker-0.4.2/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7836 2024-05-23 18:38:27.000000 model_checker-0.4.2/src/model_checker/syntax.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:29:24.275419 model_checker-0.4.2/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     9583 2024-05-23 21:29:24.000000 model_checker-0.4.2/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      510 2024-05-23 21:29:24.000000 model_checker-0.4.2/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-23 21:29:24.000000 model_checker-0.4.2/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-23 21:29:24.000000 model_checker-0.4.2/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-23 21:29:24.000000 model_checker-0.4.2/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-23 21:29:24.000000 model_checker-0.4.2/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:29:24.275419 model_checker-0.4.2/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-23 04:07:12.000000 model_checker-0.4.2/test/test.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-23 04:07:12.000000 model_checker-0.4.2/test/test_examples.py
```

### Comparing `model_checker-0.4.1/LICENCE` & `model_checker-0.4.2/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.1/PKG-INFO` & `model_checker-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.4.1
+Version: 0.4.2
 Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
@@ -86,14 +86,18 @@
 A _negated sentence_ is verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 A _conjunctive sentence_ is verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 A _disjunctive sentence_ is verified by the verifiers for either disjunct or fusions thereof and falsified by pairwise fusions of falsifiers for the disjuncts.
 Conjunction and disjunction are dual operators obeying the standard idempotence and De Morgan laws.
 The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
 For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
+By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_.
+In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`.
+This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison.
+
 A _necessity sentence_ `Box A` is true at a world just in case every world state includes a part that verifies `A` and a _possibility sentence_ `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
 Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include as parts both `s` and a maximal part of `w` that is compatible with `s`.
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
```

### Comparing `model_checker-0.4.1/README.md` & `model_checker-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 A _negated sentence_ is verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 A _conjunctive sentence_ is verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 A _disjunctive sentence_ is verified by the verifiers for either disjunct or fusions thereof and falsified by pairwise fusions of falsifiers for the disjuncts.
 Conjunction and disjunction are dual operators obeying the standard idempotence and De Morgan laws.
 The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
 For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
+By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_.
+In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`.
+This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison.
+
 A _necessity sentence_ `Box A` is true at a world just in case every world state includes a part that verifies `A` and a _possibility sentence_ `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
 Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include as parts both `s` and a maximal part of `w` that is compatible with `s`.
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
```

### Comparing `model_checker-0.4.1/pyproject.toml` & `model_checker-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.4.1"
+version = "0.4.2"
 description = "A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators."
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
```

### Comparing `model_checker-0.4.1/src/model_checker/__main__.py` & `model_checker-0.4.2/src/model_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.1/src/model_checker/model_definitions.py` & `model_checker-0.4.2/src/model_checker/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.1/src/model_checker/model_structure.py` & `model_checker-0.4.2/src/model_checker/model_structure.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.1/src/model_checker/semantics.py` & `model_checker-0.4.2/src/model_checker/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.1/src/model_checker/syntax.py` & `model_checker-0.4.2/src/model_checker/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.1/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.4.2/src/model_checker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.4.1
+Version: 0.4.2
 Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
@@ -86,14 +86,18 @@
 A _negated sentence_ is verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 A _conjunctive sentence_ is verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 A _disjunctive sentence_ is verified by the verifiers for either disjunct or fusions thereof and falsified by pairwise fusions of falsifiers for the disjuncts.
 Conjunction and disjunction are dual operators obeying the standard idempotence and De Morgan laws.
 The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
 For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
+By contrast with the _bilateral_ extensional operators which treat both verifiers and falsifiers, the semantics for `not` is _unilateral_.
+In particular `not A` is verified by a state `s` just in case every non-null part of `s` is incompatible with a verifier for `A` and every verifier for `A` is incompatible with some non-null part of `s`.
+This semantics is further motivated and elaborated in [Bernard and Champollion](https://ling.auf.net/lingbuzz/007730/current.html) and included here for comparison.
+
 A _necessity sentence_ `Box A` is true at a world just in case every world state includes a part that verifies `A` and a _possibility sentence_ `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
 Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include as parts both `s` and a maximal part of `w` that is compatible with `s`.
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
```

### Comparing `model_checker-0.4.1/test/test.py` & `model_checker-0.4.2/test/test.py`

 * *Files identical despite different names*

