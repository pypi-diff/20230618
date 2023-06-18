# Comparing `tmp/psychoanalyze-0.4.0.tar.gz` & `tmp/psychoanalyze-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.4.0.tar", max compression
+gzip compressed data, was "psychoanalyze-0.4.3.tar", max compression
```

## Comparing `psychoanalyze-0.4.0.tar` & `psychoanalyze-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-06-08 02:40:55.265614 psychoanalyze-0.4.0/LICENSE
--rw-r--r--   0        0        0     1002 2023-06-08 02:40:55.265614 psychoanalyze-0.4.0/README.md
--rw-r--r--   0        0        0     1250 2023-06-08 02:42:44.282548 psychoanalyze-0.4.0/psychoanalyze/__init__.py
--rw-r--r--   0        0        0     6402 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/blocks.py
--rw-r--r--   0        0        0     2133 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/data.py
--rw-r--r--   0        0        0      148 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/gescheider.py
--rw-r--r--   0        0        0     8869 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/layout.py
--rw-r--r--   0        0        0     5594 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/plot.py
--rw-r--r--   0        0        0     5017 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/points.py
--rw-r--r--   0        0        0     1784 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/schemas.py
--rw-r--r--   0        0        0     2285 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/sessions.py
--rw-r--r--   0        0        0     2380 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/simulate.py
--rw-r--r--   0        0        0       95 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/stimulus.py
--rw-r--r--   0        0        0      565 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/strength_duration.py
--rw-r--r--   0        0        0      611 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/subjects.py
--rw-r--r--   0        0        0        0 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/transformations.py
--rw-r--r--   0        0        0     4129 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/trials.py
--rw-r--r--   0        0        0     1692 2023-06-08 02:40:55.349614 psychoanalyze-0.4.0/psychoanalyze/weber.py
--rw-r--r--   0        0        0     2011 2023-06-08 02:42:44.282548 psychoanalyze-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 psychoanalyze-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-18 00:09:39.105786 psychoanalyze-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1188 2023-06-18 00:09:39.105786 psychoanalyze-0.4.3/README.md
+-rw-r--r--   0        0        0     1307 2023-06-18 00:11:42.137768 psychoanalyze-0.4.3/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/__main__.py
+-rw-r--r--   0        0        0      358 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/app.py
+-rw-r--r--   0        0        0     6216 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/blocks.py
+-rw-r--r--   0        0        0       90 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/dashboard/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/dashboard/__main__.py
+-rw-r--r--   0        0        0      219 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/dashboard/app.py
+-rw-r--r--   0        0        0     5239 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/dashboard/callbacks.py
+-rw-r--r--   0        0        0     6932 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/dashboard/layout.py
+-rw-r--r--   0        0        0     2133 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/data.py
+-rw-r--r--   0        0        0      148 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/gescheider.py
+-rw-r--r--   0        0        0     5602 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     5024 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/points.py
+-rw-r--r--   0        0        0     1784 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/schemas.py
+-rw-r--r--   0        0        0     2289 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/sessions.py
+-rw-r--r--   0        0        0     2380 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/simulate.py
+-rw-r--r--   0        0        0       95 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/stimulus.py
+-rw-r--r--   0        0        0      565 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/strength_duration.py
+-rw-r--r--   0        0        0      642 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/subjects.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/transformations.py
+-rw-r--r--   0        0        0     3367 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/trials.py
+-rw-r--r--   0        0        0     1692 2023-06-18 00:09:39.181790 psychoanalyze-0.4.3/psychoanalyze/weber.py
+-rw-r--r--   0        0        0     1499 2023-06-18 00:11:42.137768 psychoanalyze-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 psychoanalyze-0.4.3/PKG-INFO
```

### Comparing `psychoanalyze-0.4.0/LICENSE` & `psychoanalyze-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.0/README.md` & `psychoanalyze-0.4.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Psychophysics analysis in Python.
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psychoanalyze)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Open in Remote - Containers](https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/psychoanalyze/psychoanalyze)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/psychoanalyze/psychoanalyze/main.svg)](https://results.pre-commit.ci/latest/github/psychoanalyze/psychoanalyze/main)
+
 
 
 ## Installation
 poetry (preferred):
 ```console
 poetry add psychoanalyze
 ```
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/__init__.py` & `psychoanalyze-0.4.3/psychoanalyze/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import pandas as pd
 import numpy as np
 from psychoanalyze import (
     schemas,
     sessions,
-    blocks,
     points,
     plot,
     data,
     trials,
+    blocks,
     weber,
     strength_duration,
     subjects,
     stimulus,
     simulate,
 )
+from psychoanalyze.dashboard import layout
 
 pd.options.plotting.backend = "plotly"
 
-__version__ = "0.4.0"
+__version__ = "0.4.3"
 
 __all__ = [
     "schemas",
     "plot",
     "data",
     "trial",
     "blocks",
     "sessions",
     "weber",
     "points",
-    "trials",
     "blocks",
+    "trials",
     "strength_duration",
     "subjects",
     "stimulus",
     "simulate",
+    "layout",
 ]
 
 # def curve(trials: pd.DataFrame) -> pd.Series:
 #     """Arrange *method of constant stimuli* performance curves using trial data"""
 #     df = trials.groupby("x").mean().rename(columns={"Result": "Hit Rate"})
 #     return df
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/blocks.py` & `psychoanalyze-0.4.3/psychoanalyze/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,28 @@
 from scipy.stats import logistic
 from scipy.special import logit, expit
 import psychoanalyze as pa
 import plotly.express as px
 import os
 import pathlib
 from sklearn.linear_model import LogisticRegression
+import pandera as pr
+from pandera.typing import DataFrame, Series
+from typing import Any, cast
 
 
 dims = ["Amp2", "Width2", "Freq2", "Dur2", "Active Channels", "Return Channels"]
 index_levels = dims
 
 
+class Blocks(pr.DataFrameModel):
+    slope: float
+    threshold: float
+
+
 def add_posterior(data, posterior):
     return pd.concat(
         [data, posterior],
         keys=["Observed", "Posterior"],
         names=["Type"],
     ).reset_index()
 
@@ -47,28 +55,14 @@
     return df
 
 
 def get_fit_param(fit: pd.DataFrame, name: str):
     return fit.loc[name, "50%"]
 
 
-def from_points(points: pd.DataFrame, dim=None):
-    levels = pa.schemas.block_index_levels
-    if dim == "Amp":
-        levels = levels + ["Width1"]
-        df = points.groupby(levels).apply(pa.points.to_block)
-        return df[df["n Levels"] > 1].drop(columns="Dimension")
-    return points.groupby(levels).apply(pa.points.to_block)
-
-
-def from_trials(trials: pd.Series) -> pd.Series:
-    points = pa.points.from_trials(trials)
-    return from_points(points.reset_index())
-
-
 def dimensions(points, dims=None):
     if dims is None:
         return pa.points.dimension(points)
     return points.groupby(
         [dim for dim in list(points.index.names) if dim not in dims]
     ).apply(pa.points.dimension)
 
@@ -78,15 +72,15 @@
         return points.groupby(pa.schemas.block_index_levels).apply(pa.points.fit)
     else:
         return pd.DataFrame(
             {"Threshold": [], "Fixed Magnitude": [], "Dimension": []},
             index=pd.MultiIndex.from_frame(
                 pd.DataFrame(
                     {
-                        "Monkey": [],
+                        "Subject": [],
                         "Date": [],
                         "Amp2": [],
                         "Width2": [],
                         "Freq2": [],
                         "Dur2": [],
                         "Active Channels": [],
                         "Return Channels": [],
@@ -109,57 +103,53 @@
 
 
 def load_cached(data_path):
     channel_config = ["Active Channels", "Return Channels"]
     blocks = pd.read_csv(data_path / "blocks.csv", parse_dates=["Date"]).set_index(
         pa.sessions.dims + pa.stimulus.ref_dims + channel_config
     )
-    blocks["Day"] = days(blocks, pa.subjects.load(data_path))
+    blocks["Block"] = days(blocks, pa.subjects.load(data_path))
     return blocks
 
 
-def load(data_path=pathlib.Path("data"), monkey=None, day=None, dim=None):
+def load(data_path=pathlib.Path("data"), Subject=None, day=None, dim=None):
     blocks_path = data_path / "blocks.csv"
     if os.path.exists(blocks_path):
         blocks = load_cached(data_path)
-        if monkey:
+        if Subject:
             if day:
-                blocks = blocks[blocks["Day"] == day]
+                blocks = blocks[blocks["Block"] == day]
             else:
-                blocks = blocks.xs(monkey, drop_level=False)
+                blocks = blocks.xs(Subject, drop_level=False)
         blocks = blocks[blocks["n Levels"] > 1]
         return blocks
-    else:
-        blocks = from_trials(pa.trials.load(data_path))
-        blocks.to_csv(blocks_path)
-        return blocks
 
 
 def fixed_magnitudes(points):
     return points.groupby(pa.schemas.block_index_levels).agg(pa.points.fixed_magnitude)
 
 
 def days(blocks, intervention_dates):
-    blocks = blocks.join(intervention_dates, on="Monkey")
+    blocks = blocks.join(intervention_dates, on="Subject")
     days = (blocks.index.get_level_values("Date") - blocks["Surgery Date"]).dt.days
     days.name = "Days"
     return days
 
 
 def n_trials(trials):
-    session_cols = ["Monkey", "Date"]
+    session_cols = ["Subject", "Date"]
     ref_stim_cols = ["Amp2", "Width2", "Freq2", "Dur2"]
     channel_config = ["Active Channels", "Return Channels"]
     return trials.groupby(session_cols + ref_stim_cols + channel_config)[
         "Result"
     ].count()
 
 
 def read_fit(path, block):
-    session_cols = ["Monkey", "Date"]
+    session_cols = ["Subject", "Date"]
     ref_stim_cols = ["Amp2", "Width2", "Freq2", "Dur2"]
     channel_config = ["Active Channels", "Return Channels"]
     fits = pd.read_csv(
         path,
         index_col=session_cols + ref_stim_cols + channel_config,
         parse_dates=["Date"],
     )
@@ -179,19 +169,19 @@
     return blocks["Experiment Type"]
 
 
 def isValid(block):
     return any(block["Hit Rate"] > 0.5) & any(block["Hit Rate"] < 0.5)
 
 
-def monkey_counts(data):
+def Subject_counts(data):
     summary = (
-        data.index.get_level_values("Monkey").value_counts().rename("Total Blocks")
+        data.index.get_level_values("Subject").value_counts().rename("Total Blocks")
     )
-    summary.index.name = "Monkey"
+    summary.index.name = "Subject"
     return summary
 
 
 def model_predictions(intensity_choices, k, x_0=0.0):
     return pd.Series(
         [1 / (1 + np.exp(-k * (x - x_0))) for x in intensity_choices],
         index=intensity_choices,
@@ -204,21 +194,26 @@
         fit.predict_proba(pd.DataFrame({"Intensity": intensity_choices}))[:, 1],
         name="Hit Rate",
         index=pd.Index(intensity_choices, name="Intensity"),
     )
 
 
 def get_fit(trials):
-    return LogisticRegression().fit(trials[["Intensity"]], trials["Result"])
-
-
-def fit_params(fit):
+    fit = LogisticRegression().fit(trials[["Intensity"]], trials["Result"])
     return pd.Series(
         {
             "slope": fit.coef_[0][0],
             "intercept": fit.intercept_[0],
         }
     )
 
 
 def generate_trials(n_trials: int, model_params: dict[str, float]) -> pd.Series:
     return pa.trials.moc_sample(n_trials, model_params)
+
+
+def from_points(points: DataFrame[pa.points.Points]) -> DataFrame[Blocks]:
+    return cast(DataFrame[Blocks], pd.DataFrame({"Block": []}))
+
+
+def from_trials(trials: Series[Any]) -> DataFrame[Blocks]:
+    return from_points(pa.points.from_trials(trials))
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/data.py` & `psychoanalyze-0.4.3/psychoanalyze/data.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.0/psychoanalyze/layout.py` & `psychoanalyze-0.4.3/psychoanalyze/dashboard/layout.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,301 +1,249 @@
 import dash_bootstrap_components as dbc
-from dash import html, dcc
-import psychoanalyze as pa
-import dash_daq as daq
-import plotly.express as px
-import pandas as pd
-
-defaults = {
-    "session": {"sessions": 1, "trials": 100, "subjects": 1},
-    "param": {"thresh": 0, "scale": 1, "gamma": 0, "lambda": 0},
-    "x_min": {"x_min": -3},
-    "x_max": {"x_max": 3},
-}
-
-
-def label(type, param):
-    labels = {
-        "param": f"{param}",
-        "session": f"{param}",
-        "x_min": "Min: ",
-        "x_max": "Max: ",
-    }
-    return labels[type]
-
-
-def input_pair(type, param, default_value):
-    _label = label(type, param)
-    return dbc.InputGroup(
-        [
-            dbc.Label(_label),
-            dbc.Input(id=param, value=default_value, type="number"),
-        ]
-    )
-
-
-def input_group(type):
-    return [input_pair(type, key, value) for key, value in defaults[type].items()]
-
-
-session_inputs = input_group("session")
-param_inputs = input_group("param")
-x_min_input = input_group("x_min")
-x_max_input = input_group("x_max")
+from dash import html, dcc, dash_table
 
-threshold_column = dbc.Col(
+
+experiment_params = html.Div(
     [
-        dcc.Graph(id="time-thresholds"),
-        dbc.Table(id="thresh-data"),
+        html.H4("Experimental Design"),
+        dbc.InputGroup(
+            [
+                dbc.Input(id="n-trials", type="number", value=50),
+                dbc.InputGroupText("trials per block"),
+            ]
+        ),
+        dbc.InputGroup(
+            [
+                dbc.Input(id="n-subjects", type="number", value=2),
+                dbc.InputGroupText("subjects"),
+            ],
+            class_name="mb-4",
+        ),
     ]
 )
 
 
-def points_column(data):
-    return dbc.Col(
-        [
-            dcc.Graph(figure=pa.points.plot(data), id="psych-plot"),
-        ],
-    )
-
-
-diff_thresh_column = dbc.Col(
-    [
-        dcc.Graph(id="difference-thresholds"),
-        html.P(id="weber-fraction"),
-    ],
-)
-controls = dbc.Col(
+psi_params = html.Div(
     [
-        dbc.Card(
-            dbc.CardBody(
-                [html.H4("Entity Counts", className="card-title")] + session_inputs
-            )
-        ),
-        dbc.Card(
-            dbc.CardBody(
-                [html.H4("Simulated Params", className="card-title")] + param_inputs
-            ),
+        html.H4("Psychometric Function"),
+        dcc.Dropdown(
+            id="f",
+            options=[{"label": "Logistic (expit)", "value": "expit"}],
+            value="expit",
         ),
-        dbc.Card(
-            dbc.CardBody(
-                [html.H4("Visible Range", className="card-title")]
-                + x_min_input
-                + x_max_input
-            ),
+        dbc.InputGroup(
+            [
+                dbc.InputGroupText("intercept"),
+                dbc.Input(id="x_0", type="number", value=50.0, step=0.1),
+            ],
+        ),
+        dbc.InputGroup(
+            [
+                dbc.InputGroupText("slope"),
+                dbc.Input(id="model-k", type="number", value=1, step=0.1),
+            ]
+        ),
+        dbc.InputGroup(
+            [
+                dbc.InputGroupText("guess rate"),
+                dbc.Input(id="gamma", type="number", value=0.0, step=0.1),
+            ],
         ),
+        dbc.InputGroup(
+            [
+                dbc.InputGroupText("lapse rate"),
+                dbc.Input(id="lambda", type="number", value=0.0, step=0.1),
+            ],
+            class_name="mb-3",
+        ),
+    ]
+)
+
+component_column = dbc.Col(
+    [
+        html.H3("Simulation Parameters"),
+        experiment_params,
+        psi_params,
     ],
-    width=2,
+    width=3,
 )
 
+upload_component = dcc.Upload(
+    """Upload your own data -
+                        drag and drop or click to open file browser
+                        """,
+    id="upload-data",
+    style={
+        "width": "100%",
+        "height": "60px",
+        "lineHeight": "60px",
+        "borderWidth": "1px",
+        "borderStyle": "dashed",
+        "borderRadius": "5px",
+        "textAlign": "center",
+    },
+    multiple=True,
+)
 
-def simulation_tab(points):
-    return dbc.Tab(
-        [
-            dbc.Row(
-                [
-                    dbc.Col(
-                        [
-                            dbc.Label("n trials"),
-                            dbc.Input(type="number", value=1, id="n-trials"),
-                        ],
-                        width=1,
-                        align="center",
-                    ),
-                    dbc.Col(
-                        [
-                            points_column(points),
-                        ],
-                        width=6,
-                        align="center",
-                    ),
-                    # dbc.Col(
-                    #     [
-                    #         dash_table.DataTable(
-                    #             points.reset_index().to_dict("records"),
-                    #             id="psych-table",
-                    #         ),
-                    #     ],
-                    #     width=1,
-                    #     align="center",
-                    # ),
-                ],
-                justify="center",
+dataset_component = dcc.Dropdown(
+    options=[
+        {
+            "label": html.Span(
+                ["Schlichenmeyer et al. 2022"], style={"color": "black"}
             ),
-            # dbc.Row(pa.plot.strength_duration()),
-        ],
-        label="Simulation",
-    )
-
-
-sd_plots = [
-    dbc.Row(
-        [
-            dbc.Col(
-                dcc.Graph(
-                    # figure=pa.plot.strength_duration(
-                    #     data=pa.strength_duration.from_blocks(
-                    #         pa.blocks.load(), dim=dim
-                    #     ),
-                    #     dim=dim,
-                    #     plot_type="inverse",
-                    # )
-                    figure=px.scatter()
-                )
-            )
-            for dim in ["Amp", "Width"]
-        ]
-    )
-    for view in ["inverse", "linear"]
-]
-
-sessions = pd.read_csv("data/trials.csv")[["Monkey", "Date"]].drop_duplicates()
-
-
-def detection_tab(experiment_points, blocks):
-    return dbc.Tab(
-        dbc.Tabs(
+            "value": "schlich2022",
+        }
+    ],
+    placeholder="Select an open dataset...",
+    id="dataset",
+)
+
+empirical_data_components = html.Div(
+    [
+        dbc.Row(
             [
-                dbc.Tab(
-                    dbc.Row(
-                        [
-                            dbc.Col(
-                                dcc.Graph(figure=pa.plot.counts(sessions), id="counts")
-                            ),
-                            dbc.Col(
-                                dcc.Graph(figure=pa.plot.counts(sessions, dim="Width"))
-                            ),
-                        ],
-                    ),
-                    label="Counts",
-                ),
-                dbc.Tab(sd_plots, label="Strength-Duration Plots", tab_id="sd"),
-                dbc.Tab(
-                    dbc.Row(
-                        [
-                            dbc.Col(
-                                dcc.Graph(
-                                    # figure=pa.plot.ecdf(blocks),
-                                    id="ecdf_g_l",
-                                )
-                            ),
-                            # dbc.Col(
-                            #     dcc.Graph(
-                            #         figure=px.ecdf(blocks, x="width"),
-                            #         id="ecdf_amp",
-                            #     )
-                            # ),
-                            dbc.Col(
-                                dcc.Graph(
-                                    # figure=px.ecdf(blocks, x="Threshold"),
-                                    id="ecdf_pw"
-                                )
-                            ),
-                        ]
-                    ),
-                    label="eCDF",
-                ),
-                dbc.Tab(
-                    dbc.Row(
-                        [
-                            dbc.Col(
-                                dcc.Graph(
-                                    figure=pa.points.plot(experiment_points),
-                                    id="points",
-                                )
-                            ),
-                            dbc.Col(
-                                [
-                                    dbc.Button("Fit curves", id="fit"),
-                                    pa.points.datatable(experiment_points),
-                                ],
-                                width=2,
-                                align="center",
-                            ),
-                        ]
-                    ),
-                    label="Single Block",
-                ),
-            ],
-            active_tab="sd",
+                dbc.Col(upload_component),
+                dbc.Col(dataset_component),
+            ]
         ),
-        label="Detection",
-    )
+    ]
+)
+
+psi_tab = dbc.Tab(
+    tab_id="psi-tab",
+    label="Psychometric Function",
+    activeTabClassName="fw-bold fst-italic",
+)
+
+ecdf_tab = dbc.Tab(
+    label="eCDF",
+    tab_id="ecdf-tab",
+)
+
+time_series_tab = dbc.Tab(
+    tab_id="time-series-tab",
+    label="Time Series",
+    activeTabClassName="fw-bold fst-italic",
+)
 
+sd_tab = dbc.Tab(
+    label="Strength-Duration",
+    tab_id="sd-tab",
+)
 
-discrimination_tab = dbc.Tab(
+plot_tabs = dbc.Col(
     [
+        empirical_data_components,
+        dbc.Row(
+            dbc.Tabs(
+                [
+                    psi_tab,
+                    ecdf_tab,
+                    time_series_tab,
+                    sd_tab,
+                ],
+                active_tab="psi-tab",
+                id="plot-tabs",
+            ),
+            class_name="my-4",
+        ),
         dbc.Row(
             [
                 dbc.Col(
-                    daq.BooleanSwitch(
-                        on=True,
-                        label="Trendline",
-                        labelPosition="top",
-                        id="trendline",
-                    ),
-                ),
-                dbc.Col(
-                    dbc.RadioItems(
-                        options=[
-                            {"label": "Log Scale", "value": "Log Scale"},
-                            {"label": "Linear Scale", "value": "Linear Scale"},
-                        ],
-                        value="Log Scale",
-                        id="log-scale",
-                    ),
-                ),
-                dbc.Col(
-                    dbc.RadioItems(
-                        options=[
-                            {
-                                "label": "Group by x values",
-                                "value": "Group by x values",
-                            },
-                            {"label": "Show all blocks", "value": None},
-                        ],
-                        value=None,
-                        id="group-x",
-                    )
+                    [
+                        dcc.Graph(id="plot"),
+                    ],
+                    width=7,
                 ),
                 dbc.Col(
-                    dbc.RadioItems(
-                        options=[
-                            {"label": "Histogram", "value": "Histogram"},
-                            {"label": "Off", "value": "Off"},
-                        ],
-                        value="Histogram",
-                        id="marginal",
-                    )
+                    [
+                        dash_table.DataTable(
+                            id="table",
+                            columns=[
+                                {
+                                    "name": "Subject",
+                                    "id": "Subject",
+                                },
+                                {
+                                    "name": "Block",
+                                    "id": "Block",
+                                },
+                                {
+                                    "name": "Slope",
+                                    "id": "slope",
+                                    "type": "numeric",
+                                    "format": dash_table.Format.Format(
+                                        precision=2,
+                                        scheme=dash_table.Format.Scheme.fixed,
+                                    ),
+                                },
+                                {
+                                    "name": "Threshold",
+                                    "id": "Threshold",
+                                    "type": "numeric",
+                                    "format": dash_table.Format.Format(
+                                        precision=2,
+                                        scheme=dash_table.Format.Scheme.fixed,
+                                    ),
+                                },
+                            ],
+                            row_selectable="multi",
+                            style_data={"color": "black"},
+                            style_header={"color": "black"},
+                            page_size=15,
+                        ),
+                    ],
+                    width=4,
                 ),
-                dbc.Col(
-                    dbc.RadioItems(
-                        options=[
-                            {"label": "error bars", "value": "error bars"},
-                            {"label": "off", "value": "off"},
-                        ],
-                        value="error bars",
-                        id="error",
-                    )
+            ]
+        ),
+    ]
+)
+
+layout = dbc.Container(
+    [
+        dbc.NavbarSimple(
+            [
+                dbc.NavItem(
+                    [
+                        dbc.NavLink(
+                            "GitHub",
+                            href="https://github.com/psychoanalyze/psychoanalyze",
+                        ),
+                        html.I(className="bi bi-github"),
+                    ],
+                    className="d-flex align-items-center mx-2",
+                ),
+                dbc.NavItem(
+                    [
+                        dbc.NavLink(
+                            "Docs",
+                            href="https://docs.psychoanalyze.io",
+                        ),
+                        html.I(className="bi bi-book"),
+                    ],
+                    className="d-flex align-items-center mx-2",
                 ),
             ],
+            brand=dbc.Col(
+                [
+                    dbc.Row(html.H1("PsychoAnalyze")),
+                    dbc.Row(
+                        html.P(
+                            "Interactive data simulation & analysis for psychophysics."
+                        )
+                    ),
+                ],
+            ),
+            brand_href="/",
+            class_name="mb-3",
         ),
         dbc.Row(
             [
-                dbc.Col(dcc.Graph(id="weber"), width=6, id="weber-width"),
+                component_column,
+                plot_tabs,
             ]
         ),
+        dcc.Store(id="blocks-store"),
+        dcc.Store(id="points-store"),
     ],
-    label="Discrimination",
 )
-
-
-def experiment_tab(experiment_points, blocks):
-    return dbc.Tab(
-        dbc.Tabs(
-            [
-                detection_tab(experiment_points, blocks),
-                discrimination_tab,
-            ]
-        ),
-        label="Experiment",
-    )
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/plot.py` & `psychoanalyze-0.4.3/psychoanalyze/plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 colormap = {"U": "#e41a1c", "Y": "#377eb8", "Z": "#4daf4a"}
 
 
 def thresholds(df):
     df = pa.data.transform_errors(df)
     return px.scatter(
         df,
-        x="Day",
+        x="Block",
         y="50%",
         error_y="err+",
         error_y_minus="err-",
         color="Subject",
         color_discrete_map=colormap,
         template=template,
     )
@@ -51,15 +51,15 @@
         df,
         x="x",
         y=y,
         error_y="err+",
         error_y_minus="err-",
         color=df.get("Subject"),  # or df["Type"],
         color_discrete_map=colormap,
-        symbol=df.get("Day"),
+        symbol=df.get("Block"),
         template=template,
     )
 
 
 def logistic(data):
     df = data.reset_index()
     return px.line(
@@ -95,15 +95,15 @@
     return px.line(
         df,
         x="Intensity",
         y="Hit Rate",
         # error_y="err+",
         # error_y_minus="err-",
         # color=df.get("Subject") or df.get("Type"),
-        # symbol=df.get("Day"),
+        # symbol=df.get("Block"),
         animation_group="Intensity",
         animation_frame="Trial",
         template=template,
     )
 
 
 def posterior_animation(cumulative_draws: pd.DataFrame):
@@ -114,15 +114,15 @@
         x="x",
         y="Hit Rate",
         error_y="err+",
         error_y_minus="err-",
         animation_group="x",
         animation_frame="n",
         color=df.get("Subject"),
-        symbol=df.get("Day"),
+        symbol=df.get("Block"),
         template=template,
     )
 
 
 def difference_thresholds():
     return px.scatter(
         pd.DataFrame(
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/points.py` & `psychoanalyze-0.4.3/psychoanalyze/points.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import pandas as pd
-import cmdstanpy as stan
 import plotly.express as px
 from scipy.stats import binom
 import psychoanalyze as pa
 from dash import dash_table
 import pathlib
 from plotly import graph_objects as go
 import numpy as np
+import pandera as pr
+from pandera.typing import DataFrame, Series
+from typing import cast
+import cmdstanpy as stan
 
 
 index_levels = ["Amp1", "Width1", "Freq1", "Dur1"]
 
 
-def from_trials(trials: pd.Series) -> pd.DataFrame:
-    grouped = trials.groupby(level=trials.index.names)  # type: ignore
-    hits = grouped.sum().rename("Hits")
-    n = grouped.count().rename("n")
-    hr = (hits / n).rename("Hit Rate")
-    return pd.concat([hits, n, hr], axis=1)
+class Points(pr.DataFrameModel):
+    n: int
+    Hits: int
 
 
-def load(data_path=pathlib.Path("data")):
+def from_trials(trials: Series[int]) -> DataFrame[Points]:
+    df = (
+        trials.groupby("Intensity")
+        .agg(["count", "sum"])
+        .rename(columns={"count": "n", "sum": "Hits"})
+    )
+    df["Hit Rate"] = df["Hits"] / df["n"]
+    return cast(DataFrame[Points], df)
+
+
+def load(data_path=pathlib.Path("data")) -> DataFrame[Points]:
     trials = pa.trials.load(data_path)
     return from_trials(trials)
 
 
 def dimension(points):
     amp1, width1 = (
         points.index.get_level_values(param) for param in ["Amp1", "Width1"]
@@ -166,25 +176,18 @@
     if dim == "Amp":
         return points.index.get_level_values("Width1")[0]
     if dim == "Width":
         return points.index.get_level_values("Amp1")[0]
 
 
 def n(trials):
-    return trials.groupby(level=["Day", "Subject"]).count()
+    return trials.groupby(level=["Subject", "Block"]).count()
 
 
 def to_block(points):
-    return pd.Series(
-        {
-            # "Threshold": fit(points),
-            "Dimension": dimension(points),
-            "Fixed Magnitude": fixed_magnitude(points),
-            "n Levels": n(points),
-        }
-    )
+    return points.groupby(level=["Subject", "Block"]).sum()
 
 
 def psi(x: np.ndarray, threshold: float, width: float, gamma: float, lambda_: float):
     return gamma + (1 - gamma - lambda_) / (
         1 + np.exp(-gamma * (x - threshold) / width) ** lambda_
     )
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/schemas.py` & `psychoanalyze-0.4.3/psychoanalyze/schemas.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.0/psychoanalyze/sessions.py` & `psychoanalyze-0.4.3/psychoanalyze/sessions.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         if monkey:
             trials = trials[trials.index.get_level_values("Monkey") == monkey]
         sessions = (
             trials.groupby(["Monkey", "Date"])[["Result"]]
             .count()
             .rename(columns={"Result": "n Trials"})
         )
-    sessions["Day"] = days(sessions, pa.subjects.load(data_path))
+    sessions["Block"] = days(sessions, pa.subjects.load(data_path))
     return sessions
 
 
 def days(sessions: pd.DataFrame, subjects):
     df = sessions.join(subjects, on="Monkey")
     return (
         pd.to_datetime(df.index.get_level_values("Date")) - df["Surgery Date"]
@@ -74,9 +74,9 @@
     n_days: int,
 ) -> pd.Series:
     return pd.concat(
         {
             day: pa.blocks.generate_trials(n_trials, model_params)
             for day in range(n_days)
         },
-        names=["Day"],
+        names=["Block"],
     )
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/simulate.py` & `psychoanalyze-0.4.3/psychoanalyze/simulate.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.0/psychoanalyze/strength_duration.py` & `psychoanalyze-0.4.3/psychoanalyze/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.0/psychoanalyze/subjects.py` & `psychoanalyze-0.4.3/psychoanalyze/subjects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import psychoanalyze as pa
-
+import string
 
 def load(data_path):
     return pd.read_csv(
         data_path / "subjects.csv",
         index_col="Monkey",
         parse_dates=["Surgery Date"],
     )
@@ -19,11 +19,11 @@
     model_params: dict[str, float],
     n_days: int,
     n_subjects: int,
 ) -> pd.Series:
     return pd.concat(
         {
             subj: pa.sessions.generate_trials(n_trials, model_params, n_days)
-            for subj in range(n_subjects)
+            for subj in string.ascii_uppercase[:n_subjects]
         },
         names=["Subject"],
     )
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/trials.py` & `psychoanalyze-0.4.3/psychoanalyze/trials.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from typing import TypedDict
 import pandas as pd
 import numpy as np
 import psychoanalyze as pa
 from pathlib import Path
-from datetime import datetime
 import json
 import pandera as pr
 import random
 
 schema = pr.SeriesSchema(bool, name="Test Trials")
 
 
+class Trials(pr.DataFrameModel):
+    result: int
+
+
 data_path = Path("data/trials.csv")
 
 codes = {False: "Miss", True: "Hit"}
 
 
 def n(trials: pd.Series) -> int:
     return len(trials)
@@ -31,38 +34,16 @@
     hits = pd.Series(
         [generate_hits(100, p) for p in [0.1, 0.2, 0.5, 0.8, 0.9]], name="Hits"
     )
     x = [0, 1, 2, 3, 4]
     return pd.DataFrame({"Hits": hits, "n": [100] * 5}, index=pd.Index(x, name=dim))
 
 
-def generate(n, stim_levels=None):
-    return pa.schemas.trials.validate(
-        pd.DataFrame(
-            {"Result": np.random.binomial(1, 0.5, n)},
-            index=pd.MultiIndex.from_frame(
-                pd.DataFrame(
-                    {
-                        "Monkey": ["Z"] * n,
-                        "Date": [datetime.now()] * n,
-                        "Amp2": [0.0] * n,
-                        "Width2": [0.0] * n,
-                        "Freq2": [0.0] * n,
-                        "Dur2": [0.0] * n,
-                        "Active Channels": [1] * n,
-                        "Return Channels": [1] * n,
-                        "Amp1": random.choices(list(range(8)), k=n),
-                        "Width1": [0.0] * n,
-                        "Freq1": [0.0] * n,
-                        "Dur1": [0.0] * n,
-                    }
-                )
-            ),
-        )
-    )
+def generate(n: int) -> pd.Series:
+    return pd.Series(np.random.binomial(1, 0.5, n),dtype=int, name="Result")
 
 
 def load(data_path: Path = Path("data")):
     return pa.schemas.trials.validate(
         pd.read_csv(
             data_path / "trials.csv",
             index_col=pa.schemas.points_index_levels,
@@ -85,15 +66,15 @@
     data_dict = df.to_dict(orient="split")
     data_dict["index_names"] = pa.schemas.points_index_levels
     return json.dumps(data_dict)
 
 
 def normalize(trials):
     return {
-        "Session": trials[["Monkey", "Day"]].drop_duplicates(),
+        "Session": trials[["Monkey", "Block"]].drop_duplicates(),
         "Reference Stimulus": trials[["Amp2", "Width2", "Freq2", "Dur2"]],
         "Channel Config": trials[["Active Channels", "Return Channels"]],
         "Test Stimulus": trials[["Amp1", "Width1", "Freq1", "Dur1"]],
     }
 
 
 def result(p: float) -> bool:
```

### Comparing `psychoanalyze-0.4.0/psychoanalyze/weber.py` & `psychoanalyze-0.4.3/psychoanalyze/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.0/pyproject.toml` & `psychoanalyze-0.4.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,73 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.4.0"
+version = "0.4.3"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.11.3"
-pandas = "^1.4.2"
-black = "^23.3.0"
-datatest = "^0.11.1"
-pytest = "^7.2.2"
-scipy = "^1.8.0"
-numpy = "^1.23.4"
-mkdocstrings = "^0.18.1"
-plotly = "^5.14.1"
+python = "3.11.4"
+pandas = "^2.0.2"
+scipy = "^1.10.1"
+numpy = "^1.25.0"
 dash-bootstrap-components = "^1.4.1"
-pytest-sugar = "^0.9.6"
-pytest-mock = "^3.7.0"
-statsmodels = "^0.13.2"
-mypy = "^1.2.0"
-hypothesis = "^6.70.0"
-bandit = "^1.7.4"
-safety = "^2.0.0"
-mkdocs-material = "^8.3.9"
-tabulate = "^0.8.10"
-pandera = {extras = ["mypy"], version = "^0.14.5"}
-pre-commit = "^2.20.0"
+statsmodels = "^0.14.0"
 dash-daq = "^0.5.0"
-pandas-stubs = "^1.5.3.230321"
-cmdstanpy = "^1.0.8"
-dbt-core = "^1.5.1"
 dash = "^2.10.2"
 dbt-duckdb = "^1.5.1"
-ydata-profiling = "^4.1.2"
-nbformat = "^5.8.0"
-gunicorn = "^20.1.0"
-shandy-sqlfmt = {extras = ["jinjafmt"], version = "^0.18.0"}
 scikit-learn = "^1.2.2"
-ipywidgets = "^8.0.6"
-conda-lock = "^2.0.0"
 bambi = "^0.11.0"
-python-semantic-release = "7.28.1"
-snakeviz = "^2.2.0"
-
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
-ipykernel = "^6.22.0"
-
+pymc = "5.5.0"
+mypy = "^1.3.0"
+cmdstanpy = "^1.1.0"
+pandas-stubs = "^2.0.2.230605"
+pandera = {extras = ["mypy"], version = "^0.15.1"}
+pytest = "^7.3.2"
+hypothesis = "^6.79.0"
+datatest = "^0.11.1"
+pytest-mock = "^3.11.1"
+gunicorn = "^20.1.0"
 
-[tool.poetry.group.ci.dependencies]
-ruff = "^0.0.261"
+[tool.poetry.scripts]
+psychoanalyze = "psychoanalyze.__main__:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = [
     "psychoanalyze/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "main"
 build_command = "poetry build"
 major_on_zero = true
 
-[tool.pytest.ini_options]
-filterwarnings = [
-    "ignore::DeprecationWarning",
-    "ignore::FutureWarning"
-]
-
 [tool.bandit]
 targets = ["psychoanalyze/"]
 skips = ["B311"]
 
 [tool.mypy]
 exclude = [
     'tests',
+    'target'
 ]
+plugins = ['pandera.mypy']
 
 [[tool.mypy.overrides]]
 module = [
     'dash',
     'plotly',
     'dash_bootstrap_components',
     'plotly.express',
     'scipy.stats',
     'scipy.special',
     'sklearn.linear_model',
     'dash_daq',
-    'datatest'
+    'datatest',
+    'bambi',
+    'hypothesis'
 ]
 ignore_missing_imports = true
```

