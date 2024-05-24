# Comparing `tmp/openseries-1.5.4.tar.gz` & `tmp/openseries-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openseries-1.5.4.tar", max compression
+gzip compressed data, was "openseries-1.5.5.tar", max compression
```

## Comparing `openseries-1.5.4.tar` & `openseries-1.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1521 2024-05-05 17:48:03.342128 openseries-1.5.4/LICENSE.md
--rw-r--r--   0        0        0    42652 2024-05-05 17:48:03.346128 openseries-1.5.4/README.md
--rw-r--r--   0        0        0       41 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/__init__.py
--rw-r--r--   0        0        0    74705 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/_common_model.py
--rw-r--r--   0        0        0     3300 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/_risk.py
--rw-r--r--   0        0        0    12378 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/datefixer.py
--rw-r--r--   0        0        0    74019 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/frame.py
--rw-r--r--   0        0        0     1856 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/load_plotly.py
--rw-r--r--   0        0        0      178 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/plotly_captor_logo.json
--rw-r--r--   0        0        0     1429 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/plotly_layouts.json
--rw-r--r--   0        0        0    28313 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/series.py
--rw-r--r--   0        0        0    13905 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/simulation.py
--rw-r--r--   0        0        0     7643 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/types.py
--rw-r--r--   0        0        0     2665 2024-05-05 17:48:03.346128 openseries-1.5.4/pyproject.toml
--rw-r--r--   0        0        0    44222 1970-01-01 00:00:00.000000 openseries-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-24 20:14:16.484359 openseries-1.5.5/LICENSE.md
+-rw-r--r--   0        0        0    42652 2024-05-24 20:14:16.484359 openseries-1.5.5/README.md
+-rw-r--r--   0        0        0       41 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/__init__.py
+-rw-r--r--   0        0        0    75497 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/_common_model.py
+-rw-r--r--   0        0        0     3300 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/_risk.py
+-rw-r--r--   0        0        0    12378 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/datefixer.py
+-rw-r--r--   0        0        0    74019 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/frame.py
+-rw-r--r--   0        0        0     1856 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/load_plotly.py
+-rw-r--r--   0        0        0      178 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/plotly_captor_logo.json
+-rw-r--r--   0        0        0     1429 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/plotly_layouts.json
+-rw-r--r--   0        0        0    28313 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/series.py
+-rw-r--r--   0        0        0    13905 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/simulation.py
+-rw-r--r--   0        0        0     7689 2024-05-24 20:14:16.488359 openseries-1.5.5/openseries/types.py
+-rw-r--r--   0        0        0     2665 2024-05-24 20:14:16.488359 openseries-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0    44222 1970-01-01 00:00:00.000000 openseries-1.5.5/PKG-INFO
```

### Comparing `openseries-1.5.4/LICENSE.md` & `openseries-1.5.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/README.md` & `openseries-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/openseries/_common_model.py` & `openseries-1.5.5/openseries/_common_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 )
 from openseries.datefixer import date_offset_foll, holiday_calendar
 from openseries.load_plotly import load_plotly_dict
 from openseries.types import (
     CountriesType,
     DaysInYearType,
     LiteralBarPlotMode,
+    LiteralJsonOutput,
     LiteralLinePlotMode,
     LiteralNanMethod,
     LiteralPlotlyJSlib,
     LiteralPlotlyOutput,
     LiteralQuantileInterp,
     ValueType,
 )
@@ -647,61 +648,73 @@
         drawdown[isnan(drawdown)] = -inf
         roll_max = maximum.accumulate(drawdown, axis=0)
         self.tsdf = DataFrame(drawdown / roll_max - 1.0)
         return self
 
     def to_json(
         self: Self,
+        what_output: LiteralJsonOutput,
         filename: str,
         directory: Optional[DirectoryPath] = None,
     ) -> list[dict[str, Union[str, bool, ValueType, list[str], list[float]]]]:
         """
         Dump timeseries data into a json file.
 
-        The label and tsdf parameters are deleted before the json file is saved
-
         Parameters
         ----------
+        what_output: LiteralJsonOutput
+            Choice on whether the raw values or the tsdf Dataframe values are
+            returned as json and exported as json file.
         filename: str
             Filename including filetype
         directory: DirectoryPath, optional
             File folder location
 
         Returns
         -------
         list[Dict[str, Union[str, bool, ValueType, list[str], list[float]]]]
-            A list of dictionaries with the raw original data of the series
+            A list of dictionaries with the data of the series
 
         """
         if directory:
             dirpath = Path(directory).resolve()
         elif Path.home().joinpath("Documents").exists():
             dirpath = Path.home().joinpath("Documents")
         else:
             dirpath = Path(stack()[1].filename).parent
 
         cleaner_list = ["label", "tsdf"]
         data = dict(self.__dict__)
         output = []
         if "label" in data:
+            if what_output == "tsdf":
+                values = self.tsdf.iloc[:, 0].tolist()
+            else:
+                values = list(cast(list[float], data.get("values")))
             for item in cleaner_list:
                 data.pop(item)
+            valuetype = cast(ValueType, data.get("valuetype")).value
+            data.update({"valuetype": valuetype})
+            data.update({"values": values})
             output.append(dict(data))
         else:
             for serie in cast(list[Any], data.get("constituents")):
+                if what_output == "tsdf":
+                    values = serie.tsdf.iloc[:, 0].tolist()
+                else:
+                    values = list(serie.values)
                 itemdata = dict(serie.__dict__)
                 for item in cleaner_list:
                     itemdata.pop(item)
+                valuetype = cast(ValueType, itemdata["valuetype"]).value
+                itemdata.update({"valuetype": valuetype})
+                itemdata.update({"values": values})
                 output.append(dict(itemdata))
 
-        with Path.open(
-            dirpath.joinpath(filename),
-            "w",
-            encoding="utf-8",
-        ) as jsonfile:
+        with dirpath.joinpath(filename).open(mode="w", encoding="utf-8") as jsonfile:
             dump(output, jsonfile, indent=2, sort_keys=False)
 
         return output
 
     def to_xlsx(
         self: Self,
         filename: str,
```

### Comparing `openseries-1.5.4/openseries/_risk.py` & `openseries-1.5.5/openseries/_risk.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/openseries/datefixer.py` & `openseries-1.5.5/openseries/datefixer.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/openseries/frame.py` & `openseries-1.5.5/openseries/frame.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/openseries/load_plotly.py` & `openseries-1.5.5/openseries/load_plotly.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/openseries/plotly_layouts.json` & `openseries-1.5.5/openseries/plotly_layouts.json`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/openseries/series.py` & `openseries-1.5.5/openseries/series.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/openseries/simulation.py` & `openseries-1.5.5/openseries/simulation.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.4/openseries/types.py` & `openseries-1.5.5/openseries/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         list[str],
         dict[str, Union[str, int, float, bool, list[str]]],
     ],
 ]
 
 CaptorLogoType = dict[str, Union[str, float]]
 
+LiteralJsonOutput = Literal["values", "tsdf"]
 LiteralTrunc = Literal["before", "after", "both"]
 LiteralLinePlotMode = Literal[
     "lines",
     "markers",
     "lines+markers",
     "lines+text",
     "markers+text",
```

### Comparing `openseries-1.5.4/pyproject.toml` & `openseries-1.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openseries"
-version = "1.5.4"
+version = "1.5.5"
 description = "Tools for analyzing financial timeseries."
 authors = ["Martin Karrin <martin.karrin@captor.se>"]
 repository = "https://github.com/CaptorAB/openseries"
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
@@ -46,24 +46,24 @@
 scipy = ">=1.11.4,<2.0.0"
 statsmodels = ">=0.14.0,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.5.1"
 coverage-badge = "^1.1.1"
 mypy = "^1.10.0"
-pandas-stubs = "^2.2.1.240316"
-pre-commit = "^3.7.0"
-pytest = "^8.2.0"
-ruff = "^0.4.3"
+pandas-stubs = "^2.2.2.240514"
+pre-commit = "^3.7.1"
+pytest = "^8.2.1"
+ruff = "^0.4.5"
 types-openpyxl = "^3.1.0.20240428"
 types-python-dateutil = "^2.9.0.20240316"
-types-requests = "^2.31.0.20240406"
+types-requests = "^2.32.0.20240523"
 
 [build-system]
-requires = ["poetry-core>=1.8.2"]
+requires = ["poetry-core>=1.8.3"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning:openpyxl.*:"
 ]
```

### Comparing `openseries-1.5.4/PKG-INFO` & `openseries-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.5.4
+Version: 1.5.5
 Summary: Tools for analyzing financial timeseries.
 Home-page: https://github.com/CaptorAB/openseries
 License: BSD-3-Clause
 Keywords: python,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
 Requires-Python: >=3.9,<3.13
```

