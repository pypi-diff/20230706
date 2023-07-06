# Comparing `tmp/fairbench-0.2.7-py3-none-any.whl.zip` & `tmp/fairbench-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,43 +1,49 @@
-Zip file size: 31708 bytes, number of entries: 41
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-17 09:11 fairbench/__init__.py
+Zip file size: 37696 bytes, number of entries: 47
+-rw-rw-rw-  2.0 fat      411 b- defN 23-Jun-23 14:12 fairbench/__init__.py
 -rw-rw-rw-  2.0 fat     1952 b- defN 23-Jun-01 09:25 fairbench/export.py
+-rw-rw-rw-  2.0 fat     5762 b- defN 23-Jun-28 17:37 fairbench/stamps.py
 -rw-rw-rw-  2.0 fat       38 b- defN 23-Jun-14 13:57 fairbench/bench/__init__.py
 -rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-15 21:51 fairbench/bench/demos.py
 -rw-rw-rw-  2.0 fat     1660 b- defN 23-Jun-15 09:42 fairbench/bench/loader.py
--rw-rw-rw-  2.0 fat       93 b- defN 23-Jun-17 19:28 fairbench/export/__init__.py
--rw-rw-rw-  2.0 fat    13283 b- defN 23-Jun-23 07:56 fairbench/export/interactive.py
+-rw-rw-rw-  2.0 fat      134 b- defN 23-Jun-28 12:59 fairbench/export/__init__.py
+-rw-rw-rw-  2.0 fat    16295 b- defN 23-Jul-05 08:03 fairbench/export/interactive.py
 -rw-rw-rw-  2.0 fat     2912 b- defN 23-Jun-16 09:23 fairbench/export/native.py
+-rw-rw-rw-  2.0 fat      173 b- defN 23-Jun-28 12:05 fairbench/export/modelcards/__init__.py
+-rw-rw-rw-  2.0 fat     2856 b- defN 23-Jun-28 13:13 fairbench/export/modelcards/tohtml.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-Jun-28 13:12 fairbench/export/modelcards/tomarkdown.py
+-rw-rw-rw-  2.0 fat      562 b- defN 23-Jun-28 12:59 fairbench/export/modelcards/toyaml.py
 -rw-rw-rw-  2.0 fat      122 b- defN 23-May-13 22:58 fairbench/forks/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-May-25 07:44 fairbench/forks/categorical.py
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-16 09:22 fairbench/forks/explanation.py
--rw-rw-rw-  2.0 fat    26645 b- defN 23-Jun-20 14:13 fairbench/forks/fork.py
+-rw-rw-rw-  2.0 fat     2936 b- defN 23-Jun-28 12:59 fairbench/forks/explanation.py
+-rw-rw-rw-  2.0 fat    26874 b- defN 23-Jun-28 12:59 fairbench/forks/fork.py
 -rw-rw-rw-  2.0 fat      239 b- defN 23-Jun-20 08:51 fairbench/metrics/__init__.py
--rw-rw-rw-  2.0 fat     3777 b- defN 23-Jun-20 08:51 fairbench/metrics/classification.py
+-rw-rw-rw-  2.0 fat     4008 b- defN 23-Jul-06 00:14 fairbench/metrics/classification.py
 -rw-rw-rw-  2.0 fat     2066 b- defN 23-May-31 07:41 fairbench/metrics/disparate_impact.py
 -rw-rw-rw-  2.0 fat     1494 b- defN 23-May-31 07:41 fairbench/metrics/disparate_mistreatment.py
 -rw-rw-rw-  2.0 fat      668 b- defN 23-Jun-20 11:41 fairbench/metrics/ranking.py
--rw-rw-rw-  2.0 fat     2970 b- defN 23-Jun-20 14:07 fairbench/metrics/regression.py
+-rw-rw-rw-  2.0 fat     2970 b- defN 23-Jul-06 06:59 fairbench/metrics/regression.py
 -rw-rw-rw-  2.0 fat      100 b- defN 23-May-31 10:15 fairbench/mitigation/__init__.py
 -rw-rw-rw-  2.0 fat     1790 b- defN 23-May-31 10:16 fairbench/mitigation/postprocessing.py
 -rw-rw-rw-  2.0 fat      207 b- defN 23-Jan-15 14:06 fairbench/reports/__init__.py
 -rw-rw-rw-  2.0 fat     1491 b- defN 23-Jun-07 08:52 fairbench/reports/accumulate.py
--rw-rw-rw-  2.0 fat     2021 b- defN 23-Jun-20 14:07 fairbench/reports/adhoc.py
+-rw-rw-rw-  2.0 fat     2004 b- defN 23-Jun-23 13:28 fairbench/reports/adhoc.py
 -rw-rw-rw-  2.0 fat     2590 b- defN 23-Jun-20 08:05 fairbench/reports/base.py
 -rw-rw-rw-  2.0 fat      883 b- defN 23-May-14 15:09 fairbench/reports/surrogate.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Feb-20 08:42 fairbench/reports/reduction/__init__.py
 -rw-rw-rw-  2.0 fat     2260 b- defN 23-Jun-16 09:23 fairbench/reports/reduction/expanders.py
 -rw-rw-rw-  2.0 fat     2637 b- defN 23-Jun-20 14:07 fairbench/reports/reduction/reduce.py
 -rw-rw-rw-  2.0 fat     2834 b- defN 23-Jun-16 06:45 fairbench/reports/reduction/reducers.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-26 21:15 tests/__init__.py
 -rw-rw-rw-  2.0 fat     1394 b- defN 23-Jun-12 10:06 tests/test_batching.py
 -rw-rw-rw-  2.0 fat     1278 b- defN 23-Jun-01 09:09 tests/test_benchmarks.py
 -rw-rw-rw-  2.0 fat     1103 b- defN 23-Jun-16 09:20 tests/test_demos.py
 -rw-rw-rw-  2.0 fat     5807 b- defN 23-Jun-15 09:42 tests/test_forks.py
 -rw-rw-rw-  2.0 fat     2685 b- defN 23-Jun-20 14:07 tests/test_metrics.py
+-rw-rw-rw-  2.0 fat     1150 b- defN 23-Jun-29 09:15 tests/test_modelcards.py
 -rw-rw-rw-  2.0 fat     1624 b- defN 23-Jun-14 06:40 tests/test_reduction.py
 -rw-rw-rw-  2.0 fat     6556 b- defN 23-May-31 14:04 tests/test_reports.py
--rw-rw-rw-  2.0 fat      830 b- defN 23-Jun-23 09:02 fairbench-0.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-23 09:02 fairbench-0.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-23 09:02 fairbench-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3445 b- defN 23-Jun-23 09:02 fairbench-0.2.7.dist-info/RECORD
-41 files, 106778 bytes uncompressed, 26206 bytes compressed:  75.5%
+-rw-rw-rw-  2.0 fat      852 b- defN 23-Jul-06 18:43 fairbench-0.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 18:43 fairbench-0.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jul-06 18:43 fairbench-0.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3985 b- defN 23-Jul-06 18:43 fairbench-0.2.8.dist-info/RECORD
+47 files, 124519 bytes uncompressed, 31344 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: fairbench/__init__.py
 Comment: 
 
 Filename: fairbench/export.py
 Comment: 
 
+Filename: fairbench/stamps.py
+Comment: 
+
 Filename: fairbench/bench/__init__.py
 Comment: 
 
 Filename: fairbench/bench/demos.py
 Comment: 
 
 Filename: fairbench/bench/loader.py
@@ -18,14 +21,26 @@
 
 Filename: fairbench/export/interactive.py
 Comment: 
 
 Filename: fairbench/export/native.py
 Comment: 
 
+Filename: fairbench/export/modelcards/__init__.py
+Comment: 
+
+Filename: fairbench/export/modelcards/tohtml.py
+Comment: 
+
+Filename: fairbench/export/modelcards/tomarkdown.py
+Comment: 
+
+Filename: fairbench/export/modelcards/toyaml.py
+Comment: 
+
 Filename: fairbench/forks/__init__.py
 Comment: 
 
 Filename: fairbench/forks/categorical.py
 Comment: 
 
 Filename: fairbench/forks/explanation.py
@@ -99,26 +114,29 @@
 
 Filename: tests/test_forks.py
 Comment: 
 
 Filename: tests/test_metrics.py
 Comment: 
 
+Filename: tests/test_modelcards.py
+Comment: 
+
 Filename: tests/test_reduction.py
 Comment: 
 
 Filename: tests/test_reports.py
 Comment: 
 
-Filename: fairbench-0.2.7.dist-info/METADATA
+Filename: fairbench-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: fairbench-0.2.7.dist-info/WHEEL
+Filename: fairbench-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: fairbench-0.2.7.dist-info/top_level.txt
+Filename: fairbench-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: fairbench-0.2.7.dist-info/RECORD
+Filename: fairbench-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fairbench/__init__.py

```diff
@@ -1,2 +1,14 @@
+from fairbench.forks import *
+from fairbench.metrics import *
+from fairbench.reports import *
+from fairbench.export import *
+from fairbench.bench import *
 
-
+from fairbench import forks
+from fairbench import metrics
+from fairbench import reports
+from fairbench import export
+from fairbench import mitigation
+from fairbench import bench
+from fairbench import stamps
+from fairbench.bench import demos
```

## fairbench/export/__init__.py

```diff
@@ -1,2 +1,3 @@
 from fairbench.export.native import *
 from fairbench.export.interactive import interactive
+from fairbench.export import modelcards
```

## fairbench/export/interactive.py

```diff
@@ -1,68 +1,87 @@
 from fairbench.forks.fork import Fork, Forklike
 from fairbench.forks.explanation import tofloat, ExplainableError
 
 
-def clean(fork):
+def _clean(fork):  # pragma: no cover
     if isinstance(fork, Fork):
-        branches = {k: clean(v) for k, v in fork.branches().items()}
+        branches = {k: _clean(v) for k, v in fork.branches().items()}
         branches = {k: v for k, v in branches.items() if v is not None}
         if not branches:
             return None
         return Fork(branches)
     if isinstance(fork, Forklike):
-        branches = {k: clean(v) for k, v in fork.items()}
+        branches = {k: _clean(v) for k, v in fork.items()}
         branches = {k: v for k, v in branches.items() if v is not None}
         if not branches:
             return None
         return Forklike(branches)
     if isinstance(fork, ExplainableError):
         return None
     return fork
 
 
-def _in_ipynb():
+def _in_jupyter():  # pragma: no cover
+    """
+    Checks whether current code runs within a Jupyter notebook.
+    :return: True if within Jupyter, False otherwise
+    """
     try:
         shell = get_ipython().__class__.__name__
         if shell == "ZMQInteractiveShell":
             return True  # Jupyter notebook or qtconsole
         elif shell == "TerminalInteractiveShell":
             return False  # Terminal running IPython
         else:
             return False  # Other type (?)
     except NameError:
         return False  # Probably standard Python interpreter
 
 
-def interactive(report, name="report", width=800):  # pragma: no cover
+def interactive(
+    report, name="report", width=800, height=400, spacing=None, horizontal=True
+):  # pragma: no cover
+    """
+    Creates an interactive visualization over a fairness report.
+    :param report: A fairness report.
+    :param name: Default is 'report'.
+    :param width: The minimum width of interactive plot screens.
+    :param height: The minimum height of interactive plot screens.
+    :param spacing: The minimum spacing between bars of bar plots. If None, internally set to 50 for horizontal mode and 100 otherwise.
+    :param horizontal: Whether bar plots should be horizontally or vertically aligned.
+    """
     from bokeh.models import (
         ColumnDataSource,
         Select,
-        Range1d,
         Button,
         Div,
-        FactorRange,
         HoverTool,
         RadioButtonGroup,
     )
     from bokeh.plotting import figure
     from bokeh.layouts import column, row
     from bokeh.server.server import Server
     from bokeh.application import Application
     from bokeh.application.handlers import FunctionHandler
     import webbrowser
     from bokeh.transform import factor_cmap
     from bokeh.palettes import Category20
     from bokeh.core.validation import silence
     from bokeh.core.validation.warnings import MISSING_RENDERERS
 
+    if spacing is None:
+        spacing = 50 if horizontal else 100
+
     silence(MISSING_RENDERERS, True)
 
     def modify_doc(doc):
-        plot = figure(x_range=["1", "2"], width=width)
+        if horizontal:
+            plot = figure(y_range=["1", "2"], width=width, height=height)
+        else:
+            plot = figure(x_range=["1", "2"], width=width, height=height)
         plot.add_tools(HoverTool(tooltips=[("Name", "@keys"), ("Value", "@values")]))
         select_branch = RadioButtonGroup(
             labels=["ALL"] + list(report.branches().keys()), active=0
         )
         select_view = Select(
             value="Branches", options=["Branches", "Entries"], width=100, height=30
         )
@@ -128,20 +147,26 @@
             select_branch.labels = ["ALL"] + list(_source.keys())
 
         def update_plot(doc):
             branches = _asdict(previous[-1])
             back.visible = len(previous) > 1 or select_branch.active != 0
             plot.renderers = []  # clear plot
             selected_branch = select_branch.labels[select_branch.active]
-            plot.x_range.factors = []
+            if horizontal:
+                plot.y_range.factors = []
+            else:
+                plot.x_range.factors = []
             select_view.disabled = not True
             plot.title.text = "" if selected_branch == "ALL" else selected_branch
             plot.title_location = "above"
             if selected_branch == "ALL":
-                plot.xgrid.grid_line_color = None
+                if horizontal:
+                    plot.ygrid.grid_line_color = None
+                else:
+                    plot.xgrid.grid_line_color = None
                 explain.visible = False
                 label.text = f"<h1>{'.'.join([t for t in previous_title if t!='ALL'])}</h1>Select a branch or entry to focus and explain it."
                 _source = dict()
                 if (select_view.value == select_view.options[0]) != isinstance(
                     previous[-1], Fork
                 ):
                     for branch in branches.keys():
@@ -170,75 +195,117 @@
                             for metric in _source[branch]
                         ]
                     except TypeError:
                         return
                 keys = [
                     (metric, branch) for metric in _source for branch in _source[metric]
                 ]
-                plot.width = max(800, 50*len(keys))
-                plot.x_range.factors = keys
+                if horizontal:
+                    plot.height = max(height, spacing * len(keys))
+                    plot.y_range.factors = keys
+                    plot.y_range.range_padding = 0.1
+                else:
+                    plot.width = max(width, spacing * len(keys))
+                    plot.x_range.factors = keys
+                    plot.x_range.range_padding = 0.1
                 source = ColumnDataSource(data=dict(keys=keys, values=values))
-                plot.x_range.range_padding = 0.1
-                plot.vbar(
-                    x="keys",
-                    top="values",
-                    width=0.9,
-                    source=source,
-                    # legend_field='keys',
-                    line_color="white",
-                    fill_color=factor_cmap(
-                        "keys",
-                        palette=[
-                            Category20[20][i]
-                            for metric in _source
-                            for i, branch in enumerate(_source[metric])
-                        ],
-                        factors=keys,
-                    ),
-                )
+                if horizontal:
+                    plot.hbar(
+                        y="keys",
+                        right="values",
+                        height=0.9,
+                        source=source,
+                        # legend_field='keys',
+                        line_color="white",
+                        fill_color=factor_cmap(
+                            "keys",
+                            palette=[
+                                Category20[20][i]
+                                for metric in _source
+                                for i, branch in enumerate(_source[metric])
+                            ],
+                            factors=keys,
+                        ),
+                    )
+                else:
+                    plot.vbar(
+                        x="keys",
+                        top="values",
+                        width=0.9,
+                        source=source,
+                        # legend_field='keys',
+                        line_color="white",
+                        fill_color=factor_cmap(
+                            "keys",
+                            palette=[
+                                Category20[20][i]
+                                for metric in _source
+                                for i, branch in enumerate(_source[metric])
+                            ],
+                            factors=keys,
+                        ),
+                    )
                 select_view.disabled = not True
             else:
                 select_view.disabled = not False
                 label.text = f"<h1>{'.'.join([t for t in previous_title if t!='ALL'])}.<em>{selected_branch}</em></h1>Select ALL to switch between branch and entry views."
                 plot_data = _branch(selected_branch)
                 explain.visible = hasattr(plot_data, "explain")
                 plot_data = _asdict(plot_data)
                 keys = list(plot_data.keys())
-                plot.width = max(800, 50*len(keys))
-                plot.x_range.factors = keys
+                if horizontal:
+                    plot.height = max(height, spacing * len(keys))
+                    plot.y_range.factors = keys
+                else:
+                    plot.width = max(width, spacing * len(keys))
+                    plot.x_range.factors = keys
                 if isinstance(plot_data, Fork):
                     plot_data = plot_data.branches()
                 try:
                     values = [tofloat(value) for value in plot_data.values()]
                 except TypeError:
                     return
                 source = ColumnDataSource(data=dict(keys=keys, values=values))
-                plot.xgrid.grid_line_color = None
+                if horizontal:
+                    plot.ygrid.grid_line_color = None
+                    plot.hbar(
+                        y="keys",
+                        right="values",
+                        height=0.6,
+                        source=source,
+                        # legend_field='keys',
+                        line_color="white",
+                        fill_color=factor_cmap(
+                            "keys", palette=Category20[20], factors=keys
+                        ),
+                    )
+                else:
+                    plot.xgrid.grid_line_color = None
+                    plot.vbar(
+                        x="keys",
+                        top="values",
+                        width=0.6,
+                        source=source,
+                        # legend_field='keys',
+                        line_color="white",
+                        fill_color=factor_cmap(
+                            "keys", palette=Category20[20], factors=keys
+                        ),
+                    )
                 # plot.y_range.update(start=0, end=max(1, max(values)), bounds=(0, None))
-                plot.vbar(
-                    x="keys",
-                    top="values",
-                    width=0.6,
-                    source=source,
-                    # legend_field='keys',
-                    line_color="white",
-                    fill_color=factor_cmap(
-                        "keys", palette=Category20[20], factors=keys
-                    ),
-                )
 
         def explain_button(doc):
             selected_branch = select_branch.labels[select_branch.active]
             previous_title.append(selected_branch)
             previous_title.append("explain")
             selected_branch = select_branch.labels[select_branch.active]
             branch = (
                 previous[-1] if selected_branch == "ALL" else _branch(selected_branch)
             )
-            previous.append(clean(branch.explain))
+            previous.append(_clean(branch.explain))
             _update_branches()
             select_branch.active = 0
             update_plot(doc)
 
         def back_button(doc):
             if select_branch.labels[select_branch.active] != "ALL":
                 select_branch.active = 0
@@ -271,15 +338,15 @@
             update_plot(doc)
 
         def update_value(doc):
             selected_branch = select_branch.labels[select_branch.active]
             if selected_branch != "ALL" and _depth(_branch(selected_branch)) > 1:
                 previous_title.append(selected_branch)
                 branch = _branch(selected_branch)
-                previous.append(clean(branch))
+                previous.append(_clean(branch))
                 _update_branches()
                 select_branch.active = 0
             update_plot(doc)
 
         def update_view(doc):
             _update_branches()
             update_plot(doc)
@@ -291,15 +358,15 @@
         explain.on_click(explain_button)
         back.on_click(back_button)
         update_plot(doc)
         controls = row(select_view, select_branch, back, explain)
         doc.add_root(column(label, controls, plot))
 
     app = Application(FunctionHandler(modify_doc))
-    if _in_ipynb():
+    if _in_jupyter():
         from bokeh.io import show
         from bokeh.plotting import output_notebook
 
         output_notebook()
         show(app)
         return
     server = Server({"/": app}, num_procs=1)
```

## fairbench/forks/explanation.py

```diff
@@ -48,19 +48,23 @@
         return self.x.shape[0]
 
     def __str__(self):
         return f"{self.name} ({self.points} points)"
 
 
 class Explainable(ClosedWrapper):
-    def __init__(self, value, explain: Any = None, desc: str = None, **kwargs):
+    def __init__(
+        self, value, explain: Any = None, desc: str = None, units: Any = None, **kwargs
+    ):
         from fairbench.forks import Fork
 
         if value.__class__.__name__ == "Future":
             value = value.result()
+        if isinstance(value, np.bool_):
+            value = bool(value)
         if isinstance(value, int) or isinstance(value, float):
             value = np.float64(value)
         assert (
             isinstance(value, float)
             or isinstance(value, int)
             or isinstance(value, np.floating)
             or "tensor" in value.__class__.__name__.lower()
@@ -68,23 +72,29 @@
         ), f"Can not set data type as explainable: {type(value)}"
         assert (
             explain is None or not kwargs
         ), "Cannot create explainable with both todict and a Fork"
         super().__init__(value)
         self.explain = Fork(kwargs) if explain is None else explain
         self.desc = desc
+        self.units = units
 
     def __float__(self):
         return tofloat(self.__value__())
 
     def __int__(self):
         return int(self.__float__())
 
     def __str__(self):
-        return f"{self.__float__():.3f}"
+        value = self.__float__()
+        if self.units is not None and (callable(self.units)):
+            return str(self.units(value))
+        if self.units is not None:
+            return f"{value:.3f} {self.units}"
+        return f"{value:.3f}"
 
     @property
     def value(self):
         return self.__value__()
 
     def numpy(self):
         return self.value.numpy()
```

## fairbench/forks/fork.py

```diff
@@ -12,14 +12,15 @@
     if isinstance(v, Fork):
         v = v.branches()
     if isinstance(v, dict):
         complicated = False
         for val in v.values():
             if isinstance(val, Fork) or isinstance(val, dict):
                 complicated = True
+        tmp = list(v.values())[0]
         return "\n".join(
             "   " * tabs
             + k
             + ": "
             + ("\n" if complicated else "")
             + _str_foreign(fromtensor(v), tabs + 1)
             for k, v in v.items()
@@ -114,15 +115,18 @@
 def astensor(value, _allow_explanation=True) -> ep.Tensor:
     if value.__class__.__name__ == "Explainable" and not _allow_explanation:
         value = value.value
     elif value.__class__.__name__ == "Explainable":
         from fairbench import Explainable
 
         return Explainable(
-            astensor(value.value), explain=value.explain, desc=value.desc
+            astensor(value.value),
+            explain=value.explain,
+            desc=value.desc,
+            units=value.units,
         )
     if isinstance(value, int) or isinstance(value, float):
         value = np.float64(value)
     if (
         "tensor" not in value.__class__.__name__.lower()
         and "array" not in value.__class__.__name__.lower()
         and not isinstance(value, np.float64)
@@ -143,15 +147,18 @@
 def fromtensor(value, _allow_explanation=True):
     if value.__class__.__name__ == "Explainable" and not _allow_explanation:
         value = value.value
     elif value.__class__.__name__ == "Explainable":
         from fairbench import Explainable
 
         return Explainable(
-            fromtensor(value.value), explain=value.explain, desc=value.desc
+            fromtensor(value.value),
+            explain=value.explain,
+            desc=value.desc,
+            units=value.units,
         )
     # TODO: maybe applying this as a wrapper to methods instead of submitting to dask can be faster
     if isinstance(value, ep.Tensor):
         return value.raw
 
     return value
 
@@ -750,20 +757,20 @@
 
 @parallel_primitive
 def merge(dict1, dict2):
     return Forklike({**dict1, **dict2})
 
 
 @comparator
-def combine(*args, _role=None):
+def combine(*args, _role=None, _cast=Fork):
     ret = {}
     for arg in args:
-        assert isinstance(arg, Fork)
-        ret = merge(ret, arg._branches)
-    return Fork(ret)
+        assert isinstance(arg, Fork) or isinstance(arg, Forklike)
+        ret = merge(ret, arg._branches if isinstance(arg, Fork) else arg)
+    return _cast(ret)
 
 
 def unit_bounded(method):
     @wraps(method)
     def wrapper(*args, **kwargs):
         for iter in [args, kwargs.values()]:
             for arg in iter:
```

## fairbench/metrics/classification.py

```diff
@@ -1,56 +1,59 @@
 from fairbench.forks import parallel, unit_bounded, role
 from fairbench.forks.explanation import Explainable
 from eagerpy import Tensor
+from typing import Optional
 
 
 @role("metric")
 @parallel
 @unit_bounded
-def accuracy(predictions: Tensor, labels: Tensor, sensitive: Tensor = None):
+def accuracy(predictions: Tensor, labels: Tensor, sensitive: Optional[Tensor] = None) -> Explainable:
     if sensitive is None:
         sensitive = predictions.ones_like()
     num_sensitive = sensitive.sum()
     true = ((predictions - labels) * sensitive).abs().sum()
     return Explainable(
         0 if num_sensitive == 0 else 1 - true / num_sensitive,
         samples=num_sensitive,
         true=true,
     )
 
 
 @role("metric")
 @parallel
 @unit_bounded
-def pr(predictions: Tensor, sensitive: Tensor = None):
+def pr(predictions: Tensor, sensitive: Optional[Tensor] = None):
     if sensitive is None:
         sensitive = predictions.ones_like()
     sum_sensitive = sensitive.sum()
     sum_positives = (predictions * sensitive).sum()
     return Explainable(
         0 if sum_sensitive == 0 else (sum_positives / sum_sensitive),
         samples=sum_sensitive,
         positives=sum_positives,
     )
 
 
 @role("metric")
 @parallel
 @unit_bounded
-def positives(predictions: Tensor, sensitive: Tensor):
-    return (predictions * sensitive).sum()
+def positives(predictions: Tensor, sensitive: Optional[Tensor] = None):
+    if sensitive is None:
+        sensitive = predictions.ones_like()
+    return Explainable((predictions * sensitive).sum(), samples=sensitive.sum())
 
 
 @role("metric")
 @parallel
 @unit_bounded
 def tpr(
     predictions: Tensor,
     labels: Tensor,
-    sensitive: Tensor = None,
+    sensitive: Optional[Tensor] = None,
     max_prediction: float = 1,
 ):
     if sensitive is None:
         sensitive = predictions.ones_like()
     error = (max_prediction - (predictions - labels).abs()) * predictions
     error_sensitive = error * sensitive
     num_sensitive = (sensitive * predictions).sum()
@@ -64,15 +67,15 @@
 
 @role("metric")
 @parallel
 @unit_bounded
 def fpr(
     predictions: Tensor,
     labels: Tensor,
-    sensitive: Tensor = None,
+    sensitive: Optional[Tensor] = None,
 ):
     if sensitive is None:
         sensitive = predictions.ones_like()
     error = (predictions - labels).abs() * predictions
     error_sensitive = error * sensitive
     num_sensitive = (sensitive * predictions).sum()
     if num_sensitive == 0:
@@ -87,15 +90,15 @@
 
 @role("metric")
 @parallel
 @unit_bounded
 def tnr(
     predictions: Tensor,
     labels: Tensor,
-    sensitive: Tensor = None,
+    sensitive: Optional[Tensor] = None,
     max_prediction: float = 1,
 ):
     if sensitive is None:
         sensitive = predictions.ones_like()
     negatives = max_prediction - predictions
     error = (max_prediction - (predictions - labels).abs()) * negatives
     error_sensitive = error * sensitive
@@ -110,15 +113,15 @@
 
 @role("metric")
 @parallel
 @unit_bounded
 def fnr(
     predictions: Tensor,
     labels: Tensor,
-    sensitive: Tensor = None,
+    sensitive: Optional[Tensor] = None,
     max_prediction: float = 1,
 ):
     if sensitive is None:
         sensitive = predictions.ones_like()
     negatives = max_prediction - predictions
     error = (predictions - labels).abs() * negatives
     error_sensitive = error * sensitive
```

## fairbench/metrics/regression.py

```diff
@@ -15,15 +15,15 @@
     if sensitive is None:
         sensitive = scores.ones_like()
     num_sensitive = sensitive.sum()
     true = ((scores - targets) * sensitive).abs().sum()
     return Explainable(
         0 if num_sensitive == 0 else true / num_sensitive,
         samples=num_sensitive,
-        sse=true,
+        sae=true,
     )
 
 
 @role("metric")
 @parallel
 def rmse(scores: Tensor, targets: Tensor, sensitive: Tensor = None):
     if sensitive is None:
@@ -74,15 +74,15 @@
         sse=true,
     )
 
 
 @role("metric")
 @parallel
 def pinball(
-    scores: Tensor, targets: Tensor, alpha: float = 0.5, sensitive: Tensor = None
+    scores: Tensor, targets: Tensor, sensitive: Tensor = None, alpha: float = 0.5
 ):
     assert 0 <= alpha <= 1
     if sensitive is None:
         sensitive = scores.ones_like()
     num_sensitive = sensitive.sum()
     loss = alpha * (targets - scores).maximum(0) + (1 - alpha) * (
         scores - targets
```

## fairbench/reports/adhoc.py

```diff
@@ -1,8 +1,8 @@
-from fairbench.reports.base import report, reportargsparse
+from fairbench.reports.base import report
 from fairbench.reports import reduction as fb
 from fairbench.reports.accumulate import todict as tokwargs
 from fairbench.forks.fork import combine, merge, role
 from fairbench.reports.surrogate import surrogate_positives
 from fairbench import metrics
 from fairbench.reports import reduction
```

## Comparing `fairbench-0.2.7.dist-info/METADATA` & `fairbench-0.2.8.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbench
-Version: 0.2.7
+Version: 0.2.8
 Summary: Fairness model assessment framework
 Home-page: https://github.com/mever-team/FairBench
 Author: Emmanouil (Manios) Krasanakis
 Author-email: maniospas@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,10 +17,11 @@
 Requires-Dist: makefun
 Requires-Dist: matplotlib
 Requires-Dist: wget
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: objwrap
 Requires-Dist: bokeh
+Requires-Dist: pyyaml
 
 For tutorials, documentation, and contribution guidelines, please visit the project's homepage at https://github.com/mever-team/FairBench
```

## Comparing `fairbench-0.2.7.dist-info/RECORD` & `fairbench-0.2.8.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-fairbench/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
+fairbench/__init__.py,sha256=Ido_Y_0n5fjUZDnEXn5vFcHTNnSJBJ95PI8sp_Y_Gpo,411
 fairbench/export.py,sha256=_u97-Yi8VArkwof63mcVXgnUD-i9AY1vjxtCnQ_jKcs,1952
+fairbench/stamps.py,sha256=naC2tvM9ihnMyFqlInP57thAgCf5af4000fjY8snNCE,5762
 fairbench/bench/__init__.py,sha256=piA_S0SAZ96_-MxdcGO_V7pCKngOFBeAv8KGj9rkGRA,38
 fairbench/bench/demos.py,sha256=ODVbSjCVrl_S1lP7cZOyoaVFPUZmsz75SYbeD3sflFY,2341
 fairbench/bench/loader.py,sha256=P1PiDtR67NFSk_lIQvzQ0Wez2ZvcxprP7zMpsLcsTYo,1660
-fairbench/export/__init__.py,sha256=Qzq3t-sg7-4M2Vz_76s6dnuQ6K6fRETQo0Ad5Qj2NEI,93
-fairbench/export/interactive.py,sha256=yLMF_Qa9AcBBlbM30QL9vlsKLqmRsYJWUfUMEFuHWPw,13283
+fairbench/export/__init__.py,sha256=ZQ3m4piX_o-z5mlmG_H7O26SGuhKo7b38Nc64Bs8pik,134
+fairbench/export/interactive.py,sha256=N38BHs9PukvikIg8dasefsWArYWMa3ZxPzmlluxa5YI,16295
 fairbench/export/native.py,sha256=s9houeUkqPRIx76Ke4NxqHED650XWAZu6s27ndXiCnA,2912
+fairbench/export/modelcards/__init__.py,sha256=B9gsTh-sWzIkY5pIPSPJ8ZdurlBsr2MS4o95n3WXXj0,173
+fairbench/export/modelcards/tohtml.py,sha256=IkVy8NpNBe-OYjc68QPWZeSfAHp5b9rvZ6fl8y5-J0Y,2856
+fairbench/export/modelcards/tomarkdown.py,sha256=Jesxn2AF0lRrDZxCjhj47phKI-PmLIdQ02GNrzoZjKk,2423
+fairbench/export/modelcards/toyaml.py,sha256=-DW4YcICcuWiNGdtECTKam7XlDXliuf4S3UvJzJrp6g,562
 fairbench/forks/__init__.py,sha256=eBRDSxc31Pc1yKCc1VjFBvPMsBVaOzVOfXHpkYQodG0,122
 fairbench/forks/categorical.py,sha256=nfsA1ZjrrywMzOhEoPUF6_9oazIJWcZEI4gvil-1VIs,2130
-fairbench/forks/explanation.py,sha256=Wy6Xm5nUUOLQ7D-pyPY7o28rWiSj4_DN1dyB_WIegTE,2586
-fairbench/forks/fork.py,sha256=c1Tcbkt-wSni0Jxc0fwiAuHOba7rQv5ntTn-moJQfKo,26645
+fairbench/forks/explanation.py,sha256=x6zqF4b9dc1-XBg_xAQXu43czI4f900mrwEgoo-vR6o,2936
+fairbench/forks/fork.py,sha256=cpWhnUNZFYfJDq_k8k1IJGgKZ-Cb88z-6a6PAk-Mbto,26874
 fairbench/metrics/__init__.py,sha256=kqs5vladIyri5R_l4u6fcte-O4j_n-jt9OeiIRA2KPo,239
-fairbench/metrics/classification.py,sha256=6q1Lu6up8qjs2nxe-GXKRVjmrBuzJ6j0cIY7ip6ZAco,3777
+fairbench/metrics/classification.py,sha256=TcenssnwmcwQkn19B5537mGuKvBWZigCo8f6vmUP1CA,4008
 fairbench/metrics/disparate_impact.py,sha256=VJw9Q4cA1YqP9fTTE-aMMUzjeuk072L-HRow_vaLkZA,2066
 fairbench/metrics/disparate_mistreatment.py,sha256=ORoUcMU_Dh18Ytz4dgQn8wPyaNJ_w98m_oegxI90vc4,1494
 fairbench/metrics/ranking.py,sha256=jnj-Ig9JgxeHqkt7v7uDfosEk-0gGv8lhXYGlkx7YKM,668
-fairbench/metrics/regression.py,sha256=XIfP9cgOHMsWw-mS-eahO9JxDhM6YHyqIXOPi1yjDq0,2970
+fairbench/metrics/regression.py,sha256=w7zVO0hfLABovxIzGZ7XkWzYfT9eJOA2ceIME7XPMeQ,2970
 fairbench/mitigation/__init__.py,sha256=f-owl1xAKGweXEuVbFJGYSel3-7kccvTo6SEziKmXRk,100
 fairbench/mitigation/postprocessing.py,sha256=CF2WcAWQKKfNRJ4yvNqIjuNdLaCBrSIpI_XNhmfiUkY,1790
 fairbench/reports/__init__.py,sha256=YQm7A6K3PUB4uNOw3iDu2RUaoWa07Rsn3GJr4wZkn2M,207
 fairbench/reports/accumulate.py,sha256=jDlJFb1bK9nRfumzSWFbCpAGWi8aCOFil4L8Hj44xe0,1491
-fairbench/reports/adhoc.py,sha256=s4yyItIgq61SBKYA8nzhd7lxQXrdDWy3tvc72_-Swtk,2021
+fairbench/reports/adhoc.py,sha256=RWoOXYLZRLvKEXO5FAhTltXWZiv1WkoRv9xlsnx99D0,2004
 fairbench/reports/base.py,sha256=KQHdSzzU7c3uH0cmV7CmU1YUlIwKhRviGtAGucNEzk4,2590
 fairbench/reports/surrogate.py,sha256=LnV6kkNPMGL2SYEBSSIFWjkXQ8N5m2k4y5as2zUyDt8,883
 fairbench/reports/reduction/__init__.py,sha256=a3c0w4bKV3f6NXnGMPPGFRxdfg_YIrcccy_mEBSr8zk,155
 fairbench/reports/reduction/expanders.py,sha256=DZvDpfXw8LI3ZquA5c22-25PSuLsOhpp_B_IYo5VeVY,2260
 fairbench/reports/reduction/reduce.py,sha256=H6_rIdw4JZRkhpS2ldpi3kPgBKuHjcQ6OOuXwPyRIUk,2637
 fairbench/reports/reduction/reducers.py,sha256=EQlN9rCKDBJmls0rtoA9vyAlrIyIBzQCCcpRDBMRlMA,2834
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_batching.py,sha256=bXewsKXAlDTeyZZ8OlG74-qYQ_hhiwcYJigxy0M_YKY,1394
 tests/test_benchmarks.py,sha256=RZwehxePgR6fwFCh9HWbK3rXsXQNLHomrn7M6BboiMw,1278
 tests/test_demos.py,sha256=VgXBcev7XAnvy2OWiOZf0yBNXzhkjWvf0Bl6of00WzM,1103
 tests/test_forks.py,sha256=Dyu5UPAFG8fxVCfeZ9JwisVwUtZT0NV1WqAMe2GXt3Y,5807
 tests/test_metrics.py,sha256=mbG4oetiyfihNwIKj620SZmARxX8YuGeuAhebOv9gH4,2685
+tests/test_modelcards.py,sha256=v73DtkMJZGnfnTEymv48ad2qsQCn7XI6nOs7OedTckE,1150
 tests/test_reduction.py,sha256=JMXZeh3Catiboki8TG50A_caMh4zpSt_NKScqGS2Pr0,1624
 tests/test_reports.py,sha256=2nNSZjkrTdZl8P5bvEz8dDdRd_W7CmSvn51GDdHFPvo,6556
-fairbench-0.2.7.dist-info/METADATA,sha256=sP-bVZyLm1iGOvCvc6eK-r-v_LUxLwYdbAvoy4XAM-w,830
-fairbench-0.2.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-fairbench-0.2.7.dist-info/top_level.txt,sha256=lrkG910bN_2UdVUqCXaR6aeRjjXfOQX2-wSeVjhhFnM,16
-fairbench-0.2.7.dist-info/RECORD,,
+fairbench-0.2.8.dist-info/METADATA,sha256=lQJlnEv1BcVJmYM9akxXdF8lnBRAX4mGZvW-Bpd1Nrs,852
+fairbench-0.2.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+fairbench-0.2.8.dist-info/top_level.txt,sha256=lrkG910bN_2UdVUqCXaR6aeRjjXfOQX2-wSeVjhhFnM,16
+fairbench-0.2.8.dist-info/RECORD,,
```

