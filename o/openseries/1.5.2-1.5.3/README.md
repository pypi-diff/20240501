# Comparing `tmp/openseries-1.5.2.tar.gz` & `tmp/openseries-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openseries-1.5.2.tar", max compression
+gzip compressed data, was "openseries-1.5.3.tar", max compression
```

## Comparing `openseries-1.5.2.tar` & `openseries-1.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1521 2024-04-16 08:07:42.908003 openseries-1.5.2/LICENSE.md
--rw-r--r--   0        0        0    42091 2024-04-16 08:07:42.908003 openseries-1.5.2/README.md
--rw-r--r--   0        0        0       41 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/__init__.py
--rw-r--r--   0        0        0    72468 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/_common_model.py
--rw-r--r--   0        0        0     3299 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/_risk.py
--rw-r--r--   0        0        0    12377 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/datefixer.py
--rw-r--r--   0        0        0    73772 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/frame.py
--rw-r--r--   0        0        0     1807 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/load_plotly.py
--rw-r--r--   0        0        0      178 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/plotly_captor_logo.json
--rw-r--r--   0        0        0     1429 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/plotly_layouts.json
--rw-r--r--   0        0        0    28312 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/series.py
--rw-r--r--   0        0        0    13549 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/simulation.py
--rw-r--r--   0        0        0     7597 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/types.py
--rw-r--r--   0        0        0     2664 2024-04-16 08:07:42.908003 openseries-1.5.2/pyproject.toml
--rw-r--r--   0        0        0    43661 1970-01-01 00:00:00.000000 openseries-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-01 19:28:47.534606 openseries-1.5.3/LICENSE.md
+-rw-r--r--   0        0        0    42009 2024-05-01 19:28:47.534606 openseries-1.5.3/README.md
+-rw-r--r--   0        0        0       41 2024-05-01 19:28:47.534606 openseries-1.5.3/openseries/__init__.py
+-rw-r--r--   0        0        0    72469 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/_common_model.py
+-rw-r--r--   0        0        0     3300 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/_risk.py
+-rw-r--r--   0        0        0    12378 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/datefixer.py
+-rw-r--r--   0        0        0    74019 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/frame.py
+-rw-r--r--   0        0        0     1808 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/load_plotly.py
+-rw-r--r--   0        0        0      178 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/plotly_captor_logo.json
+-rw-r--r--   0        0        0     1429 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/plotly_layouts.json
+-rw-r--r--   0        0        0    28313 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/series.py
+-rw-r--r--   0        0        0    13905 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/simulation.py
+-rw-r--r--   0        0        0     7597 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/types.py
+-rw-r--r--   0        0        0     2665 2024-05-01 19:28:47.538606 openseries-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0    43579 1970-01-01 00:00:00.000000 openseries-1.5.3/PKG-INFO
```

### Comparing `openseries-1.5.2/LICENSE.md` & `openseries-1.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openseries-1.5.2/README.md` & `openseries-1.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -249,14 +249,15 @@
 | `jensen_alpha`          | `OpenFrame` | Calculates [Jensen's Alpha](https://www.investopedia.com/terms/j/jensensmeasure.asp) of an asset relative a market.                                                                |
 | `tracking_error_func`   | `OpenFrame` | Calculates the [tracking errors](https://www.investopedia.com/terms/t/trackingerror.asp) relative to a selected series in the OpenFrame.                                           |
 | `info_ratio_func`       | `OpenFrame` | Calculates the [information ratios](https://www.investopedia.com/terms/i/informationratio.asp) relative to a selected series in the OpenFrame.                                     |
 | `capture_ratio_func`    | `OpenFrame` | Calculates up, down and up/down [capture ratios](https://www.investopedia.com/terms/d/down-market-capture-ratio.asp) relative to a selected series.                                |
 | `rolling_info_ratio`    | `OpenFrame` | Returns a pandas.DataFrame with the rolling [information ratio](https://www.investopedia.com/terms/i/informationratio.asp) between two series.                                     |
 | `rolling_beta`          | `OpenFrame` | Returns a pandas.DataFrame with the rolling [Beta](https://www.investopedia.com/terms/b/beta.asp) of an asset relative a market.                                                   |
 | `rolling_corr`          | `OpenFrame` | Calculates and adds a series of rolling [correlations](https://www.investopedia.com/terms/c/correlation.asp) between two other series.                                             |
+| `correl_matrix`         | `OpenFrame` | Returns a `pandas.DataFrame` with a correlation matrix.                                                                                                                            |
 | `ewma_risk`             | `OpenFrame` | Returns a `pandas.DataFrame` with volatility and correlation based on [Exponentially Weighted Moving Average](https://www.investopedia.com/articles/07/ewma.asp).                  |
 
 ### Methods that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Method                             | Applies to                    | Description                                                                                                                                              |
 |:-----------------------------------|:------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `align_index_to_local_cdays`       | `OpenTimeSeries`, `OpenFrame` | Aligns the series dates to a business calendar. Defaults to Sweden.                                                                                      |
@@ -299,15 +300,14 @@
 | `max_drawdown`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Maximum drawdown](https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp).                                                                                                                                      |
 | `max_drawdown_cal_year` | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Max drawdown in a single calendar year.                                                                                                                                                                                 |
 | `positive_share`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The share of percentage changes that are positive.                                                                                                                                                                      |
 | `vol_from_var`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Implied annualized volatility from the Downside VaR using the assumption that returns are normally distributed.                                                                                                         |
 | `skew`                  | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Skew](https://www.investopedia.com/terms/s/skewness.asp) of the return distribution.                                                                                                                                   |
 | `kurtosis`              | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Kurtosis](https://www.investopedia.com/terms/k/kurtosis.asp) of the return distribution.                                                                                                                               |
 | `z_score`               | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Z-score](https://www.investopedia.com/terms/z/zscore.asp) as (last return - mean return) / standard deviation of returns.                                                                                              |
-| `correl_matrix`         | `pandas.DataFrame`       | `OpenFrame`                   | A correlation matrix.                                                                                                                                                                                                   |
 
 ### Methods below are identical to the Numerical Properties above.
 
 _They are simply methods that take different date or length inputs to return the
 properties for subset periods._
 
 | Method                    | type                     | Applies to                    | Description                                                                                                                                                                                                                                                    |
```

### Comparing `openseries-1.5.2/openseries/_common_model.py` & `openseries-1.5.3/openseries/_common_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defining the _CommonModel class."""
+
 from __future__ import annotations
 
 import datetime as dt
 from inspect import stack
 from json import dump
 from math import ceil
 from pathlib import Path
```

### Comparing `openseries-1.5.2/openseries/_risk.py` & `openseries-1.5.3/openseries/_risk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Various risk related functions."""
+
 from __future__ import annotations
 
 from math import ceil
 from typing import Union, cast
 
 from numpy import (
     divide,
```

### Comparing `openseries-1.5.2/openseries/datefixer.py` & `openseries-1.5.3/openseries/datefixer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Date related utilities."""
+
 from __future__ import annotations
 
 import datetime as dt
 from typing import Optional, Union, cast
 
 from dateutil.relativedelta import relativedelta
 from holidays import (
```

### Comparing `openseries-1.5.2/openseries/frame.py` & `openseries-1.5.3/openseries/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1930,16 +1930,17 @@
         axis="columns",
     )
     line_df["sharpe"] = line_df.ret / line_df.stdev
 
     limit_small = 0.0001
     line_df = line_df.mask(line_df.abs() < limit_small, 0.0)
     line_df["text"] = line_df.apply(
-        lambda c: "<br>".join(
-            [f"{c[nm]:.1%} - {nm}" for nm in eframe.columns_lvl_zero],
+        lambda c: "<br><br>Weights:<br>"
+        + "<br>".join(
+            [f"{c[nm]:.1%}  {nm}" for nm in eframe.columns_lvl_zero],
         ),
         axis="columns",
     )
 
     if tweak:
         limit_tweak = 0.001
         line_df["stdev_diff"] = line_df.stdev.pct_change()
@@ -2034,30 +2035,28 @@
 
     Returns
     -------
     DataFrame
         The data prepared with mean returns, volatility and weights
 
     """
-    txt = "<br>".join(
+    txt = "<br><br>Weights:<br>" + "<br>".join(
         [
-            f"{wgt:.1%} - {nm}"
+            f"{wgt:.1%}  {nm}"
             for wgt, nm in zip(
                 cast(list[float], assets.weights),
                 assets.columns_lvl_zero,
             )
         ],
     )
 
-    opt_text = "<br>".join(
-        [
-            f"{wgt:.1%} - {nm}"
-            for wgt, nm in zip(optimized[3:], assets.columns_lvl_zero)
-        ],
-    )
+    opt_text_list = [
+        f"{wgt:.1%}  {nm}" for wgt, nm in zip(optimized[3:], assets.columns_lvl_zero)
+    ]
+    opt_text = "<br><br>Weights:<br>" + "<br>".join(opt_text_list)
     vol: Series[float] = assets.vol
     plotframe = DataFrame(
         data=[
             assets.arithmetic_ret,
             vol,
             Series(
                 data=[""] * assets.item_count,
@@ -2162,15 +2161,18 @@
     if line_frame is not None:
         returns.extend(list(line_frame.loc[:, "ret"]))
         risk.extend(list(line_frame.loc[:, "stdev"]))
         figure.add_scatter(
             x=line_frame.loc[:, "stdev"],
             y=line_frame.loc[:, "ret"],
             text=line_frame.loc[:, "text"],
-            hovertemplate="%{text}<br>Return %{y}<br>Vol %{x}",
+            xhoverformat=".2%",
+            yhoverformat=".2%",
+            hovertemplate="Return %{y}<br>Vol %{x}%{text}",
+            hoverlabel_align="right",
             line={"width": 2.5, "dash": "solid"},
             mode="lines",
             name="Efficient frontier",
         )
 
     colorway = cast(dict[str, list[str]], fig["layout"]).get("colorway")[
         : len(point_frame.columns)
@@ -2178,19 +2180,20 @@
 
     if point_frame is not None:
         for col, clr in zip(point_frame.columns, colorway):
             returns.extend([point_frame.loc["ret", col]])
             risk.extend([point_frame.loc["stdev", col]])
             figure.add_scatter(
                 x=[point_frame.loc["stdev", col]],
-                xhoverformat=".2%",
                 y=[point_frame.loc["ret", col]],
+                xhoverformat=".2%",
                 yhoverformat=".2%",
                 hovertext=[point_frame.loc["text", col]],
-                hoverinfo="x+y+text+name",
+                hovertemplate=("Return %{y}<br>Vol %{x}%{hovertext}"),
+                hoverlabel_align="right",
                 marker={"size": 20, "color": clr},
                 mode=point_frame_mode,
                 name=col,
                 text=col,
                 textfont={"size": 14},
                 textposition="bottom center",
             )
```

### Comparing `openseries-1.5.2/openseries/load_plotly.py` & `openseries-1.5.3/openseries/load_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Function to load plotly layout and configuration from local json file."""
+
 from __future__ import annotations
 
 from json import load
 from logging import warning
 from pathlib import Path
 
 import requests
```

### Comparing `openseries-1.5.2/openseries/plotly_layouts.json` & `openseries-1.5.3/openseries/plotly_layouts.json`

 * *Files identical despite different names*

### Comparing `openseries-1.5.2/openseries/series.py` & `openseries-1.5.3/openseries/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defining the OpenTimeSeries class."""
+
 from __future__ import annotations
 
 import datetime as dt
 from copy import deepcopy
 from logging import warning
 from typing import Any, Optional, TypeVar, Union, cast
```

### Comparing `openseries-1.5.2/openseries/simulation.py` & `openseries-1.5.3/openseries/simulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defining the ReturnSimulation class."""
+
 from __future__ import annotations
 
 import datetime as dt
 from typing import Optional, cast
 
 from numpy import multiply, sqrt
 from numpy.random import PCG64, Generator, SeedSequence
@@ -72,30 +73,27 @@
         This is the probability of a jump happening at each point in time
     jumps_sigma: NonNegativeFloat, default: 0.0
         This is the volatility of the jump size
     jumps_mu: float, default: 0.0
         This is the average jump size
     seed: int, optional
         Seed for random process initiation
-    randomizer: numpy.random.Generator, optional
-        Random process generator
 
     """
 
     number_of_sims: PositiveInt
     trading_days: PositiveInt
     trading_days_in_year: DaysInYearType
     mean_annual_return: float
     mean_annual_vol: PositiveFloat
     dframe: DataFrame
     jumps_lamda: NonNegativeFloat = 0.0
     jumps_sigma: NonNegativeFloat = 0.0
     jumps_mu: float = 0.0
     seed: Optional[int] = None
-    randomizer: Optional[Generator] = None
 
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         validate_assignment=True,
         revalidate_instances="always",
     )
 
@@ -155,14 +153,15 @@
         cls: type[ReturnSimulation],
         number_of_sims: PositiveInt,
         mean_annual_return: float,
         mean_annual_vol: PositiveFloat,
         trading_days: PositiveInt,
         seed: int,
         trading_days_in_year: DaysInYearType = 252,
+        randomizer: Optional[Generator] = None,
     ) -> ReturnSimulation:
         """
         Create a Normal distribution simulation.
 
         Parameters
         ----------
         number_of_sims: PositiveInt
@@ -174,49 +173,52 @@
         mean_annual_vol: PositiveFloat
             Mean standard deviation
         seed: int
             Seed for random process initiation
         trading_days_in_year: DaysInYearType,
             default: 252
             Number of trading days used to annualize
+        randomizer: numpy.random.Generator, optional
+            Random process generator
 
         Returns
         -------
         ReturnSimulation
             Normal distribution simulation
 
         """
-        cls.randomizer = random_generator(seed=seed)
+        if not randomizer:
+            randomizer = random_generator(seed=seed)
 
-        returns = cls.randomizer.normal(
+        returns = randomizer.normal(
             loc=mean_annual_return / trading_days_in_year,
             scale=mean_annual_vol / sqrt(trading_days_in_year),
             size=(number_of_sims, trading_days),
         )
 
         return cls(
             number_of_sims=number_of_sims,
             trading_days=trading_days,
             trading_days_in_year=trading_days_in_year,
             mean_annual_return=mean_annual_return,
             mean_annual_vol=mean_annual_vol,
             dframe=DataFrame(data=returns, dtype="float64"),
             seed=seed,
-            randomizer=cls.randomizer,
         )
 
     @classmethod
     def from_lognormal(
         cls: type[ReturnSimulation],
         number_of_sims: PositiveInt,
         mean_annual_return: float,
         mean_annual_vol: PositiveFloat,
         trading_days: PositiveInt,
         seed: int,
         trading_days_in_year: DaysInYearType = 252,
+        randomizer: Optional[Generator] = None,
     ) -> ReturnSimulation:
         """
         Create a Lognormal distribution simulation.
 
         Parameters
         ----------
         number_of_sims: PositiveInt
@@ -228,25 +230,28 @@
         mean_annual_vol: PositiveFloat
             Mean standard deviation
         seed: int
             Seed for random process initiation
         trading_days_in_year: DaysInYearType,
             default: 252
             Number of trading days used to annualize
+        randomizer: numpy.random.Generator, optional
+            Random process generator
 
         Returns
         -------
         ReturnSimulation
             Lognormal distribution simulation
 
         """
-        cls.randomizer = random_generator(seed=seed)
+        if not randomizer:
+            randomizer = random_generator(seed=seed)
 
         returns = (
-            cls.randomizer.lognormal(
+            randomizer.lognormal(
                 mean=mean_annual_return / trading_days_in_year,
                 sigma=mean_annual_vol / sqrt(trading_days_in_year),
                 size=(number_of_sims, trading_days),
             )
             - 1
         )
 
@@ -254,26 +259,26 @@
             number_of_sims=number_of_sims,
             trading_days=trading_days,
             trading_days_in_year=trading_days_in_year,
             mean_annual_return=mean_annual_return,
             mean_annual_vol=mean_annual_vol,
             dframe=DataFrame(data=returns, dtype="float64"),
             seed=seed,
-            randomizer=cls.randomizer,
         )
 
     @classmethod
     def from_gbm(
         cls: type[ReturnSimulation],
         number_of_sims: PositiveInt,
         mean_annual_return: float,
         mean_annual_vol: PositiveFloat,
         trading_days: PositiveInt,
         seed: int,
         trading_days_in_year: DaysInYearType = 252,
+        randomizer: Optional[Generator] = None,
     ) -> ReturnSimulation:
         """
         Create a Geometric Brownian Motion simulation.
 
         Parameters
         ----------
         number_of_sims: PositiveInt
@@ -284,29 +289,32 @@
             Mean return
         mean_annual_vol: PositiveFloat
             Mean standard deviation
         seed: int
             Seed for random process initiation
         trading_days_in_year: DaysInYearType, default: 252
             Number of trading days used to annualize
+        randomizer: numpy.random.Generator, optional
+            Random process generator
 
         Returns
         -------
         ReturnSimulation
             Geometric Brownian Motion simulation
 
         """
-        cls.randomizer = random_generator(seed=seed)
+        if not randomizer:
+            randomizer = random_generator(seed=seed)
 
         drift = (mean_annual_return - 0.5 * mean_annual_vol**2.0) * (
             1.0 / trading_days_in_year
         )
 
         normal_mean = 0.0
-        wiener = cls.randomizer.normal(
+        wiener = randomizer.normal(
             loc=normal_mean,
             scale=sqrt(1.0 / trading_days_in_year) * mean_annual_vol,
             size=(number_of_sims, trading_days),
         )
 
         returns = drift + wiener
 
@@ -314,29 +322,29 @@
             number_of_sims=number_of_sims,
             trading_days=trading_days,
             trading_days_in_year=trading_days_in_year,
             mean_annual_return=mean_annual_return,
             mean_annual_vol=mean_annual_vol,
             dframe=DataFrame(data=returns, dtype="float64"),
             seed=seed,
-            randomizer=cls.randomizer,
         )
 
     @classmethod
     def from_merton_jump_gbm(
         cls: type[ReturnSimulation],
         number_of_sims: PositiveInt,
         trading_days: PositiveInt,
         mean_annual_return: float,
         mean_annual_vol: PositiveFloat,
         seed: int,
         jumps_lamda: NonNegativeFloat,
         jumps_sigma: NonNegativeFloat = 0.0,
         jumps_mu: float = 0.0,
         trading_days_in_year: DaysInYearType = 252,
+        randomizer: Optional[Generator] = None,
     ) -> ReturnSimulation:
         """
         Create a Merton Jump-Diffusion model simulation.
 
         Parameters
         ----------
         number_of_sims: PositiveInt
@@ -353,36 +361,39 @@
             This is the probability of a jump happening at each point in time
         jumps_sigma: NonNegativeFloat, default: 0.0
             This is the volatility of the jump size
         jumps_mu: float, default: 0.0
             This is the average jump size
         trading_days_in_year: DaysInYearType, default: 252
             Number of trading days used to annualize
+        randomizer: numpy.random.Generator, optional
+            Random process generator
 
         Returns
         -------
         ReturnSimulation
             Merton Jump-Diffusion model simulation
 
         """
-        cls.randomizer = random_generator(seed=seed)
+        if not randomizer:
+            randomizer = random_generator(seed=seed)
 
         normal_mean = 0.0
-        wiener = cls.randomizer.normal(
+        wiener = randomizer.normal(
             loc=normal_mean,
             scale=sqrt(1.0 / trading_days_in_year) * mean_annual_vol,
             size=(number_of_sims, trading_days),
         )
 
         poisson_jumps = multiply(
-            cls.randomizer.poisson(
+            randomizer.poisson(
                 lam=jumps_lamda * (1.0 / trading_days_in_year),
                 size=(number_of_sims, trading_days),
             ),
-            cls.randomizer.normal(
+            randomizer.normal(
                 loc=jumps_mu,
                 scale=jumps_sigma,
                 size=(number_of_sims, trading_days),
             ),
         )
 
         drift = (
@@ -402,15 +413,14 @@
             mean_annual_return=mean_annual_return,
             mean_annual_vol=mean_annual_vol,
             jumps_lamda=jumps_lamda,
             jumps_sigma=jumps_sigma,
             jumps_mu=jumps_mu,
             dframe=DataFrame(data=returns, dtype="float64"),
             seed=seed,
-            randomizer=cls.randomizer,
         )
 
     def to_dataframe(
         self: Self,
         name: str,
         start: Optional[dt.date] = None,
         end: Optional[dt.date] = None,
```

### Comparing `openseries-1.5.2/openseries/types.py` & `openseries-1.5.3/openseries/types.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.2/pyproject.toml` & `openseries-1.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openseries"
-version = "1.5.2"
+version = "1.5.3"
 description = "Tools for analyzing financial timeseries."
 authors = ["Martin Karrin <martin.karrin@captor.se>"]
 repository = "https://github.com/CaptorAB/openseries"
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
@@ -35,30 +35,30 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 holidays = ">=0.30,<1.0"
 numpy = ">=1.23.2,<=2.0.0"
 openpyxl = ">=3.1.2,<4.0.0"
 pandas = ">=2.1.2,<3.0.0"
 plotly = ">=5.18.0,<6.0.0"
-pyarrow = ">=14.0.2,<16.0.0"
+pyarrow = ">=14.0.2,<17.0.0"
 pydantic = ">=2.5.2,<3.0.0"
 python-dateutil = ">=2.8.2,<3.0.0"
 requests = ">=2.20.0,<3.0.0"
 scipy = ">=1.11.4,<2.0.0"
 statsmodels = ">=0.14.0,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
-coverage = "^7.4.4"
-coverage-badge = "^1.1.0"
-mypy = "^1.9.0"
+coverage = "^7.5.0"
+coverage-badge = "^1.1.1"
+mypy = "^1.10.0"
 pandas-stubs = "^2.2.1.240316"
 pre-commit = "^3.7.0"
-pytest = "^8.1.1"
-ruff = "^0.3.7"
-types-openpyxl = "^3.1.0.20240408"
+pytest = "^8.2.0"
+ruff = "^0.4.2"
+types-openpyxl = "^3.1.0.20240428"
 types-python-dateutil = "^2.9.0.20240316"
 types-requests = "^2.31.0.20240406"
 
 [build-system]
 requires = ["poetry-core>=1.8.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openseries-1.5.2/PKG-INFO` & `openseries-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.5.2
+Version: 1.5.3
 Summary: Tools for analyzing financial timeseries.
 Home-page: https://github.com/CaptorAB/openseries
 License: BSD-3-Clause
 Keywords: python,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
 Requires-Python: >=3.9,<3.13
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Dist: holidays (>=0.30,<1.0)
 Requires-Dist: numpy (>=1.23.2,<=2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.2,<3.0.0)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
-Requires-Dist: pyarrow (>=14.0.2,<16.0.0)
+Requires-Dist: pyarrow (>=14.0.2,<17.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<1.0.0)
 Project-URL: Repository, https://github.com/CaptorAB/openseries
 Description-Content-Type: text/markdown
@@ -285,14 +285,15 @@
 | `jensen_alpha`          | `OpenFrame` | Calculates [Jensen's Alpha](https://www.investopedia.com/terms/j/jensensmeasure.asp) of an asset relative a market.                                                                |
 | `tracking_error_func`   | `OpenFrame` | Calculates the [tracking errors](https://www.investopedia.com/terms/t/trackingerror.asp) relative to a selected series in the OpenFrame.                                           |
 | `info_ratio_func`       | `OpenFrame` | Calculates the [information ratios](https://www.investopedia.com/terms/i/informationratio.asp) relative to a selected series in the OpenFrame.                                     |
 | `capture_ratio_func`    | `OpenFrame` | Calculates up, down and up/down [capture ratios](https://www.investopedia.com/terms/d/down-market-capture-ratio.asp) relative to a selected series.                                |
 | `rolling_info_ratio`    | `OpenFrame` | Returns a pandas.DataFrame with the rolling [information ratio](https://www.investopedia.com/terms/i/informationratio.asp) between two series.                                     |
 | `rolling_beta`          | `OpenFrame` | Returns a pandas.DataFrame with the rolling [Beta](https://www.investopedia.com/terms/b/beta.asp) of an asset relative a market.                                                   |
 | `rolling_corr`          | `OpenFrame` | Calculates and adds a series of rolling [correlations](https://www.investopedia.com/terms/c/correlation.asp) between two other series.                                             |
+| `correl_matrix`         | `OpenFrame` | Returns a `pandas.DataFrame` with a correlation matrix.                                                                                                                            |
 | `ewma_risk`             | `OpenFrame` | Returns a `pandas.DataFrame` with volatility and correlation based on [Exponentially Weighted Moving Average](https://www.investopedia.com/articles/07/ewma.asp).                  |
 
 ### Methods that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Method                             | Applies to                    | Description                                                                                                                                              |
 |:-----------------------------------|:------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `align_index_to_local_cdays`       | `OpenTimeSeries`, `OpenFrame` | Aligns the series dates to a business calendar. Defaults to Sweden.                                                                                      |
@@ -335,15 +336,14 @@
 | `max_drawdown`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Maximum drawdown](https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp).                                                                                                                                      |
 | `max_drawdown_cal_year` | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Max drawdown in a single calendar year.                                                                                                                                                                                 |
 | `positive_share`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The share of percentage changes that are positive.                                                                                                                                                                      |
 | `vol_from_var`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Implied annualized volatility from the Downside VaR using the assumption that returns are normally distributed.                                                                                                         |
 | `skew`                  | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Skew](https://www.investopedia.com/terms/s/skewness.asp) of the return distribution.                                                                                                                                   |
 | `kurtosis`              | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Kurtosis](https://www.investopedia.com/terms/k/kurtosis.asp) of the return distribution.                                                                                                                               |
 | `z_score`               | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Z-score](https://www.investopedia.com/terms/z/zscore.asp) as (last return - mean return) / standard deviation of returns.                                                                                              |
-| `correl_matrix`         | `pandas.DataFrame`       | `OpenFrame`                   | A correlation matrix.                                                                                                                                                                                                   |
 
 ### Methods below are identical to the Numerical Properties above.
 
 _They are simply methods that take different date or length inputs to return the
 properties for subset periods._
 
 | Method                    | type                     | Applies to                    | Description                                                                                                                                                                                                                                                    |
```

