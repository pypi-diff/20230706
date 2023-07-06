# Comparing `tmp/nemreport-0.0.2.tar.gz` & `tmp/nemreport-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemreport-0.0.2.tar", last modified: Thu Jun 22 10:30:47 2023, max compression
+gzip compressed data, was "nemreport-0.0.3.tar", last modified: Thu Jul  6 10:34:38 2023, max compression
```

## Comparing `nemreport-0.0.2.tar` & `nemreport-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rwxr-xr-x   0        0        0     1836 2023-06-15 10:33:44.765933 nemreport-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2023-04-13 01:26:35.356696 nemreport-0.0.2/LICENSE
--rw-r--r--   0        0        0       30 2023-06-15 10:36:18.254519 nemreport-0.0.2/MANIFEST.in
--rwxr-xr-x   0        0        0      652 2023-06-16 23:16:51.756079 nemreport-0.0.2/README.md
--rw-r--r--   0        0        0      126 2023-06-15 10:11:36.097013 nemreport-0.0.2/nemreport/__init__.py
--rw-r--r--   0        0        0       28 2022-10-22 23:26:41.883203 nemreport-0.0.2/nemreport/__main__.py
--rw-r--r--   0        0        0      916 2023-06-22 10:25:53.156068 nemreport-0.0.2/nemreport/cli.py
--rw-r--r--   0        0        0     2426 2023-06-22 10:21:33.221684 nemreport-0.0.2/nemreport/model.py
--rw-r--r--   0        0        0      612 2023-06-22 10:28:30.895126 nemreport-0.0.2/nemreport/prepare_db.py
--rwxr-xr-x   0        0        0     7853 2023-06-22 10:21:47.042078 nemreport-0.0.2/nemreport/report.py
--rw-r--r--   0        0        0   163873 2023-04-13 01:26:35.356696 nemreport-0.0.2/nemreport/templates/bootstrap.min.css
--rw-r--r--   0        0        0      735 2023-04-19 10:22:38.621358 nemreport-0.0.2/nemreport/templates/index.html
--rwxr-xr-x   0        0        0    11094 2023-06-16 10:34:56.714032 nemreport-0.0.2/nemreport/templates/nmi-report.html
--rw-r--r--   0        0        0       22 2023-06-22 10:08:41.553442 nemreport-0.0.2/nemreport/version.py
--rwxr-xr-x   0        0        0     1426 2023-06-22 10:08:33.957250 nemreport-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2875 2023-06-22 10:11:26.616749 nemreport-0.0.2/requirements.txt
--rw-r--r--   0        0        0   285444 2023-06-16 23:15:18.935529 nemreport-0.0.2/screenshot.png
--rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883203 nemreport-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      559 2023-06-22 10:29:36.060259 nemreport-0.0.2/tests/test_cli.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 nemreport-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      135 2022-11-03 05:28:29.076363 nemreport-0.0.3/.flake8
+-rwxr-xr-x   0        0        0     1836 2023-06-15 10:33:44.765933 nemreport-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2023-04-13 01:26:35.356696 nemreport-0.0.3/LICENSE
+-rw-r--r--   0        0        0       30 2023-06-15 10:36:18.254519 nemreport-0.0.3/MANIFEST.in
+-rwxr-xr-x   0        0        0      652 2023-06-16 23:16:51.756079 nemreport-0.0.3/README.md
+-rw-r--r--   0        0        0      126 2023-06-15 10:11:36.097013 nemreport-0.0.3/nemreport/__init__.py
+-rw-r--r--   0        0        0       28 2022-10-22 23:26:41.883203 nemreport-0.0.3/nemreport/__main__.py
+-rw-r--r--   0        0        0      916 2023-06-22 10:25:53.156068 nemreport-0.0.3/nemreport/cli.py
+-rw-r--r--   0        0        0     5131 2023-07-06 10:28:31.528835 nemreport-0.0.3/nemreport/model.py
+-rw-r--r--   0        0        0      612 2023-06-22 10:28:30.895126 nemreport-0.0.3/nemreport/prepare_db.py
+-rwxr-xr-x   0        0        0    10549 2023-07-06 10:33:26.366407 nemreport-0.0.3/nemreport/report.py
+-rw-r--r--   0        0        0   163873 2023-04-13 01:26:35.356696 nemreport-0.0.3/nemreport/templates/bootstrap.min.css
+-rw-r--r--   0        0        0      735 2023-04-19 10:22:38.621358 nemreport-0.0.3/nemreport/templates/index.html
+-rwxr-xr-x   0        0        0    11186 2023-06-24 10:26:06.553344 nemreport-0.0.3/nemreport/templates/nmi-report.html
+-rw-r--r--   0        0        0       22 2023-07-06 10:33:56.967106 nemreport-0.0.3/nemreport/version.py
+-rwxr-xr-x   0        0        0     1426 2023-06-22 10:08:33.957250 nemreport-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2875 2023-06-22 10:11:26.616749 nemreport-0.0.3/requirements.txt
+-rw-r--r--   0        0        0   285444 2023-06-16 23:15:18.935529 nemreport-0.0.3/screenshot.png
+-rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883203 nemreport-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      559 2023-06-22 10:29:36.060259 nemreport-0.0.3/tests/test_cli.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 nemreport-0.0.3/PKG-INFO
```

### Comparing `nemreport-0.0.2/.gitignore` & `nemreport-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/LICENSE` & `nemreport-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/README.md` & `nemreport-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/nemreport/cli.py` & `nemreport-0.0.3/nemreport/cli.py`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/nemreport/prepare_db.py` & `nemreport-0.0.3/nemreport/prepare_db.py`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/nemreport/report.py` & `nemreport-0.0.3/nemreport/report.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 from datetime import datetime, time
 from pathlib import Path
 from typing import List, Optional
 
 import calplot
 import pandas as pd
 import plotly.express as px
+import plotly.graph_objects as go
 from jinja2 import Environment, FileSystemLoader
+from nemreader import extend_sqlite
 from nemreader.output_db import get_nmis
 
 from .model import (
     DB_PATH,
     db,
     get_annual_data,
     get_date_range,
     get_day_data,
+    get_day_profile,
+    get_day_profiles,
     get_season_data,
     get_usage_df,
 )
 from .prepare_db import update_nem_database
 
 log = logging.getLogger(__name__)
 this_dir = Path(__file__).parent
@@ -38,29 +42,33 @@
 env.filters["yearmonth"] = format_month
 
 
 def build_daily_usage_chart(nmi: str, kind: str) -> Optional[Path]:
     """Save calendar plot"""
     days = []
     data = []
-    for dt, imp, exp, _, _, _, _ in get_day_data(nmi):
+    for (
+        dt,
+        imp,
+        exp,
+    ) in get_day_data(nmi):
         days.append(dt)
-        exp = -exp  # Make export negative
         if kind == "import":
             data.append(imp)
         elif kind == "export":
             data.append(exp)
         elif kind == "total":
+            exp = -exp  # Make export negative
             val = imp + exp
             data.append(val)
         else:
             raise ValueError("Invalid usage chart kind")
 
     if kind == "export":
-        if min(data) == 0.0:
+        if max(data) == 0.0:
             return None
 
     vmin = max(-35, min(data))
     vmax = min(35, max(data))
 
     data = pd.Series(data, index=days)
     plot = calplot.calplot(
@@ -76,33 +84,88 @@
     fig = plot[0]
     file_path = output_dir / f"{nmi}_daily_{kind}.png"
     fig.savefig(file_path, bbox_inches="tight")
     log.info("Created %s", file_path)
     return file_path
 
 
+def build_day_profile_plot(nmi: str) -> str:
+    """Save profile plot"""
+    try:
+        df = get_day_profile(nmi)
+    except ValueError:
+        return ""
+    # trace = go.Scatter(x=df["time"], y=df["Avg kW"], name="Avg kW")
+    traces = []
+    color_dict = {
+        "SUMMER": "red",
+        "AUTUMN": "green",
+        "WINTER": "blue",
+        "SPRING": "purple",
+    }
+    for season in ["SUMMER", "AUTUMN", "WINTER", "SPRING"]:
+        if season in df:
+            color = color_dict[season]
+            trace = go.Scatter(
+                x=df["time"], y=df[season], name=season, marker=dict(color=color)
+            )
+            traces.append(trace)
+    fig = go.Figure(data=traces)
+    x_values = ["04:00", "09:00", "16:00", "21:00"]
+    for x in x_values:
+        fig.add_vline(x=x, line_width=1, line_dash="dash", line_color="black")
+    fig.update_layout(
+        legend=dict(orientation="h", yanchor="top", y=1.02, xanchor="right", x=1)
+    )
+    fig.update_xaxes(dtick=12)
+
+    file_path = output_dir / f"{nmi}_day_profile.html"
+    fig.write_html(file_path, full_html=False, include_plotlyjs="cdn")
+    log.info("Created %s", file_path)
+    return file_path
+
+
+def build_histogram_plot(nmi: str) -> str:
+    """Save profile plot"""
+    df = get_day_profiles(nmi)
+    fig = px.histogram(df, x="Avg kW", log_y=True)
+    file_path = output_dir / f"{nmi}_histogram.html"
+    fig.write_html(file_path, full_html=False, include_plotlyjs="cdn")
+    log.info("Created %s", file_path)
+    return file_path
+
+
+def build_days_profiles_plot(nmi: str) -> str:
+    """Save profile plot"""
+    df = get_day_profiles(nmi)
+    fig = px.line(df, x="time", y="Avg kW", color="day")
+    x_values = ["04:00", "09:00", "16:00", "21:00"]
+    for x in x_values:
+        fig.add_vline(x=x, line_width=1, line_dash="dash", line_color="black")
+    fig.update_xaxes(dtick=12)
+    fig.update_traces(line_color="royalblue", showlegend=False)
+    file_path = output_dir / f"{nmi}_days_profiles.html"
+    fig.write_html(file_path, full_html=False, include_plotlyjs="cdn")
+    log.info("Created %s", file_path)
+    return file_path
+
+
 def build_daily_plot(nmi: str) -> str:
     """Save calendar plot"""
 
     day_data = list(get_day_data(nmi))
     data = {
-        "morning": [x[3] for x in day_data],
-        "day": [x[4] for x in day_data],
-        "evening": [x[5] for x in day_data],
-        "night": [x[6] for x in day_data],
+        "import": [x[1] for x in day_data],
         "export": [-x[2] for x in day_data],
     }
     index = [x[0] for x in day_data]
     df = pd.DataFrame(index=index, data=data)
     color_dict = {
         "export": "green",
-        "morning": "tan",
-        "day": "skyblue",
-        "evening": "orangered",
-        "night": "slategrey",
+        "import": "orangered",
     }
     fig = px.bar(df, x=df.index, y=list(data.keys()), color_discrete_map=color_dict)
     fig.update_xaxes(
         rangeslider_visible=False,
         rangeselector=dict(
             buttons=list(
                 [
@@ -110,14 +173,18 @@
                     dict(count=6, label="6m", step="month", stepmode="backward"),
                     dict(count=1, label="1y", step="year", stepmode="backward"),
                     dict(step="all"),
                 ]
             )
         ),
     )
+    fig.update_layout(
+        xaxis_title=None,
+        yaxis_title="kWh",
+    )
     file_path = output_dir / f"{nmi}_daily_plot.html"
     fig.write_html(file_path, full_html=False, include_plotlyjs="cdn")
     log.info("Created %s", file_path)
     return file_path
 
 
 def build_usage_histogram(nmi: str) -> str:
@@ -215,33 +282,50 @@
 
 
 def build_report(nmi: str):
     template = env.get_template("nmi-report.html")
     start, end = get_date_range(nmi)
     fp_imp = build_daily_usage_chart(nmi, "import")
     fp_exp = build_daily_usage_chart(nmi, "export")
+
     build_daily_usage_chart(nmi, "total")
     has_export = True if fp_exp else None
 
-    """
     ch_daily_fp = build_daily_plot(nmi)
     with open(ch_daily_fp, "r") as fh:
         daily_chart = fh.read()
-    """
 
     ch_tou_fp = build_usage_histogram(nmi)
     with open(ch_tou_fp, "r") as fh:
         tou_chart = fh.read()
 
+    profile_fp = build_day_profile_plot(nmi)
+    if profile_fp:
+        with open(profile_fp, "r") as fh:
+            profile_chart = fh.read()
+    else:
+        profile_chart = ""
+
+    profiles_fp = build_days_profiles_plot(nmi)
+    with open(profiles_fp, "r") as fh:
+        profiles_chart = fh.read()
+
+    histogram_fp = build_histogram_plot(nmi)
+    with open(histogram_fp, "r") as fh:
+        histogram_chart = fh.read()
+
     report_data = {
         "start": start,
         "end": end,
         "has_export": has_export,
-        "daily_chart": "",
+        "daily_chart": daily_chart,
         "tou_chart": tou_chart,
+        "profile_chart": profile_chart,
+        "profiles_chart": profiles_chart,
+        "histogram_chart": histogram_chart,
         "imp_overview_chart": fp_imp.name,
         "exp_overview_chart": fp_exp.name if has_export else None,
         "season_data": get_seasonal_data(nmi),
         "annual_data": get_annual_data(nmi),
         "month_data": get_month_data(nmi),
     }
 
@@ -262,14 +346,15 @@
     logging.info("Created %s", file_path)
     return file_path
 
 
 def build_reports():
     if "daily_reads" not in db.table_names():
         update_nem_database()
+    extend_sqlite(DB_PATH)
     copy_static_data()
     nmis = get_nmis(DB_PATH)
     for nmi in nmis:
         build_report(nmi)
     fp = Path(build_index(nmis)).resolve()
     webbrowser.open(fp.as_uri())
     return fp
```

### Comparing `nemreport-0.0.2/nemreport/templates/bootstrap.min.css` & `nemreport-0.0.3/nemreport/templates/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/nemreport/templates/index.html` & `nemreport-0.0.3/nemreport/templates/index.html`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/nemreport/templates/nmi-report.html` & `nemreport-0.0.3/nemreport/templates/nmi-report.html`

 * *Files 1% similar despite different names*

```diff
@@ -180,21 +180,28 @@
                 </tr>
                 {% endfor %}
             </tbody>
         </table>
 
 
         <h2>More Charts</h2>
+
+        {{profile_chart}}
+
+        {{profiles_chart}}
+
         <img src="{{imp_overview_chart}}" class="img-fluid">
 
         {% if exp_overview_chart %}
         <img src="{{exp_overview_chart}}" class="img-fluid">
         {% endif %}
 
         {{daily_chart}}
+
+        {{histogram_chart}}
     </div><!-- Container -->
 
 
     <script>
         function calculateTotal() {
 
             var numDays = 365;
```

#### html2text {}

```diff
@@ -45,9 +45,10 @@
 Month        #Days           Imp (morning)          Imp (day)          Imp (evening)          Imp (night)          Imp (total)    Exp
              {
 {            {row.num_days}} {                      {                  {                      {                    {              {
 {row.month}} {% if           {row.imp_morning|round {row.imp_day|round {row.imp_evening|round {row.imp_night|round {row.imp|round {row.exp|round
              row.incomplete  (2)}}                  (2)}}              (2)}}                  (2)}}                (2)}}          (2)}}
              %}*{% endif %}
 ***** More Charts *****
-[{{imp_overview_chart}}] {% if exp_overview_chart %} [{{exp_overview_chart}}]
-{% endif %} {{daily_chart}}
+{{profile_chart}} {{profiles_chart}} [{{imp_overview_chart}}] {% if
+exp_overview_chart %} [{{exp_overview_chart}}] {% endif %} {{daily_chart}} {
+{histogram_chart}}
```

### Comparing `nemreport-0.0.2/pyproject.toml` & `nemreport-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/requirements.txt` & `nemreport-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/screenshot.png` & `nemreport-0.0.3/screenshot.png`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/tests/test_cli.py` & `nemreport-0.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.2/PKG-INFO` & `nemreport-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemreport
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate energy report from NEM meter data files
 Keywords: energy,NEM12,NEM13
 Author-email: Alex Guinman <alex@guinman.id.au>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

