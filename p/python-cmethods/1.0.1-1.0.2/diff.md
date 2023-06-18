# Comparing `tmp/python_cmethods-1.0.1-py3-none-any.whl.zip` & `tmp/python_cmethods-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 39021 bytes, number of entries: 7
--rw-r--r--  2.0 unx    56727 b- defN 23-Apr-17 17:43 cmethods/__init__.py
--rw-r--r--  2.0 unx      160 b- defN 23-Apr-17 17:43 cmethods/_version.py
--rw-r--r--  2.0 unx    32891 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    50808 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      581 b- defN 23-Apr-17 17:43 python_cmethods-1.0.1.dist-info/RECORD
-7 files, 141268 bytes uncompressed, 37989 bytes compressed:  73.1%
+Zip file size: 39254 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    57280 b- defN 23-Jun-18 07:24 cmethods/__init__.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-18 07:24 cmethods/_version.py
+-rw-r--r--  2.0 unx    32891 b- defN 23-Jun-18 07:24 python_cmethods-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    50938 b- defN 23-Jun-18 07:24 python_cmethods-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 07:24 python_cmethods-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-18 07:24 python_cmethods-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      581 b- defN 23-Jun-18 07:24 python_cmethods-1.0.2.dist-info/RECORD
+7 files, 141951 bytes uncompressed, 38222 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: cmethods/__init__.py
 Comment: 
 
 Filename: cmethods/_version.py
 Comment: 
 
-Filename: python_cmethods-1.0.1.dist-info/LICENSE
+Filename: python_cmethods-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: python_cmethods-1.0.1.dist-info/METADATA
+Filename: python_cmethods-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: python_cmethods-1.0.1.dist-info/WHEEL
+Filename: python_cmethods-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: python_cmethods-1.0.1.dist-info/top_level.txt
+Filename: python_cmethods-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: python_cmethods-1.0.1.dist-info/RECORD
+Filename: python_cmethods-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmethods/__init__.py

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023 Benjamin Thomas Schwertfeger
-# Github: https://github.com/btschwertfeger
+# GitHub: https://github.com/btschwertfeger
 #
 
 r"""
     Module to apply different bias correction techniques to time-series climate data
 
     T = Temperatures ($T$)
     X = Some climate variable ($X$)
@@ -16,16 +16,19 @@
     simp = data to correct (predicted simulated data) ($T_{sim,p}$)
     F = Cumulative Distribution Function
     \mu = mean
     \sigma = standard deviation
     i = index
     _{m} = long-term monthly interval
 """
+
+from __future__ import annotations
+
 import multiprocessing
-from typing import List, Union
+from typing import Any, Callable, List, Optional, Union
 
 import numpy as np
 import xarray as xr
 from tqdm import tqdm
 
 __author__ = "Benjamin Thomas Schwertfeger"
 __copyright__ = __author__
@@ -35,68 +38,66 @@
 
 
 class UnknownMethodError(Exception):
     """
     Exception raised for errors if unknown method called in CMethods class.
     """
 
-    def __init__(self, method: str, available_methods: list):
+    def __init__(self: "UnknownMethodError", method: str, available_methods: list):
         super().__init__(
             f'Unknown method "{method}"! Available methods: {available_methods}'
         )
 
 
 class CMethods:
     """
-    The CMethods class serves a collection of bias correction procedures to adjust
-    time-series of climate data.
+     The CMethods class serves a collection of bias correction procedures to adjust
+     time-series of climate data.
 
-    The following bias correction techniques are available:
-        Scaling-based techniques:
-            * Linear Scaling :func:`cmethods.CMethods.linear_scaling`
-            * Variance Scaling :func:`cmethods.CMethods.variance_scaling`
-            * Delta (change) Method :func:`cmethods.CMethods.delta_method`
-
-        Distribution-based techniques:
-            * Quantile Mapping :func:`cmethods.CMethods.quantile_mapping`
-            * Detrended Quantile Mapping :func:`cmethods.CMethods.detrended_quantile_mapping`
-            * Quantile Delta Mapping :func:`cmethods.CMethods.quantile_delta_mapping`
-
-    Except for the Variance Scaling all methods can be applied on both, stochastic and non-stochastic
-    variables. The Variance Scaling can only be applied on stochastic climate variables.
-
-    Stochastic climate variables are those that are subject to random fluctuations
-    and are not predictable. They have no predictable trend or pattern. Examples of
-    stochastic climate variables include precipitation, air temperature, and humidity.
-
-    Non-stochastic climate variables, on the other hand, have clear trend and pattern histories
-    and can be readily predicted. They are often referred to as climate elements and include
-    variables such as water temperature and air pressure.
+     The following bias correction techniques are available:
+         Scaling-based techniques:
+             * Linear Scaling :func:`cmethods.CMethods.linear_scaling`
+             * Variance Scaling :func:`cmethods.CMethods.variance_scaling`
+             * Delta (change) Method :func:`cmethods.CMethods.delta_method`
+
+         Distribution-based techniques:
+             * Quantile Mapping :func:`cmethods.CMethods.quantile_mapping`
+             * Detrended Quantile Mapping :func:`cmethods.CMethods.detrended_quantile_mapping`
+             * Quantile Delta Mapping :func:`cmethods.CMethods.quantile_delta_mapping`
+
+     Except for the Variance Scaling all methods can be applied on both, stochastic and non-stochastic
+     variables. The Variance Scaling can only be applied on stochastic climate variables.
+
+    - Non-stochastic climate variables are those that can be predicted with relative certainty based
+     on factors such as location, elevation, and season. Examples of non-stochastic climate variables
+     include air temperature, air pressure, and solar radiation.
+
+     - Stochastic climate variables, on the other hand, are those that exhibit a high degree of
+       variability and unpredictability, making them difficult to forecast accurately.
+       Precipitation is an example of a stochastic climate variable because it can vary greatly in timing,
+       intensity, and location due to complex atmospheric and meteorological processes.
     """
 
-    SCALING_METHODS = ["linear_scaling", "variance_scaling", "delta_method"]
-    DISTRIBUTION_METHODS = [
+    SCALING_METHODS: List[str] = ["linear_scaling", "variance_scaling", "delta_method"]
+    DISTRIBUTION_METHODS: List[str] = [
         "quantile_mapping",
         "detrended_quantile_mapping",
         "quantile_delta_mapping",
     ]
 
-    CUSTOM_METHODS = SCALING_METHODS + DISTRIBUTION_METHODS
-    METHODS = CUSTOM_METHODS
-
-    ADDITIVE = ["+", "add"]
-    MULTIPLICATIVE = ["*", "mult"]
+    CUSTOM_METHODS: List[str] = SCALING_METHODS + DISTRIBUTION_METHODS
+    METHODS: List[str] = CUSTOM_METHODS
 
-    MAX_SCALING_FACTOR = 10
+    ADDITIVE: List[str] = ["+", "add"]
+    MULTIPLICATIVE: List[str] = ["*", "mult"]
 
-    def __init__(self):
-        pass
+    MAX_SCALING_FACTOR: Union[int, float] = 10
 
     @classmethod
-    def get_available_methods(cls) -> list:
+    def get_available_methods(cls: "CMethods") -> List[str]:
         """
         Function to return the available adjustment methods of the CMethods class.
 
         :return: List of available bias correction methods
         :rtype: List[str]
 
         .. code-block:: python
@@ -110,15 +111,15 @@
                 "linear_scaling", "variance_scaling", "delta_method",
                 "quantile_mapping", "quantile_delta_mapping"
             ]
         """
         return cls.METHODS
 
     @classmethod
-    def get_function(cls, method: str):
+    def get_function(cls: "CMethods", method: str) -> Callable:
         """
         Returns the bias correction function corresponding to the ``method`` name.
 
         :param method: The method name to get the function for
         :type method: str
         :raises UnknownMethodError: If the function is not implemented
         :return: The function of the corresponding method
@@ -138,24 +139,24 @@
             return cls.empirical_quantile_mapping
         if method == "quantile_delta_mapping":
             return cls.quantile_delta_mapping
         raise UnknownMethodError(method, cls.METHODS)
 
     @classmethod
     def adjust_3d(
-        cls,
+        cls: "CMethods",
         method: str,
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         n_quantiles: int = 100,
         kind: str = "+",
-        group: Union[str, None] = None,
+        group: Optional[str] = None,
         n_jobs: int = 1,
-        **kwargs,
+        **kwargs: Any,
     ) -> xr.core.dataarray.DataArray:
         """
         Function to apply a bias correction method on 3-dimensional climate data.
 
         *It is very important to pass ``group="time.month`` for scaling-based
         techniques if the correction should be performed as described in the
         referenced articles!* It is wanted to be the default.
@@ -167,29 +168,29 @@
         :type obs: xr.core.dataarray.DataArray
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param n_quantiles: Number of quantiles to respect. Only applies to
-            distribution-based bias correction techniques, defaults to 100
+            distribution-based bias correction techniques, defaults to ``100``
         :type n_quantiles: int, optional
-        :param kind: The kind of adjustment - additive or multiplicative, defaults to "+"
+        :param kind: The kind of adjustment - additive or multiplicative, defaults to ``"+"``
         :type kind: str, optional
-        :param group: The grouping base, Only applies to scaling-based techniques, defaults to None
-        :type group: Union[str, None], optional
-        :param n_jobs: Number of parallels jobs to run the correction, defaults to 1
+        :param group: The grouping base, Only applies to scaling-based techniques, defaults to ``None``
+        :type group: str, optional
+        :param n_jobs: Number of parallels jobs to run the correction, defaults to ``1``
         :type n_jobs: int, optional
         :raises UnknownMethodError: If the correction method is not implemented
         :return: The bias-corrected time series
         :rtype: xr.core.dataarray.DataArray
 
         .. code-block:: python
             :linenos:
-            :caption: Example application - 3-dimensinoal bias correction
+            :caption: Example application - 3-dimensional bias correction
 
             >>> import xarray as xr
             >>> from cmethods import CMethods as cm
 
             >>> # Note: The data sets must contain the dimensions "time", "lat", and "lon"
             >>> #       for the respective variable.
             >>> obsh = xr.open_dataset("path/to/reference_data-control_period.nc")
@@ -215,16 +216,16 @@
             ...     simh = simh[variable],
             ...     simp = simp[variable],
             ...     n_quantiles = 250,
             ...     n_jobs = 4
             ... )
 
             '''
-            The next exampke shows how to apply the Linear Scaling bias correction
-            techqnique based on long-term monthly means.
+            The next example shows how to apply the Linear Scaling bias correction
+            technique based on long-term monthly means.
             '''
             >>> ls_adjusted = cm.adjust_3d(
             ...     method="linear_scaling",
             ...     obs=obs[variable],
             ...     simh=simh[variable],
             ...     simp=simp[variable],
             ...     group="time.month",
@@ -236,31 +237,31 @@
         simp = simp.transpose("lat", "lon", "time").load()
 
         result = simp.copy(deep=True)
         len_lat, len_lon = len(simp.lat), len(simp.lon)
 
         if method in cls.CUSTOM_METHODS:
             if n_jobs == 1:
-                method = cls.get_function(method)
+                func = cls.get_function(method)
                 for lat in tqdm(range(len_lat)):
                     for lon in range(len_lon):
-                        result[lat, lon] = method(
+                        result[lat, lon] = func(
                             obs=obs[lat, lon],
                             simh=simh[lat, lon],
                             simp=simp[lat, lon],
                             group=group,
                             kind=kind,
                             n_quantiles=n_quantiles,
                             **kwargs,
                         )
             else:
                 try:
                     pool = multiprocessing.Pool(processes=n_jobs)
                     # with multiprocessing.Pool(processes=n_jobs) as pool:
-                    # conntext manager is not used because than the coverage does not work.
+                    # context manager is not used because than the coverage does not work.
                     # this may change when upgrading to only support Python 3.11+
                     params: List[dict] = [
                         {
                             "method": method,
                             "obs": obs[lat],
                             "simh": simh[lat],
                             "simp": simp[lat],
@@ -277,28 +278,28 @@
                     pool.close()
                     pool.join()
 
             return result.transpose("time", "lat", "lon")
         raise UnknownMethodError(method, cls.METHODS)
 
     @classmethod
-    def pool_adjust(cls, params: dict) -> np.array:
+    def pool_adjust(cls: "CMethods", params: dict) -> np.ndarray:
         """
         Adjustment along the longitudes for one specific latitude
         used by :func:`cmethods.CMethods.adjust_3d`
         as callback function for :class:`multiprocessing.Pool`.
 
-        **Not intended to be executed somwhere else.**
+        **Not intended to be executed somewhere else.**
 
         :params params: The method specific parameters
         :type params: dict
         :raises UnknownMethodError: If the specified method is not implemented
         :return: The bias-corrected time series as 2-dimensional (longitudes x time)
             numpy array
-        :rtype: np.array
+        :rtype: np.ndarray
         """
         kwargs = params.get("kwargs", {})
 
         result = params["simp"].copy(deep=True).load()
         len_lon = len(params["obs"].lon)
 
         func_adjustment = None
@@ -316,28 +317,28 @@
                 )
             return np.array(result)
 
         raise UnknownMethodError(params["method"], cls.METHODS)
 
     @classmethod
     def grouped_correction(
-        cls,
+        cls: "CMethods",
         method: str,
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         group: str,
         kind: str = "+",
-        **kwargs,
+        **kwargs: Any,
     ) -> xr.core.dataarray.DataArray:
         """Method to adjust 1 dimensional climate data while respecting adjustment groups.
 
         ----- P A R A M E T E R S -----
             method (str): adjustment method name
-            obs (xarray.core.dataarray.DataArray): observed / obserence Data
+            obs (xarray.core.dataarray.DataArray): observed / reference Data
             simh (xarray.core.dataarray.DataArray): simulated historical Data
             simp (xarray.core.dataarray.DataArray): future simulated Data
             method (str): Scaling method (e.g.: 'linear_scaling')
             group (str): [optional]  Group / Period (either: 'time.month', 'time.year' or 'time.dayofyear')
 
         ----- R E T U R N -----
 
@@ -364,22 +365,22 @@
                 result[index] = computed_result[i]
 
         return np.array(result)
 
     # ? -----========= L I N E A R - S C A L I N G =========------
     @classmethod
     def linear_scaling(
-        cls,
+        cls: "CMethods",
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
-        group: Union[str, None] = "time.month",
+        group: Optional[str] = "time.month",
         kind: str = "+",
-        **kwargs,
-    ) -> np.array:
+        **kwargs: Any,
+    ) -> np.ndarray:
         r"""
         The Linear Scaling bias correction technique can be applied on stochastic and
         non-stochastic climate variables to minimize deviations in the mean values
         between predicted and observed time-series of past and future time periods.
 
         Since the multiplicative scaling can result in very high scaling factors,
         a maximum scaling factor of 10 is set. This can be changed by passing
@@ -393,18 +394,18 @@
         *"Bias correction of regional climate model simulations for hydrological climate-change
         impact studies: Review and evaluation of different methods"*
         (https://doi.org/10.1016/j.jhydrol.2012.05.052). In the following the equations
         for both additive and multiplicative Linear Scaling are shown:
 
         **Additive**:
 
-            In Linear Scaling, the long-term monthly mean (:math:`\mu_m`) of the modeled data :math:`T_{sim,h}` is subtracted
-            from the long-term monthly mean of the reference data :math:`T_{obs,h}` at time step :math:`i`.
-            This difference in month-dependent long-term mean is than added to the long-term monthly mean for time step :math:`i`,
-            in the time-series that is to be adjusted (:math:`T_{sim,p}`).
+            In Linear Scaling, the long-term monthly mean (:math:`\mu_m`) of the modeled data :math:`X_{sim,h}` is subtracted
+            from the long-term monthly mean of the reference data :math:`X_{obs,h}` at time step :math:`i`.
+            This difference in month-dependent long-term mean is than added to the value of time step :math:`i`,
+            in the time-series that is to be adjusted (:math:`X_{sim,p}`).
 
             .. math::
 
                 X^{*LS}_{sim,p}(i) = X_{sim,p}(i) + \mu_{m}(X_{obs,h}(i)) - \mu_{m}(X_{sim,h}(i))
 
 
         **Multiplicative**:
@@ -422,21 +423,21 @@
         :type obs: xr.core.dataarray.DataArray
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param group: The grouping defines the basis of the mean, defaults to ``time.month``
-        :type group: Union[str, None], optional
+        :type group: str | None
         :param kind: The kind of the correction, additive for non-stochastic and multiplicative
             for stochastic climate variables, defaults to ``+``
         :type kind: str, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
-        :rtype: np.array
+        :rtype: np.ndarray
 
         .. code-block:: python
             :linenos:
             :caption: Example: Linear Scaling
 
             >>> import xarray as xr
             >>> from cmethods import CMethods as cm
@@ -476,22 +477,22 @@
         raise NotImplementedError(
             f"{kind} not available for linear_scaling. Use '+' or '*' instead."
         )
 
     # ? -----========= V A R I A N C E - S C A L I N G =========------
     @classmethod
     def variance_scaling(
-        cls,
+        cls: "CMethods",
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
-        group: Union[str, None] = "time.month",
+        group: Optional[str] = "time.month",
         kind: str = "+",
-        **kwargs,
-    ) -> np.array:
+        **kwargs: Any,
+    ) -> np.ndarray:
         r"""
         The Variance Scaling bias correction technique can be applied only on non-stochastic
         climate variables to minimize deviations in the mean and variance
         between predicted and observed time-series of past and future time periods.
 
         This method must be applied on a 1-dimensional data set i.e., there is only one
         time-series passed for each of ``obs``, ``simh``, and ``simp``.
@@ -500,15 +501,15 @@
         method described in the equations of Teutschbein, Claudia and Seibert, Jan (2012)
         *"Bias correction of regional climate model simulations for hydrological climate-change
         impact studies: Review and evaluation of different methods"*
         (https://doi.org/10.1016/j.jhydrol.2012.05.052). In the following the equations
         of the Variance Scaling approach are shown:
 
         **(1)** First, the modeled data of the control and scenario period must be bias-corrected using
-        the Linear Scaling technique. This corrects the deviation in the mean.
+        the additive linear scaling technique. This adjusts the deviation in the mean.
 
         .. math::
 
             X^{*LS}_{sim,h}(i) = X_{sim,h}(i) + \mu_{m}(X_{obs,h}(i)) - \mu_{m}(X_{sim,h}(i))
 
             X^{*LS}_{sim,p}(i) = X_{sim,p}(i) + \mu_{m}(X_{obs,h}(i)) - \mu_{m}(X_{sim,h}(i))
 
@@ -526,15 +527,15 @@
         **(3)** Now the standard deviation (so variance too) can be scaled.
 
         .. math::
 
             X^{VS(2)}_{sim,p}(i) = X^{VS(1)}_{sim,p}(i) \cdot \left[\frac{\sigma_{m}(X_{obs,h}(i))}{\sigma_{m}(X^{VS(1)}_{sim,h}(i))}\right]
 
 
-        **(4)** Finally the prevously removed mean is shifted back
+        **(4)** Finally the previously removed mean is shifted back
 
         .. math::
 
             X^{*VS}_{sim,p}(i) = X^{VS(2)}_{sim,p}(i) + \mu_{m}(X^{*LS}_{sim,p}(i))
 
 
         :param obs: The reference data set of the control period
@@ -542,21 +543,21 @@
         :type obs: xr.core.dataarray.DataArray
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param group: The grouping defines the basis of the mean, defaults to ``time.month``
-        :type group: Union[str, None], optional
+        :type group: str | None
         :param kind: The kind of the correction, additive for non-stochastic climate variables
             no other kind is available so far, defaults to ``+``
         :type kind: str, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``add``)
         :return: The bias-corrected time series
-        :rtype: np.array
+        :rtype: np.ndarray
 
         .. code-block:: python
             :linenos:
             :caption: Example: Variance Scaling
 
             >>> import xarray as xr
             >>> from cmethods import CMethods as cm
@@ -602,37 +603,37 @@
         raise NotImplementedError(
             f"{kind} not available for variance_scaling. Use '+' instead."
         )
 
     # ? -----========= D E L T A - M E T H O D =========------
     @classmethod
     def delta_method(
-        cls,
+        cls: "CMethods",
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
-        group: Union[str, None] = "time.month",
+        group: Optional[str] = "time.month",
         kind: str = "+",
-        **kwargs,
-    ) -> np.array:
+        **kwargs: Any,
+    ) -> np.ndarray:
         r"""
         The Delta Method bias correction technique can be applied on stochastic and
         non-stochastic climate variables to minimize deviations in the mean values
         between predicted and observed time-series of past and future time periods.
 
         Since the multiplicative scaling can result in very high scaling factors,
         a maximum scaling factor of 10 is set. This can be changed by passing
         another value to the optional `max_scaling_factor` argument.
 
         This method must be applied on a 1-dimensional data set i.e., there is only one
         time-series passed for each of ``obs``, ``simh``, and ``simp``.
 
         The Delta Method bias correction technique implemented here is based on the
         method described in the equations of Beyer, R. and Krapp, M. and Manica, A. (2020)
-        *"An empirical evaluation of bias correction methods for palaeoclimate simulations"*
+        *"An empirical evaluation of bias correction methods for paleoclimate simulations"*
         (https://doi.org/10.5194/cp-16-1493-2020). In the following the equations
         for both additive and multiplicative Delta Method are shown:
 
         **Additive**:
 
             The Delta Method looks like the Linear Scaling method but the important difference is, that the Delta method
             uses the change between the modeled data instead of the difference between the modeled and reference data of the control
@@ -661,21 +662,21 @@
         :type obs: xr.core.dataarray.DataArray
         :param simh: The modeled data of the control period
         :type simh: xr.core.dataarray.DataArray
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param group: The grouping defines the basis of the mean, defaults to ``time.month``
-        :type group: Union[str, None], optional
+        :type group: str | None
         :param kind: The kind of the correction, additive for non-stochastic and multiplicative
             for stochastic climate variables, defaults to ``+``
         :type kind: str, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
-        :rtype: np.array
+        :rtype: np.ndarray
 
         .. code-block:: python
             :linenos:
             :caption: Example: Delta Method
 
             >>> import xarray as xr
             >>> from cmethods import CMethods as cm
@@ -714,26 +715,26 @@
         raise NotImplementedError(
             f"{kind} not available for delta_method. Use '+' or '*' instead."
         )
 
     # ? -----========= Q U A N T I L E - M A P P I N G =========------
     @classmethod
     def quantile_mapping(
-        cls,
+        cls: "CMethods",
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         n_quantiles: int,
         kind: str = "+",
-        **kwargs,
-    ) -> np.array:
+        **kwargs: Any,
+    ) -> np.ndarray:
         r"""
         The Quantile Mapping bias correction technique can be used to minimize distributional
-        biases between modeled and observed time-series climate data. Its interval-independant
-        behaviour ensures that the whole time series is taken into account to redistribute
+        biases between modeled and observed time-series climate data. Its interval-independent
+        behavior ensures that the whole time series is taken into account to redistribute
         its values, based on the distributions of the modeled and observed/reference data of the
         control period.
 
         This method must be applied on a 1-dimensional data set i.e., there is only one
         time-series passed for each of ``obs``, ``simh``, and ``simp``.
 
         The Quantile Mapping technique implemented here is based on the equations of
@@ -799,15 +800,15 @@
         :type kind: str, optional
         :param val_min: Lower boundary for interpolation (only if ``kind="*"``, default: ``0.0``)
         :type val_min: float, optional
         :param val_max: Upper boundary for interpolation (only if ``kind="*"``, default: ``None``)
         :type val_max: float, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
-        :rtype: np.array
+        :rtype: np.ndarray
 
         .. code-block:: python
             :linenos:
             :caption: Example: Quantile Mapping
 
             >>> import xarray as xr
             >>> from cmethods import CMethods as cm
@@ -852,22 +853,22 @@
 
         raise NotImplementedError(
             f"{kind} for quantile_mapping is not available. Use '+' or '*' instead."
         )
 
     @classmethod
     def detrended_quantile_mapping(
-        cls,
+        cls: "CMethods",
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         n_quantiles: int,
         kind: str = "+",
-        **kwargs,
-    ) -> np.array:
+        **kwargs: Any,
+    ) -> np.ndarray:
         r"""
         The Detrended Quantile Mapping bias correction technique can be used to minimize distributional
         biases between modeled and observed time-series climate data like the regular Quantile Mapping.
         Detrending means, that the values of :math:`X_{sim,p}` are shifted to the value range of
         :math:`X_{sim,h}` before the regular Quantile Mapping is applied.
         After the Quantile Mapping was applied, the mean is shifted back. Since it does not make sens
         to take the whole mean to rescale the data, the month-dependent long-term mean is used.
@@ -878,15 +879,15 @@
 
         The Detrended Quantile Mapping technique implemented here is based on the equations of
         Alex J. Cannon and Stephen R. Sobie and Trevor Q. Murdock (2015) *"Bias Correction of GCM
         Precipitation by Quantile Mapping: How Well Do Methods Preserve Changes in Quantiles
         and Extremes?"* (https://doi.org/10.1175/JCLI-D-14-00754.1).
 
         In the following the equations of Alex J. Cannon (2015) are shown (without detrending; see QM
-        for explainations):
+        for explanations):
 
         **Additive**:
 
             .. math::
 
                 X^{*QM}_{sim,p}(i) = F^{-1}_{obs,h} \left\{F_{sim,h}\left[X_{sim,p}(i)\right]\right\}
 
@@ -913,15 +914,15 @@
         :type kind: str, optional
         :param val_min: Lower boundary for interpolation (only if ``kind="*"``, default: ``0.0``)
         :type val_min: float, optional
         :param val_max: Upper boundary for interpolation (only if ``kind="*"``, default: ``None``)
         :type val_max: float, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
-        :rtype: np.array
+        :rtype: np.ndarray
 
         .. code-block:: python
             :linenos:
             :caption: Example: Quantile Mapping
 
             >>> import xarray as xr
             >>> from cmethods import CMethods as cm
@@ -975,15 +976,15 @@
                 )  # Eq. 1
                 X = (
                     cls.get_inverse_of_cdf(cdf_obs, epsilon, xbins)
                     + m_simp_mean
                     - m_simh_mean
                 )  # Eq. 1
 
-            elif kind in cls.MULTIPLICATIVE:
+            else:  # kind in cls.MULTIPLICATIVE:
                 epsilon = np.interp(  # Eq. 2
                     cls.ensure_devidable((m_simh_mean * m_simp), m_simp_mean),
                     xbins,
                     cdf_simh,
                     left=kwargs.get("val_min", 0.0),
                     right=kwargs.get("val_max", None),
                 )
@@ -993,21 +994,21 @@
             for i, idx in enumerate(idxs):
                 res[idx] = X[i]
         return res
 
     # ? -----========= E M P I R I C A L - Q U A N T I L E - M A P P I N G =========------
     @classmethod
     def empirical_quantile_mapping(
-        cls,
+        cls: "CMethods",
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         n_quantiles: int = 100,
-        extrapolate: Union[str, None] = None,
-        **kwargs,
+        extrapolate: Optional[str] = None,
+        **kwargs: Any,
     ) -> xr.core.dataarray.DataArray:
         """
         Method to adjust 1-dimensional climate data by empirical quantile mapping
 
         :param obs: The reference data set of the control period
             (in most cases the observational data)
         :type obs: xr.core.dataarray.DataArray
@@ -1016,34 +1017,34 @@
         :param simp: The modeled data of the scenario period (this is the data set
             on which the bias correction takes action)
         :type simp: xr.core.dataarray.DataArray
         :param n_quantiles: Number of quantiles to respect/use, defaults to ``100``
         :type n_quantiles: int, optional
         :type kind: str, optional
         :param extrapolate: Bounded range or extrapolate, defaults to ``None``
-        :type extrapolate: Union[str, None], optional
+        :type extrapolate: str | None
         :return: The bias-corrected time series
         :rtype: xr.core.dataarray.DataArray
         :raises NotImplementedError: This method is not implemented
         """
         raise NotImplementedError(
             "Not implemented; please have a look at: https://svn.oss.deltares.nl/repos/openearthtools/trunk/python/applications/hydrotools/hydrotools/statistics/bias_correction.py "
         )
 
     # ? -----========= Q U A N T I L E - D E L T A - M A P P I N G =========------
     @classmethod
     def quantile_delta_mapping(
-        cls,
+        cls: "CMethods",
         obs: xr.core.dataarray.DataArray,
         simh: xr.core.dataarray.DataArray,
         simp: xr.core.dataarray.DataArray,
         n_quantiles: int,
         kind: str = "+",
-        **kwargs,
-    ) -> np.array:
+        **kwargs: Any,
+    ) -> np.ndarray:
         r"""
         The Quantile Delta Mapping bias correction technique can be used to minimize distributional
         biases between modeled and observed time-series climate data. Its interval-independant
         behaviour ensures that the whole time series is taken into account to redistribute
         its values, based on the distributions of the modeled and observed/reference data of the
         control period. In contrast to the regular Quantile Mapping (:func:`cmethods.CMethods.quantile_mapping`)
         the Quantile Delta Mapping also takes the change between the modeled data of the control and scenario
@@ -1127,15 +1128,15 @@
         :param n_quantiles: Number of quantiles to respect/use
         :type n_quantiles: int
         :param kind: The kind of the correction, additive for non-stochastic and multiplicative
             for non-stochastic climate variables, defaults to ``+``
         :type kind: str, optional
         :raises NotImplementedError: If the kind is not in (``+``, ``*``, ``add``, ``mult``)
         :return: The bias-corrected time series
-        :rtype: np.array
+        :rtype: np.ndarray
 
         .. code-block:: python
             :linenos:
             :caption: Example: Quantile Delta Mapping
 
             >>> import xarray as xr
             >>> from cmethods import CMethods as cm
@@ -1184,66 +1185,70 @@
             cdf_obs = cls.get_cdf(obs, xbins)
             cdf_simh = cls.get_cdf(simh, xbins)
             cdf_simp = cls.get_cdf(simp, xbins)
 
             epsilon = np.interp(simp, xbins, cdf_simp)  # Eq. 1.1
             QDM1 = cls.get_inverse_of_cdf(cdf_obs, epsilon, xbins)  # Eq. 1.2
 
-            delta = cls.ensure_devidable(
+            delta = cls.ensure_devidable(  # Eq. 2.3
                 simp, cls.get_inverse_of_cdf(cdf_simh, epsilon, xbins)
-            )  # Eq. 2.3
+            )
             return QDM1 * delta  # Eq. 2.4
         raise NotImplementedError(
             f"{kind} not available for quantile_delta_mapping. Use '+' or '*' instead."
         )
 
     @classmethod
     def ensure_devidable(
-        cls, numerator: Union[float, np.array], denominator: Union[float, np.array]
-    ) -> np.array:
+        cls: "CMethods",
+        numerator: Union[float, np.ndarray],
+        denominator: Union[float, np.ndarray],
+    ) -> np.ndarray:
         """
         Ensures that the arrays can be devided. The numerator will be multiplied by
         the maximum scaling factor of the CMethods class if division by zero.
 
         :param numerator: Numerator to use
-        :type numerator: np.array
+        :type numerator: np.ndarray
         :param denominator: Denominator that can be zero
-        :type denominator: np.array
+        :type denominator: np.ndarray
         :return: Zero-ensured devision
-        :rtype: np.array
+        :rtype: np.ndarray | float
         """
         with np.errstate(divide="ignore", invalid="ignore"):
             result = numerator / denominator
 
         if isinstance(numerator, np.ndarray):
             mask_inf = np.isinf(result)
             result[mask_inf] = numerator[mask_inf] * cls.MAX_SCALING_FACTOR
 
             mask_nan = np.isnan(result)
             result[mask_nan] = 0
         else:
             if np.isinf(result):
                 result = numerator * cls.MAX_SCALING_FACTOR
             elif np.isnan(result):
-                result = 0
+                result = 0.0
 
         return result
 
     @staticmethod
-    def get_pdf(x: Union[list, np.array], xbins: Union[list, np.array]) -> np.array:
+    def get_pdf(
+        x: Union[list, np.ndarray], xbins: Union[list, np.ndarray]
+    ) -> np.ndarray:
         r"""
         Compuites and returns the the probability density function :math:`P(x)`
         of ``x`` based on ``xbins``.
 
         :param x: The vector to get :math:`P(x)` from
-        :type x: Union[list, np.array]
+        :type x: Union[list, np.ndarray]
         :param xbins: The boundaries/bins of :math:`P(x)`
-        :type xbins: Union[list, np.array]
+        :type xbins: Union[list, np.ndarray]
         :return: The probability densitiy function of ``x``
-        :rtype: np.array
+        :rtype: np.ndarray
 
         .. code-block:: python
             :linenos:
             :caption: Compute the probability density function :math:`P(x)`
 
             >>> from cmethods import CMethods as cm
 
@@ -1252,25 +1257,27 @@
             >>> print(cm.get_pdf(x=x, xbins=xbins))
             [2, 5, 5]
         """
         pdf, _ = np.histogram(x, xbins)
         return pdf
 
     @staticmethod
-    def get_cdf(x: Union[list, np.array], xbins: Union[list, np.array]) -> np.array:
+    def get_cdf(
+        x: Union[list, np.ndarray], xbins: Union[list, np.ndarray]
+    ) -> np.ndarray:
         r"""
         Computes and returns returns the cumulative distribution function :math:`F(x)`
         of ``x`` based on ``xbins``.
 
         :param x: Vector to get :math:`F(x)` from
-        :type x: Union[list, np.array]
+        :type x: Union[list, np.ndarray]
         :param xbins: The boundaries/bins of :math:`F(x)`
-        :type xbins: Union[list, np.array]
+        :type xbins: Union[list, np.ndarray]
         :return: The cumulative distribution function of ``x``
-        :rtype: np.array
+        :rtype: np.ndarray
 
 
         .. code-block:: python
             :linenos:
             :caption: Compute the cmmulative distribution function :math:`F(x)`
 
             >>> from cmethods import CMethods as cm
@@ -1281,31 +1288,31 @@
             [0, 2, 7, 12]
         """
         pdf, _ = np.histogram(x, xbins)
         return np.insert(np.cumsum(pdf), 0, 0.0)
 
     @staticmethod
     def get_inverse_of_cdf(
-        base_cdf: Union[list, np.array],
-        insert_cdf: Union[list, np.array],
-        xbins: Union[list, np.array],
-    ) -> np.array:
+        base_cdf: Union[list, np.ndarray],
+        insert_cdf: Union[list, np.ndarray],
+        xbins: Union[list, np.ndarray],
+    ) -> np.ndarray:
         r"""
         Returns the inverse cumulative distribution function as:
         :math:`F^{-1}_{x}\left[y\right]` where :math:`x` represents ``base_cdf`` and
         ``insert_cdf`` is represented by :math:`y`.
 
         :param base_cdf: The basis
-        :type base_cdf: Union[list, np.array]
+        :type base_cdf: Union[list, np.ndarray]
         :param insert_cdf: The CDF that gets inserted
-        :type insert_cdf: Union[list, np.array]
+        :type insert_cdf: Union[list, np.ndarray]
         :param xbins: Probability boundaries
-        :type xbins: Union[list, np.array]
+        :type xbins: Union[list, np.ndarray]
         :return: The inverse CDF
-        :rtype: np.array
+        :rtype: np.ndarray
         """
         return np.interp(insert_cdf, base_cdf, xbins)
 
     @staticmethod
     def get_adjusted_scaling_factor(
         factor: Union[int, float], max_scaling_factor: Union[int, float]
     ) -> float:
```

## cmethods/_version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '1.0.1'
-__version_tuple__ = version_tuple = (1, 0, 1)
+__version__ = version = '1.0.2'
+__version_tuple__ = version_tuple = (1, 0, 2)
```

## Comparing `python_cmethods-1.0.1.dist-info/LICENSE` & `python_cmethods-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_cmethods-1.0.1.dist-info/METADATA` & `python_cmethods-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 1.0.1
+Version: 1.0.2
 Summary: Collection of bias correction procedures for 1- and 3-dimensional climate data
 Author-email: Benjamin Thomas Schwertfeger <development@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -658,17 +658,17 @@
 Requires-Dist: xarray (>=2022.11.0)
 Requires-Dist: netCDF4 (>=1.6.1)
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
-Requires-Dist: setuptools-scm ; extra == 'dev'
 Requires-Dist: scikit-learn ; extra == 'dev'
 Requires-Dist: scipy ; extra == 'dev'
+Requires-Dist: setuptools-scm ; extra == 'dev'
 Requires-Dist: click ; extra == 'dev'
 Requires-Dist: sphinx ; extra == 'dev'
 Requires-Dist: sphinx-rtd-theme ; extra == 'dev'
 Provides-Extra: examples
 Requires-Dist: matplotlib ; extra == 'examples'
 
 # python-cmethods
@@ -691,15 +691,15 @@
 
 </div>
 
 This Python module serves as a collection of different scale- and distribution-based bias correction techniques for climatic research
 
 The documentation is available at: [https://python-cmethods.readthedocs.io/en/stable/](https://python-cmethods.readthedocs.io/en/stable/)
 
-> ⚠️ For the application of bias corrections on _lage data sets_ it is recomanded to use the command-line tool [BiasAdjustCXX](https://github.com/btschwertfeger/BiasAdjustCXX) since bias corrections are complex statistical transformation which are very slow in Python compared to the C++ implementation.
+> ⚠️ For the application of bias corrections on _lage data sets_ it is recommended to use the command-line tool [BiasAdjustCXX](https://github.com/btschwertfeger/BiasAdjustCXX) since bias corrections are complex statistical transformation which are very slow in Python compared to the C++ implementation.
 
 ---
 
 ## Table of Contents
 
 1. [ About ](#about)
 2. [ Available Methods ](#methods)
@@ -750,21 +750,22 @@
 | `quantile_mapping`       | Quantile Mapping (additive and multiplicative) and Detrended Quantile Mapping (additive and multiplicative; to use DQM, set parameter `detrended` to `True`) |
 | `quantile_delta_mapping` | Quantile Delta Mapping (additive and multiplicative)                                                                                                         |
 | `adjust_3d`              | requires a method name and the respective parameters to adjust all time series of a 3-dimensional data set                                                   |
 
 Except for the variance scaling, all methods can be applied on stochastic and non-stochastic
 climate variables. Variance scaling can only be applied on non-stochastic climate variables.
 
-- Stochastic climate variables are those that are subject to random fluctuations
-  and are not predictable. They have no predictable trend or pattern. Examples of
-  stochastic climate variables include precipitation, air temperature, and humidity.
-
-- Non-stochastic climate variables, on the other hand, have clear trend and pattern histories
-  and can be readily predicted. They are often referred to as climate elements and include
-  variables such as water temperature and air pressure.
+- Non-stochastic climate variables are those that can be predicted with relative certainty based
+  on factors such as location, elevation, and season. Examples of non-stochastic climate variables
+  include air temperature, air pressure, and solar radiation.
+
+- Stochastic climate variables, on the other hand, are those that exhibit a high degree of
+  variability and unpredictability, making them difficult to forecast accurately.
+  Precipitation is an example of a stochastic climate variable because it can vary greatly in timing,
+  intensity, and location due to complex atmospheric and meteorological processes.
 
 ---
 
 <a name="installation"></a>
 
 ## 3. Installation
 
@@ -798,28 +799,28 @@
     obs = obsh['tas'],
     simh = simh['tas'],
     simp = simp['tas'],
     n_quaniles = 1000,
     kind = '+'
 )
 # to calculate the relative rather than the absolute change,
-# '*' can be used instead of '+' (this is prefered when adjusting
+# '*' can be used instead of '+' (this is preferred when adjusting
 # stochastic variables like precipitation)
 ```
 
 Notes:
 
 - When using the `adjust_3d` method you have to specify the method by name.
 - For the multiplicative techniques a maximum scaling factor of 10 is defined. This can be changed by the attribute `max_scaling_factor`.
 
 ## Examples (see repository on [GitHub](https://github.com/btschwertfeger/python-cmethods))
 
 Notebook with different methods and plots: `/examples/examples.ipynb`
 
-There is also an exmple script (`/examples/biasadjust.py`) that can be used to apply the available bias correction methods
+There is also an example script (`/examples/biasadjust.py`) that can be used to apply the available bias correction methods
 on 1- and 3-dimensional data sets (see `/examples/input_data/*.nc`).
 
 Help:
 
 ```bash
 ╰─ python3 biasadjust.py --help
 ```
```

