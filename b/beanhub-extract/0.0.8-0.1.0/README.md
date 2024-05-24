# Comparing `tmp/beanhub_extract-0.0.8.tar.gz` & `tmp/beanhub_extract-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_extract-0.0.8.tar", max compression
+gzip compressed data, was "beanhub_extract-0.1.0.tar", max compression
```

## Comparing `beanhub_extract-0.0.8.tar` & `beanhub_extract-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-05-11 07:51:15.529460 beanhub_extract-0.0.8/LICENSE
--rw-r--r--   0        0        0     2934 2024-05-11 07:51:15.529460 beanhub_extract-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/data_types.py
--rw-r--r--   0        0        0      115 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/extractors/__init__.py
--rw-r--r--   0        0        0     2423 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/extractors/mercury.py
--rw-r--r--   0        0        0      977 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/utils.py
--rw-r--r--   0        0        0      587 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 beanhub_extract-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2934 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/beanhub_extract/__init__.py
+-rw-r--r--   0        0        0     2167 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/beanhub_extract/data_types.py
+-rw-r--r--   0        0        0      574 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/beanhub_extract/extractors/__init__.py
+-rw-r--r--   0        0        0      459 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/beanhub_extract/extractors/base.py
+-rw-r--r--   0        0        0     2476 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/beanhub_extract/extractors/chase.py
+-rw-r--r--   0        0        0     3439 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/beanhub_extract/extractors/mercury.py
+-rw-r--r--   0        0        0      977 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/beanhub_extract/utils.py
+-rw-r--r--   0        0        0      618 2024-05-24 00:19:11.537423 beanhub_extract-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 beanhub_extract-0.1.0/PKG-INFO
```

### Comparing `beanhub_extract-0.0.8/LICENSE` & `beanhub_extract-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.8/README.md` & `beanhub_extract-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.8/beanhub_extract/data_types.py` & `beanhub_extract-0.1.0/beanhub_extract/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,7 +48,15 @@
     gl_code: str | None = None
     # Name on the credit/debit card
     name_on_card: str | None = None
     # Last 4 digits of credit/debit card
     last_four_digits: str | None = None
     # All the columns not handled and put into `Transaction`'s attributes by the extractor goes here
     extra: dict | None = None
+
+
+@dataclasses.dataclass
+class Fingerprint:
+    # the starting date of rows
+    starting_date: datetime.date
+    # the hash value of the first row
+    first_row_hash: str
```

### Comparing `beanhub_extract-0.0.8/beanhub_extract/extractors/mercury.py` & `beanhub_extract-0.1.0/beanhub_extract/extractors/mercury.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import csv
 import datetime
 import decimal
+import hashlib
 import os
 import typing
 
 import pytz
 
+from ..data_types import Fingerprint
 from ..data_types import Transaction
+from .base import ExtractorBase
 
 
 def parse_date(date_str: str) -> datetime.date:
     parts = date_str.split("-")
     return datetime.date(int(parts[-1]), *(map(int, parts[:-1])))
 
 
@@ -22,20 +25,55 @@
 def parse_datetime(timestamp_str: str) -> datetime.datetime:
     parts = timestamp_str.split(" ")
     date = parse_date(parts[0])
     time = parse_time(parts[1])
     return datetime.datetime.combine(date, time)
 
 
-class MercuryExtractor:
+class MercuryExtractor(ExtractorBase):
     EXTRACTOR_NAME = "mercury"
     DEFAULT_IMPORT_ID = "{{ file | as_posix_path }}:{{ reversed_lineno }}"
-
-    def __init__(self, input_file: typing.TextIO):
-        self.input_file = input_file
+    ALL_FIELDS = [
+        "Date (UTC)",
+        "Description",
+        "Amount",
+        "Status",
+        "Source Account",
+        "Bank Description",
+        "Reference",
+        "Note",
+        "Last Four Digits",
+        "Name On Card",
+        "Category",
+        "GL Code",
+        "Timestamp",
+        "Original Currency",
+    ]
+
+    def detect(self) -> bool:
+        reader = csv.DictReader(self.input_file)
+        try:
+            return reader.fieldnames == self.ALL_FIELDS
+        except Exception:
+            return False
+
+    def fingerprint(self) -> Fingerprint | None:
+        reader = csv.DictReader(self.input_file)
+        row = None
+        for row in reader:
+            pass
+        if row is None:
+            return
+        hash = hashlib.sha256()
+        for field in reader.fieldnames:
+            hash.update(row[field].encode("utf8"))
+        return Fingerprint(
+            starting_date=parse_date(row["Date (UTC)"]),
+            first_row_hash=hash.hexdigest(),
+        )
 
     def __call__(self) -> typing.Generator[Transaction, None, None]:
         filename = None
         if hasattr(self.input_file, "name"):
             filename = self.input_file.name
         row_count_reader = csv.DictReader(self.input_file)
         row_count = 0
```

### Comparing `beanhub_extract-0.0.8/beanhub_extract/utils.py` & `beanhub_extract-0.1.0/beanhub_extract/utils.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.8/pyproject.toml` & `beanhub_extract-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "beanhub-extract"
-version = "0.0.8"
+version = "0.1.0"
 description = "The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytz = ">= 2023.1, <2025"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.1"
 pytest-mock = "^3.11.1"
+pytest-lazy-fixture = "^0.6.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `beanhub_extract-0.0.8/PKG-INFO` & `beanhub_extract-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-extract
-Version: 0.0.8
+Version: 0.1.0
 Summary: The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beanhub-extract Version: 0.0.8 Summary: The simple
+Metadata-Version: 2.1 Name: beanhub-extract Version: 0.1.0 Summary: The simple
 library for extracting all kind of bank account transaction export files,
 mostly for beanhub-import to inject and generate transactions License: MIT
 Author: Fang-Pen Lin Author-email: fangpen@launchplatform.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: pytz (>=2023.1,<2025)
```

