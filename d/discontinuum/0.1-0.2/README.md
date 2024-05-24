# Comparing `tmp/discontinuum-0.1.tar.gz` & `tmp/discontinuum-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discontinuum-0.1.tar", last modified: Tue May  7 14:18:15 2024, max compression
+gzip compressed data, was "discontinuum-0.2.tar", last modified: Fri May 24 15:31:22 2024, max compression
```

## Comparing `discontinuum-0.1.tar` & `discontinuum-0.2.tar`

### file list

```diff
@@ -1,36 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:15.495016 discontinuum-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:15.487016 discontinuum-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:15.491016 discontinuum-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-07 14:18:09.000000 discontinuum-0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 14:18:09.000000 discontinuum-0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-07 14:18:09.000000 discontinuum-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-07 14:18:09.000000 discontinuum-0.1/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-07 14:18:09.000000 discontinuum-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-07 14:18:09.000000 discontinuum-0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 14:18:15.495016 discontinuum-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 14:18:09.000000 discontinuum-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:15.491016 discontinuum-0.1/discontinuum/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-07 14:18:15.000000 discontinuum-0.1/discontinuum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:15.491016 discontinuum-0.1/discontinuum/models/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/models/pymc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:15.491016 discontinuum-0.1/discontinuum/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/providers/usgs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:15.491016 discontinuum-0.1/discontinuum/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-07 14:18:09.000000 discontinuum-0.1/discontinuum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:18:15.495016 discontinuum-0.1/discontinuum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 14:18:15.000000 discontinuum-0.1/discontinuum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-07 14:18:15.000000 discontinuum-0.1/discontinuum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:18:15.000000 discontinuum-0.1/discontinuum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 14:18:15.000000 discontinuum-0.1/discontinuum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 14:18:15.000000 discontinuum-0.1/discontinuum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 14:18:09.000000 discontinuum-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:18:15.495016 discontinuum-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.793535 discontinuum-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.781535 discontinuum-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.785535 discontinuum-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-24 15:31:17.000000 discontinuum-0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-24 15:31:17.000000 discontinuum-0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-24 15:31:17.000000 discontinuum-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-24 15:31:17.000000 discontinuum-0.2/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-24 15:31:17.000000 discontinuum-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 15:31:17.000000 discontinuum-0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-24 15:31:22.793535 discontinuum-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-24 15:31:17.000000 discontinuum-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.781535 discontinuum-0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.785535 discontinuum-0.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    88360 2024-05-24 15:31:17.000000 discontinuum-0.2/docs/assets/illinois-river-nitrate.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.785535 discontinuum-0.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   377933 2024-05-24 15:31:17.000000 discontinuum-0.2/notebooks/!best-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   152795 2024-05-24 15:31:17.000000 discontinuum-0.2/notebooks/loadest-gp-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-24 15:31:17.000000 discontinuum-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:31:22.793535 discontinuum-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.785535 discontinuum-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.789535 discontinuum-0.2/src/discontinuum/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-24 15:31:22.000000 discontinuum-0.2/src/discontinuum/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.789535 discontinuum-0.2/src/discontinuum/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/engines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/engines/pymc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.789535 discontinuum-0.2/src/discontinuum/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/providers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.789535 discontinuum-0.2/src/discontinuum/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-24 15:31:17.000000 discontinuum-0.2/src/discontinuum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.789535 discontinuum-0.2/src/discontinuum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-24 15:31:22.000000 discontinuum-0.2/src/discontinuum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-24 15:31:22.000000 discontinuum-0.2/src/discontinuum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:31:22.000000 discontinuum-0.2/src/discontinuum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-24 15:31:22.000000 discontinuum-0.2/src/discontinuum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 15:31:22.000000 discontinuum-0.2/src/discontinuum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.789535 discontinuum-0.2/src/loadest_gp/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 15:31:17.000000 discontinuum-0.2/src/loadest_gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-24 15:31:17.000000 discontinuum-0.2/src/loadest_gp/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-24 15:31:17.000000 discontinuum-0.2/src/loadest_gp/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:22.789535 discontinuum-0.2/src/loadest_gp/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:31:17.000000 discontinuum-0.2/src/loadest_gp/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-24 15:31:17.000000 discontinuum-0.2/src/loadest_gp/providers/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-24 15:31:17.000000 discontinuum-0.2/src/loadest_gp/utils.py
```

### Comparing `discontinuum-0.1/.github/workflows/python-package.yml` & `discontinuum-0.2/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest
+        python -m pip install -e .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
```

### Comparing `discontinuum-0.1/.github/workflows/python-publish.yml` & `discontinuum-0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `discontinuum-0.1/.gitignore` & `discontinuum-0.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 var/
 wheels/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+_version.py
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `discontinuum-0.1/DISCLAIMER.md` & `discontinuum-0.2/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `discontinuum-0.1/LICENSE` & `discontinuum-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discontinuum-0.1/LICENSE.md` & `discontinuum-0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `discontinuum-0.1/discontinuum/providers/base.py` & `discontinuum-0.2/src/discontinuum/providers/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,36 @@
+"""
+"""
 from __future__ import annotations
-from typing import TYPE_CHECKING
-
 
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    # from pandas import DataFrame
-    from xarray import DataArray, DataSet
-    from typing import Optional, List, Union, Dict
+    from xarray import Dataset
 
 
 @dataclass
-class Parameter:
-    standard_name: str
-    units: str
-
-
-@dataclass
-class Location:
+class MetaData:
     id: str
     name: str
     latitude: float
     longitude: float
 
 
-def get_daily(
-    site: str, start_date: str, end_date: str, params: list[Parameter]
-) -> DataSet:
-    """Return timeseries of daily data for monitoring site."""
-    raise NotImplementedError
-
-
-def get_location(site: str) -> Location:
-    """Return metadata for monitoring site."""
+def get_covariates(
+        location: str, start_date: str, end_date: str, variable: str,
+        ) -> Dataset:
+    """Return timeseries of covariate data."""
     raise NotImplementedError
 
 
-def get_parameters() -> Parameter:
-    """Return timeseries of paramete"""
+def get_target(
+        location: str, start_date: str, end_date: str, variabe: str
+        ) -> Dataset:
+    """Return target data."""
     raise NotImplementedError
 
 
-def get_samples(site: str, start_date: str, end_date: str, param: Parameter) -> DataSet:
-    """Return sample data for monitoring site."""
+def get_metadata(location: str) -> MetaData:
+    """Return metadata."""
     raise NotImplementedError
```

### Comparing `discontinuum-0.1/discontinuum/providers/usgs.py` & `discontinuum-0.2/src/loadest_gp/providers/usgs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Helper functions for pulling USGS data."""
 
 from __future__ import annotations
-from typing import TYPE_CHECKING
-
-import xarray as xr
 
+import warnings
 from dataclasses import dataclass
-from dataretrieval import nwis
+from typing import TYPE_CHECKING
 
-from discontinuum.providers.base import Location
+import pandas as pd
+import xarray as xr
+from dataretrieval import nwis, wqp
+from discontinuum.providers.base import MetaData
 
 if TYPE_CHECKING:
     # from pandas import DataFrame
-    from xarray import DataArray, Dataset
-    from typing import Optional, List, Union, Dict
+    from typing import Dict, List, Optional, Union
+
+    from xarray import Dataset
 
 CFS_TO_M3 = 0.0283168
 
 
 @dataclass
 class USGSParameter:
     pcode: str
@@ -42,15 +44,16 @@
         """
         return self.standard_name
 
 
 USGSFlow = USGSParameter(
     pcode="00060",
     standard_name="flow",
-    units="m^3/s",
+    long_name="Streamflow",
+    units="cubic meters per second",
     suffix="_Mean",
     conversion=0.0283168,
 )
 
 
 # better to use a dictionary here where the key becomes the name of the parameter
 def get_parameters(pcodes: Dict[str, str]) -> Union[USGSParameter, List[USGSParameter]]:
@@ -85,41 +88,44 @@
 
     if len(params) == 1:
         params = params[0]
 
     return params
 
 
-def get_location(site: str) -> Location:
-    """Get site information from the USGS NWIS API.
+def get_metadata(site: str) -> MetaData:
+    """Get site metadata from the USGS NWIS API.
 
     Parameters
     ----------
     site : str
         USGS site number.
 
     Returns
     -------
     pandas.DataFrame
         Dataframe with the site information.
     """
     df, _ = nwis.get_info(sites=site)
     row = df.iloc[0]
 
-    return Location(
+    return MetaData(
         id=row["site_no"],
         name=row["station_nm"],
         latitude=row["dec_lat_va"],
         longitude=row["dec_long_va"],
     )
 
 
 # TODO pass a dict not a list of params
 def get_daily(
-    site: str, start_date: str, end_date: str, params: List[USGSParameter] = [USGSFlow]
+    site: str,
+    start_date: str,
+    end_date: str,
+    params: Union[List[USGSParameter], USGSParameter] = USGSFlow,
 ) -> Dataset:
     """Get daily data from the USGS NWIS API.
 
     Parameters
     ----------
     site : str
         USGS site number.
@@ -131,14 +137,17 @@
         List of parameters to retrieve. The default is flow only `[USGSFlow]`.
 
     Returns
     -------
     Dataset
         Dataset with the requested data.
     """
+    if not isinstance(params, list):
+        params = [params]
+
     pcodes = [param.pcode for param in params]
 
     df, _ = nwis.get_dv(sites=site, start=start_date, end=end_date, parameterCd=pcodes)
 
     # rename columns
     df = df.rename(columns={param.pcode + param.suffix: param.name for param in params})
     # drop columns
@@ -148,29 +157,144 @@
 
     ds = xr.Dataset.from_dataframe(df)
     # rename "datetime" to "time", which is xarray convention
     ds = ds.rename({"datetime": "time"})
     # ds["date"] = ds["date"].dt.date
 
     # set metadata
-    ds.attrs = get_location(site).__dict__
+    ds.attrs = get_metadata(site).__dict__
 
     for param in params:
         ds[param.name] = ds[param.name] * param.conversion
         # xarray metadata assignment must come after all other operations
         ds[param.name].attrs = param.__dict__
 
     return ds
 
 
+def format_wqp_date(date: str) -> str:
+    """Reformat date from 'YYYY-MM-DD' to 'MM-DD-YYYY'."""
+    return "-".join(date.split("-")[1:] + [date.split("-")[0]])
+
+
 def get_samples(
+        site: str,
+        start_date: str,
+        end_date: str,
+        characteristic: str,
+        fraction: str,
+        provider: str = "NWIS",
+        name: str = "concentration",
+        filter_pcodes: Optional[List[str]] = None,
+):
+    """Get sample data from the Water Quality Portal API.
+
+    Parameters
+    ----------
+    site : str
+        Water Quality Portal site id; e.g., 'USGS-12345678'.
+    start_date : str
+        Start date in the format 'YYYY-MM-DD'.
+    end_date : str
+        End date in the format 'YYYY-MM-DD'.
+    characteristic : str
+        The name of the parameter to retrieve.
+    fraction : str
+        The fraction of the parameter to retrieve. Options are 'Total',
+        'Dissolved', 'Suspended'.
+    provider : str
+        The data provider. Options are 'NWIS' or 'STORET'.
+    name : str
+        Short name for the parameter. Default is 'concentration'.
+    """
+    if fraction and fraction not in ["Total", "Dissolved", "Suspended"]:
+        raise ValueError("Fraction must be 'Total', 'Dissolved', 'Suspended'")
+
+    if provider not in ["NWIS", "STORET"]:
+        raise ValueError("Provider must be 'NWIS' or 'STORET'")
+
+    if provider == "NWIS" and not site.startswith("USGS-"):
+        site = "USGS-" + site
+
+    # reformat dates from 'YYYY-MM-DD' to 'MM-DD-YYYY'
+    start_date = format_wqp_date(start_date)
+    end_date = format_wqp_date(end_date)
+
+    df, _ = wqp.get_results(
+        siteid=site,
+        startDateLo=start_date,
+        startDateHi=end_date,
+        characteristicName=characteristic,
+        provider=provider,
+    )
+
+    # filter by fraction
+    if fraction:
+        df = df[df["ResultSampleFractionText"] == fraction]
+
+    # create datetime index
+    df.index = pd.to_datetime(
+        df["ActivityStartDate"] + " " + df["ActivityStartTime/Time"]
+    )
+
+    df[name] = df["ResultMeasureValue"].astype(float)
+    df.index.name = "time"
+    df.index = df.index.tz_localize(None)
+
+    if provider == "NWIS":
+        # add parameter metadata
+        if not filter_pcodes and len(set(df["USGSPCode"])) != 1:
+            # TODO print the pcodes
+            raise ValueError("Multiple parameters returned from NWIS.")
+
+        elif filter_pcodes:
+            # filter df by list of pcodes
+            df = df[df["USGSPCode"].isin(filter_pcodes)]
+
+    # create xarray dataset and remove unnecessary columns
+    # TODO include censoring flag
+    ds = xr.Dataset.from_dataframe(df[[name]])
+
+    # drop censored values and warn user
+    if any(ds[name].isnull()):
+        ds = ds.dropna(dim="time")
+        warnings.warn(
+            "Censored values have been removed from the dataset.",
+            stacklevel=1,
+            )
+
+    if provider == "NWIS":
+        # strip the "USGS-" prefix from the site number
+        site_id = site[5:]
+        ds.attrs = get_metadata(site_id).__dict__
+
+        if filter_pcodes:
+            pcode = filter_pcodes[0]
+
+        else:
+            pcode = df["USGSPCode"].iloc[0]
+
+        pcode = str(pcode).zfill(5)
+
+        attrs = get_parameters({name: pcode})
+        ds[name].attrs = attrs.__dict__
+
+    if provider == "STORET":
+        pass
+
+    return ds
+
+
+def get_qwdata_samples(
     site: str, start_date: str, end_date: str, pcode: str, name: str = "concentration"
 ) -> Dataset:
     """Get sample data from the USGS NWIS API.
 
+    Warning: The QWData service is deprecated and no longer receives data.
+
     Parameters
     ----------
     site : str
         USGS site number.
     start_date : str
         Start date in the format 'yyyy-mm-dd'.
     end_date : str
@@ -188,26 +312,26 @@
     df, _ = nwis.get_qwdata(
         sites=site, start=start_date, end=end_date, parameterCd=pcode
     )
     attrs = get_parameters({name: pcode})
     ppcode = "p" + pcode
 
     # check if data are strings
-    if df[ppcode].dtype == 'O':
+    if df[ppcode].dtype == "O":
         # remove "<" and ">" from values and convert to float
         # TODO handle censoring
-        df[ppcode] = df[ppcode].str.extract('(\d+.\d+)', expand=False).astype(float)
+        df[ppcode] = df[ppcode].str.extract(r"(\d+.\d+)", expand=False).astype(float)
 
     df = df.rename(columns={ppcode: name})
 
     df = df[[name]]
     # remove timezone for xarray compatibility
     df.index = df.index.tz_localize(None)
 
     ds = xr.Dataset.from_dataframe(df)
     # rename "datetime" to "time", which is xarray convention
     ds = ds.rename({"datetime": "time"})
 
-    ds.attrs = get_location(site).__dict__
+    ds.attrs = get_metadata(site).__dict__
     ds[name].attrs = attrs.__dict__
 
     return ds
```

### Comparing `discontinuum-0.1/pyproject.toml` & `discontinuum-0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -14,43 +14,60 @@
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 
 dependencies = [
     "pymc >= 5.0.0",
+    "scikit-learn",
     "xarray",
 ]
 
 dynamic = ["version"]
 
 [tool.setuptools]
-packages = ["discontinuum","discontinuum.providers","discontinuum.models", "discontinuum.tests"]
+package-dir = {"" = "src"}
+# packages = ["discontinuum","discontinuum.providers","discontinuum.models", "discontinuum.tests"]
 
 [project.optional-dependencies]
-test = [
+dev = [
   "flake8",
   "ruff",
   "pytest > 5.0.0",
   "pytest-cov[all]",
 ]
 
-provider_usgs = [
+loadest_gp = [
   "dataretrieval",
 ]
 
+doc = [
+  "sphinx",
+  "sphinx-rtd-theme",
+  "nbsphinx",
+  "ipython",
+  "ipykernel",
+]
+
 [project.urls]
 homepage = "https://github.com/thodson-usgs/discontinuum"
 repository = "https://github.com/thodson-usgs/discontinuum.git"
 
 [tool.setuptools_scm]
-write_to = "discontinuum/_version.py"
+write_to = "src/discontinuum/_version.py"
 
 [tool.ruff]
-# Set the maximum line length to 127 (width of GitHub editor)
-line-length = 127
+line-length = 127 # 79
+
+[tool.ruff.format]
+quote-style = "double"
+docstring-code-format = true
+docstring-code-line-length = 72
 
 [tool.ruff.lint]
-# Add the `line-too-long` rule to the enforced rule set. By default, Ruff omits rules that
-# overlap with the use of a formatter, like Black, but we can override this behavior by
-# explicitly adding the rule.
-extend-select = ["E501"]
+preview = true
+# Default ["E4", "E7", "E9", and "F"] --> Pyflakes ("F") and pycodestyle ("E")
+extend-select = [
+  "B", "I", "Q",
+  "W291", "W292", "W293", "W605",
+  "E231", "E252", "E261", "E262", "E303", "E501",
+]
```

