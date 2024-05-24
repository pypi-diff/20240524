# Comparing `tmp/mptradelib-0.5.5.tar.gz` & `tmp/mptradelib-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.5.5.tar", max compression
+gzip compressed data, was "mptradelib-0.5.6.tar", max compression
```

## Comparing `mptradelib-0.5.5.tar` & `mptradelib-0.5.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.5/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.5/mptradelib/__init__.py
--rw-r--r--   0        0        0     4515 2024-05-21 20:24:35.631241 mptradelib-0.5.5/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.5/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.5/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.5/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.5/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.5/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.5/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.5/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.5/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.5/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.5/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.5/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.5/mptradelib/livetrade.py
--rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.5/mptradelib/optimizers/__init__.py
--rw-r--r--   0        0        0     8133 2024-05-21 12:30:56.533060 mptradelib-0.5.5/mptradelib/optimizers/walkforward.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.5/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.5/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.5/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0     9286 2024-05-21 20:24:00.945335 mptradelib-0.5.5/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.5/mptradelib/utils/utils.py
--rw-r--r--   0        0        0      822 2024-05-21 20:24:58.936129 mptradelib-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.6/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4515 2024-05-21 20:24:35.631241 mptradelib-0.5.6/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.6/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.6/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.6/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.6/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.6/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.6/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.6/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.6/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.6/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.6/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.6/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.6/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.6/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     8569 2024-05-23 19:20:16.364263 mptradelib-0.5.6/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.6/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.6/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.6/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0    10302 2024-05-23 19:18:54.556637 mptradelib-0.5.6/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.6/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:19:31.018101 mptradelib-0.5.6/mptradelib/widgets/__init__.py
+-rw-r--r--   0        0        0     2005 2024-05-23 19:19:52.537757 mptradelib-0.5.6/mptradelib/widgets/daterangepicker.py
+-rw-r--r--   0        0        0      822 2024-05-23 19:19:57.219043 mptradelib-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.6/PKG-INFO
```

### Comparing `mptradelib-0.5.5/README.md` & `mptradelib-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/backtest.py` & `mptradelib-0.5.6/mptradelib/backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/broker/broker.py` & `mptradelib-0.5.6/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/broker/session.py` & `mptradelib-0.5.6/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/broker/shoonya.py` & `mptradelib-0.5.6/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/broker/ticker.py` & `mptradelib-0.5.6/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/cli/new.py` & `mptradelib-0.5.6/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.5.6/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.5.6/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.5.6/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/feed.py` & `mptradelib-0.5.6/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/livetrade.py` & `mptradelib-0.5.6/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/optimizers/walkforward.py` & `mptradelib-0.5.6/mptradelib/optimizers/walkforward.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 import pandas as pd
 from mptradelib.backtest import Backtest
 from typing import Callable, List, Dict
 from tqdm import tqdm
 import numpy as np
 import plotly.graph_objects as go
 
+class StrategyFuncs(pyd.BaseModel):
+    model_config = pyd.ConfigDict(arbitrary_types_allowed=True)
+
+    compute: Callable[[pd.DataFrame, dict], pd.DataFrame]
+    exit_func: Callable[[pd.DataFrame, dict], None] = None
+
 class Stage(pyd.BaseModel):
     model_config = pyd.ConfigDict(arbitrary_types_allowed=True)
 
     main_df: pd.DataFrame = pyd.Field(..., alias='df')
     stage_no: int
     stage_size: int
     test_fraction: float = 0.25
@@ -34,32 +40,32 @@
     @property
     def opt_result(self):
         return self._opt_result
     
     def _get_test_size(self):
         return int(self.stage_size * self.test_fraction)
 
-    def optimize(self, compute, **params: dict):
-        b = Backtest(self.opt_df, compute=compute)
+    def optimize(self, strategy_funcs: StrategyFuncs, **params: dict):
+        b = Backtest(self.opt_df, compute=strategy_funcs.compute, exit_func=strategy_funcs.exit_func)
         self._opt_result = b.optimize(params)
         return self
 
-    def validate(self, compute, **kwargs):
-        b = Backtest(self.test_df, compute=compute)
+    def validate(self, strategy_funcs: StrategyFuncs, **kwargs):
+        b = Backtest(self.test_df, compute=strategy_funcs.compute, exit_func=strategy_funcs.exit_func)
         trades, _ = b.run(**kwargs)
         return trades
 
 
 class Walkforward(pyd.BaseModel):
     model_config = pyd.ConfigDict(arbitrary_types_allowed=True)
 
     df: pd.DataFrame
     stage_count: int = 6
     test_fraction: float = 0.25
-    strategy: Callable[[pd.DataFrame, dict],pd.DataFrame]
+    strategy_funcs: StrategyFuncs
     stages: List[Stage] = []
 
     def _create_stages(self) -> List[Stage]:
         stage_size = int(len(self.df)/(1 + (self.stage_count-1) * self.test_fraction))
         stages = []
         for i in range(self.stage_count):
             stage = Stage(df=self.df, stage_no=i, stage_size=stage_size, test_fraction=self.test_fraction)
@@ -69,34 +75,34 @@
     def optimize(self, **params: dict):
         show_progressbar = params.pop('show_progressbar', True)
 
         stages: Stage = self._create_stages()
         if show_progressbar:
             with tqdm(total=len(stages)) as pb:
                 for stage in stages:
-                    s = stage.optimize(self.strategy, **params)
+                    s = stage.optimize(self.strategy_funcs, **params)
                     self.stages.append(s)
                     pb.update()
         else:
             for stage in stages:
-                stage.optimize(self.strategy, **params)
+                stage.optimize(self.strategy_funcs, **params)
                 self.stages.append(stage)
         return self
     
     @property
     def opt_result(self):
         return [s.opt_result for s in self.stages]
 
     def _get_date(self, d, index):
         return d.datetime.iloc[index].strftime("%Y-%m-%d")
     
-    def validate(self, compute, params):
+    def validate(self, strategy_func, params):
         results = []
         for i in range(len(self.stages)):
-            r = self.stages[i].validate(compute, **params[i])
+            r = self.stages[i].validate(strategy_func, **params[i])
             results.append(r)
         return pd.concat(results)
 
     def plot_splits(self):
         stages = self._create_stages()
         fig = go.Figure()
         for i in range(len(stages)):
@@ -129,26 +135,26 @@
 
 class MultiSymbolWalkforwardAnalysis(pyd.BaseModel):
     model_config = pyd.ConfigDict(arbitrary_types_allowed=True)
 
     dfs: Dict[str, pd.DataFrame]
     stage_count: int = 6
     test_fraction: float = 0.25
-    strategy: Callable[[pd.DataFrame, dict],pd.DataFrame]
+    strategy_funcs: StrategyFuncs
     walkforwards: Dict[str, Walkforward] = {}
     __computed_result = None
 
     def optimize(self, **params: dict):
         with tqdm(total=len(self.dfs)) as pb:
             for k, df in self.dfs.items():
                 w = Walkforward(
                     df=df, 
                     stage_count=self.stage_count, 
                     test_fraction=self.test_fraction, 
-                    strategy=self.strategy
+                    strategy_funcs=self.strategy_funcs
                 )
                 w.optimize(**params)
                 pb.update()
                 self.walkforwards[k] = w
         return self
     
     @property
@@ -185,14 +191,16 @@
     def create_pre_pivot_dfs(self, param_cols: tuple):
         final_result = []
         results_agg = []
         default_cols = ['profit', 'trades', 'profit_perc']
         cols = param_cols + default_cols
         for i in range(len(list(self.walkforwards.values())[0].stages)):
             for stage in self.transform_to_agg_stages()[i]:
+                if stage['trades'].empty:
+                    continue
                 row = [stage['params'][p] for p in param_cols]
                 row.append(round(stage['trades'].profit.sum(), 2))
                 row.append(stage['trades'])
                 row.append(self.profit_perc_sum(stage['trades']))
                 results_agg.append(row)
             final_result.append(pd.DataFrame(results_agg, columns=cols))
         return final_result
@@ -202,17 +210,17 @@
         ppdf = self.create_pre_pivot_dfs(cols)
         for d in ppdf:
             profit_perc = d.pivot_table(values='profit_perc', index=[cols[0]], columns=[cols[1]])
             p = self._find_optimal_param_for_test(profit_perc)
             extracted_params.append(dict(zip(cols, p)))
         return extracted_params
     
-    def validate(self, sym, compute, params):
+    def validate(self, sym, strategy_func, params):
         w = self.walkforwards[sym]
-        return w.validate(compute, params)
+        return w.validate(strategy_func, params)
         
     def _find_optimal_param_for_test(self, d):        
         sample = d.copy()
         sample['mean'] = sample.mean(axis=1)
         sample['sdv'] = sample.std(axis=1)
         scoredf = sample
```

### Comparing `mptradelib-0.5.5/mptradelib/test_renko.py` & `mptradelib-0.5.6/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/utils/simulated_trades.py` & `mptradelib-0.5.6/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/mptradelib/utils/tearsheet.py` & `mptradelib-0.5.6/mptradelib/utils/tearsheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import pandas as pd
 import numpy as np
 from .simulated_trades import SimulateTrades
 import pydantic as pyd
 from typing import List
+import datetime as dt
 try:
     from plotly.subplots import make_subplots
     import plotly.graph_objects as go
     import plotly.express as px
 except ImportError:
     print("please install plotly by 'pip install plotly' to enable plotting")
 
 class Line(pyd.BaseModel):
     colname: str
     name: str = None
     overlay: bool = True
 
 class Tearsheet:
+    chart_fig: go.Figure = None
+
     def __init__(self, result: pd.DataFrame, seed=10000, leverage=1) -> None:
         self.df = result
         self._seed = seed
         self._leverage = leverage
 
     def profit_factor(self):
         r = self.df[self.df.profit > 0].profit.sum()/abs(self.df[self.df.profit < 0].profit.sum())
@@ -38,22 +41,26 @@
         )
     
     def win_rate(self):
         r = self.win_vs_loss()
         return round(r[0]/sum(r) * 100, 2)
     
     def drawdown(self):
+        if self.df.empty:
+            return None, None
         cum_profit = self.df.profit.cumsum()
         curr_max = cum_profit.expanding().max()
         dd = cum_profit - curr_max
         perc = dd/curr_max * 100
         return dd, perc
 
     def max_drawdown(self):
         dd, ddp = self.drawdown()
+        if dd is None:
+            return 0, 0
         return round(dd.min(), 2), round(ddp.min(), 2)
     
     def sharpe_ratio(self):
         n = len(self.df.profit)
         return round(np.sqrt(n) * np.mean(self.df.profit)/np.std(self.df.profit), 2)
     
     def avg_profit(self):
@@ -208,29 +215,30 @@
             y=dd,
             fill="tozeroy",
             fillcolor="rgba(228,128,68,120)",
             line={'color': 'rgba(228,128,68,120)'},
         )
         fig.add_trace(drawdowns, row=1, col=1)
 
-
-    def plot_chart(self, name, df, trades, lines: List[Line], jupyter=False):
+    def plot_chart(self, name, df, trades, 
+                   from_date = dt.datetime.now().date(), 
+                   to_date = dt.datetime.now().date() + dt.timedelta(days=1),
+                   lines: List[Line] = [], jupyter=False):
         row_count = 1 + len([l for l in lines if not l.overlay])
-        last_date = df.iloc[len(df) - 1].datetime.date()
-        filtered_df = df[df.datetime.dt.date == last_date]
-        filtered_trades = trades[trades.entry_time.dt.date == last_date]
+        filtered_df = df[(df.datetime.dt.date >= from_date) & (df.datetime.dt.date < to_date)]
+        filtered_trades = trades[(trades.entry_time.dt.date >= from_date) & (trades.entry_time.dt.date >= to_date)]
 
         cs_chart = go.Candlestick(
             x=filtered_df.datetime,
             open=filtered_df.open,
             high=filtered_df.high,
             low=filtered_df.low,
             close=filtered_df.close,
             showlegend=False,
-            name=name
+            name=name,
         )
 
         main_trace = [cs_chart]
         non_overlay_traces = []
         for l in lines:
             trace = go.Scatter(
                 x=filtered_df.datetime,
@@ -239,48 +247,64 @@
             )
             
             if l.overlay:
                 main_trace.append(trace)
             else:
                 non_overlay_traces.append(trace)
 
+        row_height = round(1/(len(non_overlay_traces) + 4), 1)
+        row_heights = [ row_height for _ in range(len(non_overlay_traces) + 1)]
+        row_heights[0] = 4 * row_height
         
-        fig = make_subplots(
-            rows=len(non_overlay_traces) + 1, 
-            cols=1, 
-            subplot_titles=tuple([name] + [t.name for t in non_overlay_traces]),
-        )
+        if self.chart_fig is None:
+            self.chart_fig = make_subplots(
+                rows=len(non_overlay_traces) + 1, 
+                cols=1, 
+                subplot_titles=tuple([name] + [t.name for t in non_overlay_traces]),
+                row_heights=row_heights,
+                vertical_spacing=0.02,
+                shared_xaxes=True,
+            )
+        else:
+            self.chart_fig.data = []
 
         for t in main_trace:
-            fig.add_trace(t, row=1, col=1)
+            self.chart_fig.add_trace(t, row=1, col=1)
 
         for i in range(len(non_overlay_traces)):
-            fig.add_trace(non_overlay_traces[i], row=2+i, col=1)
+            self.chart_fig.add_trace(non_overlay_traces[i], row=2+i, col=1)
 
         for row in filtered_trades.itertuples():
-            fig.add_annotation(x=row.entry_time, y=row.entry_price,
+            self.chart_fig.add_annotation(x=row.entry_time, y=row.entry_price,
                 text= "LE" if row.direction > 0 else "SE",
                 showarrow=True,
                 arrowhead=1,
                 bgcolor="#ff7f0e",
             )
-            fig.add_annotation(x=row.exit_time, y=row.exit_price,
+            self.chart_fig.add_annotation(x=row.exit_time, y=row.exit_price,
                 text= "LEx" if row.direction > 0 else "SEx",
                 showarrow=True,
                 arrowhead=1,
                 bgcolor="#ff7f0e",
             )
 
-        fig.update_layout(
+        self.chart_fig.update_layout(
             hoversubplots="axis",
             hovermode="x unified",
             grid=dict(rows=row_count, columns=1),
             autosize=True,
             margin=dict(l=30, r=30, t=40, b=30),
+            height=800,
+            legend=dict(
+                orientation="h",
+                yanchor="bottom",
+                y=1.02,
+                xanchor="right",
+                x=1
+            )
         )
 
-        fig.update_xaxes(
+        self.chart_fig.update_xaxes(
             rangeslider_visible=False,
         )
 
-        if jupyter:
-            return fig
+        return self.chart_fig
```

### Comparing `mptradelib-0.5.5/mptradelib/utils/utils.py` & `mptradelib-0.5.6/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.5/pyproject.toml` & `mptradelib-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.5.5"
+version = "0.5.6"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.5.5/PKG-INFO` & `mptradelib-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.5.5
+Version: 0.5.6
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

