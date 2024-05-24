# Comparing `tmp/fundamend-0.0.1.tar.gz` & `tmp/fundamend-0.1.0.tar.gz`

## Comparing `fundamend-0.0.1.tar` & `fundamend-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fundamend-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fundamend-0.0.1/README.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fundamend-0.0.1/domain-specific-terms.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fundamend-0.0.1/requirements.txt
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 fundamend-0.0.1/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fundamend-0.0.1/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fundamend-0.0.1/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fundamend-0.0.1/src/_fundamend_version.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fundamend-0.0.1/src/fundamend/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fundamend-0.0.1/src/fundamend/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fundamend-0.0.1/src/fundamend/models/__init__.py
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 fundamend-0.0.1/src/fundamend/models/messageimplementationguide.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fundamend-0.0.1/src/fundamend/reader/__init__.py
--rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 fundamend-0.0.1/src/fundamend/reader/migreader.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fundamend-0.0.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fundamend-0.0.1/LICENSE
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 fundamend-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 fundamend-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fundamend-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 fundamend-0.1.0/README.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fundamend-0.1.0/domain-specific-terms.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fundamend-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 fundamend-0.1.0/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fundamend-0.1.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fundamend-0.1.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fundamend-0.1.0/src/_fundamend_version.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fundamend-0.1.0/src/fundamend/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fundamend-0.1.0/src/fundamend/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fundamend-0.1.0/src/fundamend/models/__init__.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 fundamend-0.1.0/src/fundamend/models/messageimplementationguide.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fundamend-0.1.0/src/fundamend/reader/__init__.py
+-rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 fundamend-0.1.0/src/fundamend/reader/migreader.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fundamend-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fundamend-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 fundamend-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 fundamend-0.1.0/PKG-INFO
```

### Comparing `fundamend-0.0.1/.pre-commit-config.yaml` & `fundamend-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/README.md` & `fundamend-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ## Sinn und Zweck
 Seit 2024 bietet der BDEW (endlich) maschinenlesbare MIG- und AHB-Spezifikationen an, wo zuvor nur PDF oder Word-Dateien veröffentlicht wurden.
 Das ist ein wichtiger Schritt für eine echte Digitalisierung der Marktkommunikation im deutschen Energiemarkt.
 
 Die nun maschinenlesbaren Informationen über den Aufgabe von EDIFACT-Nachrichten sind XML-basiert.
 
-Dieses Repository enthält ein kleines Python-Paket, das die XML-Dateien einliest und als Python-Objekte zur Verfügung stellt, damit sich niemand mit XML herumschlagen muss.
+Dieses Repository enthält ein kleines Python-Paket, das die XML-Dateien einliest und als vollständig typisierte Python-Objekte zur Verfügung stellt, damit sich niemand mit XML herumschlagen muss.
 Das ist alles.
 
 ## Installation und Verwendung
 Das Paket ist auf PyPI verfügbar und kann mit pip installiert werden:
 ```bash
 pip install fundamend
 ```
```

### Comparing `fundamend-0.0.1/tox.ini` & `fundamend-0.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/dependabot.yml` & `fundamend-0.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/workflows/coverage.yml` & `fundamend-0.1.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/workflows/dependabot_automerge.yml` & `fundamend-0.1.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/workflows/dev_test.yml` & `fundamend-0.1.0/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/workflows/formatting.yml` & `fundamend-0.1.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/workflows/packaging_test.yml` & `fundamend-0.1.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/workflows/python-publish.yml` & `fundamend-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/workflows/pythonlint.yml` & `fundamend-0.1.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.github/workflows/unittests.yml` & `fundamend-0.1.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/dev_requirements/requirements-packaging.txt` & `fundamend-0.1.0/dev_requirements/requirements-packaging.txt`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/src/fundamend/models/messageimplementationguide.py` & `fundamend-0.1.0/src/fundamend/models/messageimplementationguide.py`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/src/fundamend/reader/migreader.py` & `fundamend-0.1.0/src/fundamend/reader/migreader.py`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/.gitignore` & `fundamend-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/LICENSE` & `fundamend-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/pyproject.toml` & `fundamend-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fundamend-0.0.1/PKG-INFO` & `fundamend-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fundamend
-Version: 0.0.1
+Version: 0.1.0
 Summary: XML basierte Formate und DatemModelle für die Energiewirtschaft in Deutschland
 Project-URL: Changelog, https://github.com/Hochfrequenz/xml-fundamend/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/xml-fundamend
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: AHB,BDEW,MIG,Marktkommunikation,XML
@@ -34,15 +34,15 @@
 
 ## Sinn und Zweck
 Seit 2024 bietet der BDEW (endlich) maschinenlesbare MIG- und AHB-Spezifikationen an, wo zuvor nur PDF oder Word-Dateien veröffentlicht wurden.
 Das ist ein wichtiger Schritt für eine echte Digitalisierung der Marktkommunikation im deutschen Energiemarkt.
 
 Die nun maschinenlesbaren Informationen über den Aufgabe von EDIFACT-Nachrichten sind XML-basiert.
 
-Dieses Repository enthält ein kleines Python-Paket, das die XML-Dateien einliest und als Python-Objekte zur Verfügung stellt, damit sich niemand mit XML herumschlagen muss.
+Dieses Repository enthält ein kleines Python-Paket, das die XML-Dateien einliest und als vollständig typisierte Python-Objekte zur Verfügung stellt, damit sich niemand mit XML herumschlagen muss.
 Das ist alles.
 
 ## Installation und Verwendung
 Das Paket ist auf PyPI verfügbar und kann mit pip installiert werden:
 ```bash
 pip install fundamend
 ```
```

