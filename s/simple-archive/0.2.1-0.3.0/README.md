# Comparing `tmp/simple_archive-0.2.1.tar.gz` & `tmp/simple_archive-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_archive-0.2.1.tar", last modified: Thu May 16 08:29:21 2024, max compression
+gzip compressed data, was "simple_archive-0.3.0.tar", last modified: Fri May 24 12:39:05 2024, max compression
```

## Comparing `simple_archive-0.2.1.tar` & `simple_archive-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1077 2024-05-16 08:29:04.700432 simple_archive-0.2.1/LICENSE
--rw-r--r--   0        0        0     2292 2024-05-16 08:29:04.700432 simple_archive-0.2.1/README.md
--rw-r--r--   0        0        0     1300 2024-05-16 08:29:21.084499 simple_archive-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      148 2024-05-16 08:29:04.700432 simple_archive-0.2.1/simple_archive/__init__.py
--rw-r--r--   0        0        0      598 2024-05-16 08:29:04.700432 simple_archive-0.2.1/simple_archive/cli.py
--rw-r--r--   0        0        0     6968 2024-05-16 08:29:04.700432 simple_archive-0.2.1/simple_archive/simple_archive.py
--rw-r--r--   0        0        0     2594 2024-05-16 08:29:04.700432 simple_archive-0.2.1/simple_archive/use_cases.py
--rw-r--r--   0        0        0    18267 2024-05-16 08:29:04.700432 simple_archive-0.2.1/tests/requirements-testing.lock
--rw-r--r--   0        0        0      121 2024-05-16 08:29:04.700432 simple_archive-0.2.1/tests/test_dublin_core.py
--rw-r--r--   0        0        0      362 2024-05-16 08:29:04.700432 simple_archive-0.2.1/tests/test_simple_archive.py
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 simple_archive-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-24 12:38:52.528104 simple_archive-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2440 2024-05-24 12:38:52.528104 simple_archive-0.3.0/README.md
+-rw-r--r--   0        0        0     1300 2024-05-24 12:39:05.128226 simple_archive-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      148 2024-05-24 12:38:52.528104 simple_archive-0.3.0/simple_archive/__init__.py
+-rw-r--r--   0        0        0      598 2024-05-24 12:38:52.528104 simple_archive-0.3.0/simple_archive/cli.py
+-rw-r--r--   0        0        0     3925 2024-05-24 12:38:52.528104 simple_archive-0.3.0/simple_archive/file_system.py
+-rw-r--r--   0        0        0     9914 2024-05-24 12:38:52.528104 simple_archive-0.3.0/simple_archive/simple_archive.py
+-rw-r--r--   0        0        0     2594 2024-05-24 12:38:52.528104 simple_archive-0.3.0/simple_archive/use_cases.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:38:52.528104 simple_archive-0.3.0/tests/data/gen/.keep
+-rw-r--r--   0        0        0        6 2024-05-24 12:38:52.528104 simple_archive-0.3.0/tests/data/values.txt
+-rw-r--r--   0        0        0    18267 2024-05-24 12:38:52.528104 simple_archive-0.3.0/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     1399 2024-05-24 12:38:52.528104 simple_archive-0.3.0/tests/test_dublin_core.py
+-rw-r--r--   0        0        0     5335 2024-05-24 12:38:52.528104 simple_archive-0.3.0/tests/test_simple_archive.py
+-rw-r--r--   0        0        0     3397 1970-01-01 00:00:00.000000 simple_archive-0.3.0/PKG-INFO
```

### Comparing `simple_archive-0.2.1/LICENSE` & `simple_archive-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_archive-0.2.1/README.md` & `simple_archive-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,24 @@
 Run `safar <path/to/csv>`
 
 - Use `--zip` if you want to create a zip-archive.
 - By default all archives is written to `./output` but you can give `--output dir` to change that.
 
 ### CSV Format
 
-The expected CSV format is shown below where the metadata is given in the form `namespace.element[.qualifier[.language]]`.
+The expected CSV format is shown below where the metadata is given in the form `namespace.element[.qualifier]`.
 
-**NOTE** Currently only the `dc` namespace is handled.
+Language can be specified by `namespace.element[language]` or `namespace.element.qualifier[language]`
+
+Example: `dc.description[sv_SE]`
+
+Supported namespaces:
+
+- `dc` (required)
+- `local`
+- `metashare`
+- `dcterms`
 
 ```csv
 files,dc.title,dc.date.issued,...
 filename1||filename2,Title,2023-03-14,...
 ``
```

### Comparing `simple_archive-0.2.1/pyproject.toml` & `simple_archive-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simple-archive"
-version = "0.2.1"
+version = "0.3.0"
 description = "CLI and library for working with Simple Archive Format"
 authors = [
     { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `simple_archive-0.2.1/simple_archive/cli.py` & `simple_archive-0.3.0/simple_archive/cli.py`

 * *Files identical despite different names*

### Comparing `simple_archive-0.2.1/simple_archive/simple_archive.py` & `simple_archive-0.3.0/simple_archive/simple_archive.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 """Model for Simple Archive."""
 
 import csv
 import logging
-import shutil
+import re
+import zipfile
 from datetime import date
 from pathlib import Path
-from typing import Any, Optional
+from typing import IO, Any, Optional, Union
 from xml.etree.ElementTree import Element, ElementTree, SubElement
-from zipfile import ZIP_DEFLATED, ZipFile
 
 import pydantic
+from typing_extensions import Self
+
+from simple_archive.file_system import (
+    FileSystem,
+    PathFileSystem,
+    ZipFileSystem,
+)
 
 DEFAULT_ENCODING = "utf-8"
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -28,31 +35,61 @@
 
     element: str
     value: str
     qualifier: Optional[str] = None
     language: Optional[str] = None
 
 
-class DublinCore(pydantic.BaseModel):
+LANGUAGE_IN_SQUARE_BRACKETS = re.compile(r"\[([a-zA-Z_]+)\]")
+
+
+class DublinCore(pydantic.RootModel):
     """Dublin Core model."""
 
-    elements: list[DublinCoreElement]
+    root: list[DublinCoreElement]
+
+    @pydantic.model_validator(mode="before")
+    @classmethod
+    def build_list_from_dict_if_needed(cls, values: Any) -> list:  # noqa: D102
+        if isinstance(values, list):
+            return values
+        new_values = []
+        for key, value in values.items():
+            if isinstance(value, str):
+                new_value = {"element": key, "value": value}
+                if lang := LANGUAGE_IN_SQUARE_BRACKETS.search(key):
+                    new_value["element"] = key[: lang.start()]
+                    new_value["language"] = lang.group(1)
+                new_values.append(new_value)
+            elif isinstance(value, dict):
+                new_value = {"element": key}
+                for key1, value1 in value.items():
+                    if key1 == "value":
+                        new_value["value"] = value1
+                    elif key1 == "language":
+                        new_value["language"] = value1
+                    else:
+                        new_value["qualifier"] = key1
+                        new_value["value"] = value1
+                new_values.append(new_value)
+        return new_values
 
 
-def build_xml(dc: DublinCore) -> ElementTree:
+def build_xml(dc: DublinCore, *, schema: str) -> ElementTree:
     """Build an ElementTree from a DublinCore model.
 
     Args:
         dc (DublinCore): the model to build from
+        schema (str): the schema to annotate dublin_core with
 
     Returns:
         ElementTree: the resulting ElementTree
     """
-    root = Element("dublin_core")
-    for element in dc.elements:
+    root = Element("dublin_core", attrib={"schema": schema})
+    for element in dc.root:
         dcvalue(
             root,
             element=element.element,
             qualifier=element.qualifier,
             language=element.language,
             text=element.value,
         )
@@ -86,116 +123,177 @@
         attribs["language"] = language
     elem = SubElement(parent, "dcvalue", attrib=attribs)
     if text:
         elem.text = text
     return elem
 
 
+class Metadata(pydantic.BaseModel):
+    """Model of metadata."""
+
+    model_config = pydantic.ConfigDict(extra="forbid")
+
+    dc: DublinCore
+    local: Optional[DublinCore] = None
+    dcterms: Optional[DublinCore] = None
+    metashare: Optional[DublinCore] = None
+
+    @pydantic.field_validator("dcterms")
+    @classmethod
+    def set_language_for_dcterms(cls, v: Optional[DublinCore]) -> Optional[DublinCore]:
+        """Set language if not set."""
+        if not v:
+            return v
+        for elem in v.root:
+            if elem.language is None:
+                elem.language = "*"
+        return v
+
+    @pydantic.field_validator("metashare")
+    @classmethod
+    def set_language_for_metashare(cls, v: Optional[DublinCore]) -> Optional[DublinCore]:
+        """Set language if not set."""
+        if not v:
+            return v
+        for elem in v.root:
+            if elem.language is None:
+                elem.language = "en_US"
+        return v
+
+
 class Item(pydantic.BaseModel):
     """Simple Archive Item model."""
 
     files: list[Path]
-    dc: DublinCore
+    metadata: Metadata
 
     @pydantic.field_validator("files", mode="before")
     @classmethod
     def split_str(cls, v: Any) -> Any:  # noqa: D102
-        return v.split("||") if isinstance(v, str) else v
+        if isinstance(v, str):
+            return v.split("||") if v else []
+        return v
+
+    @pydantic.model_validator(mode="after")
+    def check_if_has_files(self) -> Self:  # noqa: D102
+        if len(self.files) > 0:
+            elem = DublinCoreElement(element="has", value="yes", qualifier="files")
+        else:
+            elem = DublinCoreElement(element="has", value="no", qualifier="files")
+
+        if self.metadata.local is None:
+            self.metadata.local = DublinCore(root=[elem])
+            return self
+        for local_elem in self.metadata.local.root:
+            if local_elem.element == elem.element and local_elem.qualifier == elem.qualifier:
+                local_elem.value = elem.value
+                return self
+
+        self.metadata.local.root.append(elem)
+        return self
 
     @pydantic.model_validator(mode="before")
     @classmethod
-    def collect_dc_fields(cls, values: Any) -> dict:  # noqa: D102
-        new_values: dict[str, dict[str, list[dict[str, str]]]] = {}
-        for field, value in values.items():
-            if field.startswith("dc."):
-                if "dc" not in new_values:
-                    new_values["dc"] = {}
-                if "elements" not in new_values["dc"]:
-                    new_values["dc"]["elements"] = []
-                subfields: list[str] = field.split(".")
-                element = {"value": value}
-                for sub_field, key in zip(
-                    subfields[1:],
-                    (
-                        "element",
-                        "qualifier",
-                        "language",
-                    ),  # strict=False TODO: use this when Python 3.9 is dropped, see https://github.com/spraakbanken/simple-archive/issuse/5
-                ):
-                    element[key] = sub_field  # noqa: PERF403
-                new_values["dc"]["elements"].append(element)
-                # new_values["dc"][field[3:]] = value
+    def unflatten_values(cls, values: Any) -> dict:  # noqa: D102
+        nested: dict = {}
+        for key, value in values.items():
+            parts = key.split(".")
+            sub = nested
+
+            for part in parts[:-1]:
+                if part not in sub:
+                    sub[part] = {}
+                sub = sub[part]
+
+            sub[parts[-1]] = value
+        new_values: dict = {"metadata": {}}
+        for key, value in nested.items():
+            if key == "files":
+                new_values["files"] = value
+            elif isinstance(value, pydantic.BaseModel):
+                new_values[key] = value
             else:
-                new_values[field] = value
+                new_values["metadata"][key] = value
         return new_values
 
 
 class SimpleArchive:
     """Simple Archive model."""
 
-    def __init__(self, input_folder: Path, items: list) -> None:  # noqa: D107
+    def __init__(self, input_folder: Path, items: list[Item]) -> None:  # noqa: D107
         self.input_folder = input_folder
         self.items = items
 
     @classmethod
     def from_csv_path(cls, csv_path: Path) -> "SimpleArchive":  # noqa: D102
         items = []
         with open(csv_path, encoding=DEFAULT_ENCODING, newline="") as csvfile:  # noqa: PTH123
             reader = csv.DictReader(csvfile)
             for row in reader:
                 item = Item(**row)
                 items.append(item)
         return cls(input_folder=csv_path.parent, items=items)
 
     def write_to_path(self, output_path: Path) -> None:  # noqa: D102
-        for item_nr, item in enumerate(self.items):
-            item_path = output_path / f"item_{item_nr:03d}"
-            logger.info("creating '%s' ...", item_path)
-            item_path.mkdir(parents=True, exist_ok=False)
-
-            self.write_contents_file(item, item_path)
-            self.copy_files(item, item_path)
-            self.write_metadata(item, item_path)
+        path_fs = PathFileSystem(output_path)
+        self._write_to_fs(path_fs)
 
     def write_to_zip(self, output_path: Path) -> None:  # noqa: D102
-        with ZipFile(output_path, "w", compression=ZIP_DEFLATED) as zipfile:
-            for item_nr, item in enumerate(self.items):
-                item_path = f"item_{item_nr:03d}"
-                # zipfile.mkdir(item_path)
-                # copy files
-                for file_path in item.files:
-                    src_path = self.input_folder / file_path
-                    dst_path = f"{item_path}/{file_path}"
-                    zipfile.write(src_path, dst_path)
-                # write contents
-                contents_path = f"{item_path}/contents"
-                with zipfile.open(contents_path, "w") as contents_file:
-                    for file_path in item.files:
-                        contents_file.write(file_path.name.encode("utf-8"))
-                        contents_file.write(b"\n")
-                # write metadata
-                dublin_core_xml = build_xml(item.dc)
-                dublin_core_path = f"{item_path}/dublin_core.xml"
-                logger.info("writing '%s'in zip-archive ", dublin_core_path)
-                with zipfile.open(dublin_core_path, "w") as dublin_core_file:
-                    dublin_core_xml.write(dublin_core_file)
+        with zipfile.ZipFile(output_path, "w", compression=zipfile.ZIP_DEFLATED) as zipf:
+            zip_fs = ZipFileSystem(zipf)
+            self._write_to_fs(zip_fs)
 
-    def write_contents_file(self, item: Item, item_path: Path) -> None:  # noqa: PLR6301, D102
-        contents_path = item_path / "contents"
+    def _write_to_fs(self, fs: FileSystem) -> None:
+        for item_nr, item in enumerate(self.items):
+            item_path = f"item_{item_nr:03d}"
+            fs.mkdir(item_path)
+
+            self._write_contents_file(item, item_path, fs)
+            self._copy_files(item, item_path, fs)
+            self._write_metadata(item.metadata, item_path, fs)
+
+    def _write_contents_file(self, item: Item, item_path: str, fs: FileSystem) -> None:  # noqa: PLR6301
+        contents_path = f"{item_path}/contents"
         logger.info("writing '%s'", contents_path)
-        with contents_path.open(mode="w", encoding="utf-8") as contents_file:
+        with fs.open_text(contents_path) as contents_file:
             for file_path in item.files:
                 contents_file.write(file_path.name)
                 contents_file.write("\n")
 
-    def copy_files(self, item: Item, item_path: Path) -> None:  # noqa: D102
+    def _copy_files(self, item: Item, item_path: str, fs: FileSystem) -> None:
         for file_path in item.files:
             src_path = self.input_folder / file_path
-            dst_path = item_path
+            dst_path = f"{item_path}/{file_path}"
             logger.info("  copying '%s to '%s'", src_path, dst_path)
-            shutil.copy(src_path, dst_path)
+            fs.copy(src_path, dst_path)
 
-    def write_metadata(self, item: Item, item_path: Path) -> None:  # noqa: D102, PLR6301
-        dublin_core_xml = build_xml(item.dc)
-        dublin_core_path = item_path / "dublin_core.xml"
-        logger.info("writing '%s'", dublin_core_path)
-        dublin_core_xml.write(dublin_core_path)
+    def _write_metadata(self, metadata: Metadata, item_path: str, fs: FileSystem) -> None:  # noqa: PLR6301
+        with fs.open_bytes(f"{item_path}/dublin_core.xml") as dc_file:
+            build_and_write_metadata(metadata.dc, schema="dc", path_or_file=dc_file)
+
+        if metadata.local:
+            with fs.open_bytes(f"{item_path}/metadata_local.xml") as local_file:
+                build_and_write_metadata(metadata.local, schema="local", path_or_file=local_file)
+        if metadata.dcterms:
+            with fs.open_bytes(f"{item_path}/metadata_dcterms.xml") as dcterms_file:
+                build_and_write_metadata(
+                    metadata.dcterms, schema="dcterms", path_or_file=dcterms_file
+                )
+        if metadata.metashare:
+            with fs.open_bytes(f"{item_path}/metadata_metashare.xml") as metashare_file:
+                build_and_write_metadata(
+                    metadata.metashare, schema="metashare", path_or_file=metashare_file
+                )
+
+
+def build_and_write_metadata(
+    metadata: DublinCore, schema: str, path_or_file: Union[Path, IO[bytes]]
+) -> None:
+    """Build and write metadata.
+
+    Args:
+        metadata (DublinCore): metadata to build
+        schema (str): schema to use
+        path_or_file (Union[Path, IO[bytes]]): path or file to write to
+    """
+    metadata_xml = build_xml(metadata, schema=schema)
+    metadata_xml.write(path_or_file, encoding="utf-8", xml_declaration=True)
```

### Comparing `simple_archive-0.2.1/simple_archive/use_cases.py` & `simple_archive-0.3.0/simple_archive/use_cases.py`

 * *Files identical despite different names*

### Comparing `simple_archive-0.2.1/tests/requirements-testing.lock` & `simple_archive-0.3.0/tests/requirements-testing.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is @generated by PDM.
 # Please do not edit it manually.
 
-annotated-types==0.6.0 \
-    --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
-    --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
+annotated-types==0.7.0 \
+    --hash=sha256:1f02e8b43a8fbbc3f3e0d4f0f4bfc8131bcb4eebe8849b8e5c773f3a1c582a53 \
+    --hash=sha256:aff07c09a53a08bc8cfccb9c85b05f1aa9a2a6f23728d790723543408344ce89
 bracex==2.4 \
     --hash=sha256:a27eaf1df42cf561fed58b7a8f3fdf129d1ea16a81e1fadd1d17989bc6384beb \
     --hash=sha256:efdc71eff95eaff5e0f8cfebe7d01adf2c8637c8c92edaf63ef348c241a82418
-bump-my-version==0.21.0 \
-    --hash=sha256:a614d8176b5ac0e644239c9a8a246b696d316f68406fd78b8486a9e13fc93266 \
-    --hash=sha256:c3f1a31e32345679b517cbba99a0875457ee45d7ba6189fcd2a74d3ddae41515
+bump-my-version==0.21.1 \
+    --hash=sha256:946a7edcf30c5a8574c579684df983136ea395f70c184e4db32eb3e307584c14 \
+    --hash=sha256:ec612474e9e790c3fbbfed153a10b356f84fc15096ceff181b399d5e985bfacc
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 colorama==0.4.6; sys_platform == "win32" or platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 coverage==7.5.1 \
@@ -179,17 +179,17 @@
     --hash=sha256:fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
 pydantic-settings==2.2.1 \
     --hash=sha256:00b9f6a5e95553590434c0fa01ead0b216c3e10bc54ae02e37f359948643c5ed \
     --hash=sha256:0235391d26db4d2190cb9b31051c4b46882d28a51533f97440867f012d4da091
 pygments==2.18.0 \
     --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
     --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
-pytest==8.2.0 \
-    --hash=sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233 \
-    --hash=sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f
+pytest==8.2.1 \
+    --hash=sha256:5046e5b46d8e4cac199c373041f26be56fdb81eb4e67dc11d4e10811fc3408fd \
+    --hash=sha256:faccc5d332b8c3719f40283d0d44aa5cf101cec36f88cde9ed8f2bc0538612b1
 pytest-cov==5.0.0 \
     --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
     --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
 python-dotenv==1.0.1 \
     --hash=sha256:e324ee90a023d808f1959c46bcbc04446a10ced277783dc6ee09987c37ec10ca \
     --hash=sha256:f7b63ef50f1b690dddf550d03497b66d609393b40b564ed0d674909a68ebf16a
 questionary==2.0.1 \
@@ -197,46 +197,46 @@
     --hash=sha256:bcce898bf3dbb446ff62830c86c5c6fb9a22a54146f0f5597d3da43b10d8fc8b
 rich==13.7.1 \
     --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
     --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
 rich-click==1.8.2 \
     --hash=sha256:8e29bdede858b59aa2859a1ab1c4ccbd39ed7ed5870262dae756fba6b5dc72e8 \
     --hash=sha256:b57856f304e4fe0394b82d7ce0784450758f8c8b4e201ccc4320501cc201806b
-ruff==0.4.4 \
-    --hash=sha256:1aecced1269481ef2894cc495647392a34b0bf3e28ff53ed95a385b13aa45768 \
-    --hash=sha256:29d44ef5bb6a08e235c8249294fa8d431adc1426bfda99ed493119e6f9ea1bf6 \
-    --hash=sha256:39df0537b47d3b597293edbb95baf54ff5b49589eb7ff41926d8243caa995ea6 \
-    --hash=sha256:424e5b72597482543b684c11def82669cc6b395aa8cc69acc1858b5ef3e5daae \
-    --hash=sha256:4c8e2f1e8fc12d07ab521a9005d68a969e167b589cbcaee354cb61e9d9de9c15 \
-    --hash=sha256:60ed88b636a463214905c002fa3eaab19795679ed55529f91e488db3fe8976ab \
-    --hash=sha256:8e7e6ebc10ef16dcdc77fd5557ee60647512b400e4a60bdc4849468f076f6eef \
-    --hash=sha256:958b4ea5589706a81065e2a776237de2ecc3e763342e5cc8e02a4a4d8a5e6f95 \
-    --hash=sha256:9da73eb616b3241a307b837f32756dc20a0b07e2bcb694fec73699c93d04a69e \
-    --hash=sha256:b1867ee9bf3acc21778dcb293db504692eda5f7a11a6e6cc40890182a9f9e595 \
-    --hash=sha256:b5eb0a4bfd6400b7d07c09a7725e1a98c3b838be557fee229ac0f84d9aa49c36 \
-    --hash=sha256:b90fc5e170fc71c712cc4d9ab0e24ea505c6a9e4ebf346787a67e691dfb72e85 \
-    --hash=sha256:b9ddb2c494fb79fc208cd15ffe08f32b7682519e067413dbaf5f4b01a6087bcd \
-    --hash=sha256:c4efe62b5bbb24178c950732ddd40712b878a9b96b1d02b0ff0b08a090cbd891 \
-    --hash=sha256:c51c928a14f9f0a871082603e25a1588059b7e08a920f2f9fa7157b5bf08cfe9 \
-    --hash=sha256:cb53473849f011bca6e754f2cdf47cafc9c4f4ff4570003a0dad0b9b6890e876 \
-    --hash=sha256:f87ea42d5cdebdc6a69761a9d0bc83ae9b3b30d0ad78952005ba6568d6c022af
+ruff==0.4.5 \
+    --hash=sha256:1169e47e9c4136c997f08f9857ae889d614c5035d87d38fda9b44b4338909cdf \
+    --hash=sha256:25f483ad9d50b00e7fd577f6d0305aa18494c6af139bce7319c68a17180087f4 \
+    --hash=sha256:286eabd47e7d4d521d199cab84deca135557e6d1e0f0d01c29e757c3cb151b54 \
+    --hash=sha256:441dab55c568e38d02bbda68a926a3d0b54f5510095c9de7f95e47a39e0168aa \
+    --hash=sha256:63fde3bf6f3ad4e990357af1d30e8ba2730860a954ea9282c95fc0846f5f64af \
+    --hash=sha256:6e1b139b45e2911419044237d90b60e472f57285950e1492c757dfc88259bb06 \
+    --hash=sha256:755ac9ac2598a941512fc36a9070a13c88d72ff874a9781493eb237ab02d75df \
+    --hash=sha256:75a426506a183d9201e7e5664de3f6b414ad3850d7625764106f7b6d0486f0a1 \
+    --hash=sha256:78e3ba4620dee27f76bbcad97067766026c918ba0f2d035c2fc25cbdd04d9c97 \
+    --hash=sha256:84dd157474e16e3a82745d2afa1016c17d27cb5d52b12e3d45d418bcc6d49264 \
+    --hash=sha256:8f58e615dec58b1a6b291769b559e12fdffb53cc4187160a2fc83250eaf54e96 \
+    --hash=sha256:9d15de3425f53161b3f5a5658d4522e4eee5ea002bf2ac7aa380743dd9ad5fba \
+    --hash=sha256:a6f29a8221d2e3d85ff0c7b4371c0e37b39c87732c969b4d90f3dad2e721c5b1 \
+    --hash=sha256:aed8166c18b1a169a5d3ec28a49b43340949e400665555b51ee06f22813ef062 \
+    --hash=sha256:b0b03c619d2b4350b4a27e34fd2ac64d0dabe1afbf43de57d0f9d8a05ecffa45 \
+    --hash=sha256:d6ef817124d72b54cc923f3444828ba24fa45c3164bc9e8f1813db2f3d3a8a11 \
+    --hash=sha256:f4b02a65985be2b34b170025a8b92449088ce61e33e69956ce4d316c0fe7cce0
 shellingham==1.5.4 \
     --hash=sha256:7ecfff8f2fd72616f7481040475a65b2bf8af90a56c89140852d1120324e8686 \
     --hash=sha256:8dbca0739d487e5bd35ab3ca4b36e11c4078f3a234bfce294b0a0291363404de
 tomli==2.0.1; python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
 tomlkit==0.12.5 \
     --hash=sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f \
     --hash=sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c
 typer==0.12.3 \
     --hash=sha256:070d7ca53f785acbccba8e7d28b08dcd88f79f1fbda035ade0aecec71ca5c914 \
     --hash=sha256:49e73131481d804288ef62598d97a1ceef3058905aa536a1134f90891ba35482
-typing-extensions==4.11.0 \
-    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
-    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+typing-extensions==4.12.0 \
+    --hash=sha256:8cbcdc8606ebcb0d95453ad7dc5065e6237b6aa230a31e81d0f440c30fed5fd8 \
+    --hash=sha256:b349c66bea9016ac22978d800cfff206d5f9816951f12a7d0ec5578b0a819594
 wcmatch==8.5.2 \
     --hash=sha256:17d3ad3758f9d0b5b4dedc770b65420d4dac62e680229c287bf24c9db856a478 \
     --hash=sha256:a70222b86dea82fb382dd87b73278c10756c138bd6f8f714e2183128887b9eb2
 wcwidth==0.2.13 \
     --hash=sha256:3da69048e4540d84af32131829ff948f1e022c1c6bdb8d6102117aac784f6859 \
     --hash=sha256:72ea0c06399eb286d978fdedb6923a9eb47e1c486ce63e9b4e64fc18303972b5
```

### Comparing `simple_archive-0.2.1/PKG-INFO` & `simple_archive-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-archive
-Version: 0.2.1
+Version: 0.3.0
 Summary: CLI and library for working with Simple Archive Format
 Author-Email: =?utf-8?q?Spr=C3=A5kbanken_Text?= <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
@@ -66,15 +66,24 @@
 Run `safar <path/to/csv>`
 
 - Use `--zip` if you want to create a zip-archive.
 - By default all archives is written to `./output` but you can give `--output dir` to change that.
 
 ### CSV Format
 
-The expected CSV format is shown below where the metadata is given in the form `namespace.element[.qualifier[.language]]`.
+The expected CSV format is shown below where the metadata is given in the form `namespace.element[.qualifier]`.
 
-**NOTE** Currently only the `dc` namespace is handled.
+Language can be specified by `namespace.element[language]` or `namespace.element.qualifier[language]`
+
+Example: `dc.description[sv_SE]`
+
+Supported namespaces:
+
+- `dc` (required)
+- `local`
+- `metashare`
+- `dcterms`
 
 ```csv
 files,dc.title,dc.date.issued,...
 filename1||filename2,Title,2023-03-14,...
 ``
```

