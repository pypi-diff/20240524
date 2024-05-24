# Comparing `tmp/rsam_ew-1.2.0.tar.gz` & `tmp/rsam_ew-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsam_ew-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rsam_ew-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rsam_ew-1.2.0.tar` & `rsam_ew-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1085 2024-05-08 08:08:12.548040 rsam_ew-1.2.0/LICENSE
--rw-r--r--   0        0        0       47 2024-05-11 08:31:09.928735 rsam_ew-1.2.0/README.md
--rw-r--r--   0        0        0      973 2024-05-18 05:42:15.204296 rsam_ew-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      328 2024-05-13 12:10:52.060571 rsam_ew-1.2.0/src/rsam_ew/__init__.py
--rw-r--r--   0        0        0     7983 2024-05-18 05:47:02.195415 rsam_ew-1.2.0/src/rsam_ew/rsam.py
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 rsam_ew-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-08 08:08:12.548040 rsam_ew-1.3.0/LICENSE
+-rw-r--r--   0        0        0       47 2024-05-11 08:31:09.928735 rsam_ew-1.3.0/README.md
+-rw-r--r--   0        0        0      973 2024-05-24 08:25:09.042319 rsam_ew-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      363 2024-05-24 07:34:11.126167 rsam_ew-1.3.0/src/rsam_ew/__init__.py
+-rw-r--r--   0        0        0    14055 2024-05-13 15:28:42.530201 rsam_ew-1.3.0/src/rsam_ew/magma.py
+-rw-r--r--   0        0        0    10589 2024-05-24 08:23:36.120276 rsam_ew-1.3.0/src/rsam_ew/rsam.py
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 rsam_ew-1.3.0/PKG-INFO
```

### Comparing `rsam_ew-1.2.0/LICENSE` & `rsam_ew-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsam_ew-1.2.0/pyproject.toml` & `rsam_ew-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name =  "rsam-ew"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
     {name = "Martanto", email = "martanto@live.com"},
 ]
 description = "Plot RSAM from earthworm files"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["seismic", "volcano", "seiscomp", "volcanology", "seismology", "magma indonesia"]
```

### Comparing `rsam_ew-1.2.0/src/rsam_ew/rsam.py` & `rsam_ew-1.3.0/src/rsam_ew/rsam.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from .magma import Plot, colors
 from datetime import datetime
 from zipfile import ZipFile, ZipInfo
 from typing import Tuple
 from pathlib import Path
 from pandas import DatetimeIndex
 
 import pandas as pd
 import os
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
+import matplotlib.ticker as mticker
 
 month_translator = {
     'Mei': 'May',
     'Agu': 'Aug',
     'Okt': 'Oct',
     'Des': 'Dec',
 }
@@ -173,53 +175,112 @@
         save_path = os.path.join(self.rsam_dir, f'rsam_{start_date}_{end_date}.csv')
         df.to_csv(save_path)
 
         print(f'✅ RSAM file saved at {save_path}')
         return df
 
     def plot_ax(self, ax: plt.Axes, df: pd.DataFrame, smoothing: str = '1d', interval_day: int = 1,
-                y_min: float = 0, y_max: float = None) -> plt.Axes:
+                y_min: float = 0, y_max: float = None, show_gridline: bool = True) -> plt.Axes:
+
+        if y_max is None:
+            y_max = df['value'].max()
 
         ax.scatter(df.index, df['value'], c='k', alpha=0.3, s=10, label='10 minutes')
         ax.plot(df.index, df[smoothing], c='red', label=smoothing, alpha=1)
 
         ax.set_xlabel('Datetime', fontsize=12)
         ax.xaxis.set_major_locator(mdates.DayLocator(interval=interval_day))
         ax.xaxis.set_major_formatter(mdates.DateFormatter('%Y-%m-%d'))
         ax.set_ylim(y_min, y_max)
         ax.set_xlim(df.first_valid_index(), df.last_valid_index())
         ax.legend(loc='upper right', fontsize='8', ncol=4)
 
+        if show_gridline is True:
+            ax.grid(visible=True, axis='x')
+
         return ax
 
     def plot(self, start_date: str, end_date: str, title: str = None, smoothing: str = '1d', width: int = 12,
              height: int = 9, interval_day: int = 1, y_min: float = 0, y_max: float = None, show_gridline: bool = True,
              save: bool = True):
         dates: DatetimeIndex = pd.date_range(start_date, end_date, freq="D")
 
         df = self.get_df(dates)
         df[smoothing] = df['value'].rolling(smoothing, center=True).median()
 
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(width, height),
                                layout="constrained", sharex=True)
 
-        if y_max is None:
-            y_max = df['value'].max()
-
         if title is None:
             title = f'RSAM {self.nslc}'
 
         ax = self.plot_ax(ax, df=df, smoothing=smoothing, interval_day=interval_day,
-                          y_min=y_min, y_max=y_max)
+                          y_min=y_min, y_max=y_max, show_gridline=show_gridline)
 
         ax.set_title('{} \n Periode {} - {}'.format(title, start_date, end_date), fontsize=14)
 
         plt.xticks(rotation=45)
-        if show_gridline is True:
-            plt.grid(visible=True, which='both')
 
         if save:
             save_path = os.path.join(self.figures_dir, f'rsam_{self.nslc}_{start_date}_{end_date}_{smoothing}.png')
             fig.savefig(save_path, dpi=300)
             print(f'📈 RSAM Graphics saved to {save_path}')
 
         return fig
+
+    def plot_with_magma(self, token: str, volcano_code: str,  start_date: str, end_date: str,
+                        smoothing: str = '1d', interval: int = 1, earthquake_events: str | list[str] = None,
+                        width: int = 12, height: int = None, height_per_eq: int = 2, y_min: float = 0, y_max: float = None,
+                        show_gridline: bool = True, height_ratios=None):
+
+        if height_ratios is None:
+            height_ratios = [1, 0.2]
+
+        magma_plot = Plot(
+            token=token,
+            volcano_code=volcano_code,
+            start_date=start_date,
+            end_date=end_date,
+            earthquake_events=earthquake_events,
+        )
+
+        df = magma_plot.df
+
+        if height is None:
+            height = df.columns.size + 1
+
+        fig = plt.figure(figsize=(width, height), dpi=100)
+
+        (fig_magma, fig_rsam) = fig.subfigures(nrows=2, ncols=1, height_ratios=height_ratios)
+
+        fig_magma.subplots_adjust(hspace=0.0)
+        fig_magma.supylabel('Jumlah')
+        axs_magma = fig_magma.subplots(nrows=len(df.columns), ncols=1, sharex=True)
+        for gempa, column_name in enumerate(df.columns):
+            axs_magma[gempa].bar(df.index, df[column_name], width=0.5, label=column_name,
+                                 color=colors[column_name], linewidth=0)
+            axs_magma[gempa].set_ylim([0, df[column_name].max() * 1.2])
+
+            axs_magma[gempa].legend(loc=2)
+            axs_magma[gempa].tick_params(labelbottom=False)
+            # axs_magma[gempa].yaxis.set_major_locator(mticker.MultipleLocator(1))
+            axs_magma[gempa].yaxis.get_major_ticks()[0].label1.set_visible(False)
+
+        dates: DatetimeIndex = pd.date_range(start_date, end_date, freq="D")
+
+        df = self.get_df(dates)
+
+        df[smoothing] = df['value'].rolling(smoothing, center=True).median()
+
+        ax_rsam = fig_rsam.subplots(nrows=1, ncols=1)
+        self.plot_ax(ax_rsam, df=df, smoothing=smoothing, interval_day=interval,
+                          y_min=y_min, y_max=y_max, show_gridline=show_gridline)
+
+        plt.tight_layout()
+        plt.tick_params(axis='both', which='major', labelsize=10)
+        plt.xticks(rotation=60)
+
+        save_path = os.path.join(self.figures_dir, f'rsam_magma_{start_date}_{end_date}_{smoothing}.png')
+        fig.savefig(save_path, dpi=300)
+        print(f'📈 Graphics saved to {save_path}')
+
+        plt.show()
```

### Comparing `rsam_ew-1.2.0/PKG-INFO` & `rsam_ew-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsam-ew
-Version: 1.2.0
+Version: 1.3.0
 Summary: Plot RSAM from earthworm files
 Keywords: seismic,volcano,seiscomp,volcanology,seismology,magma indonesia
 Author-email: Martanto <martanto@live.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

