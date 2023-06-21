# Comparing `tmp/searvey-0.3.3-py3-none-any.whl.zip` & `tmp/searvey-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 43951 bytes, number of entries: 18
+Zip file size: 43235 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      372 b- defN 80-Jan-01 00:00 searvey/__init__.py
 -rw-r--r--  2.0 unx    35798 b- defN 80-Jan-01 00:00 searvey/coops.py
 -rw-r--r--  2.0 unx     2497 b- defN 80-Jan-01 00:00 searvey/critech.py
 -rw-r--r--  2.0 unx      462 b- defN 80-Jan-01 00:00 searvey/custom_types.py
 -rw-r--r--  2.0 unx     2513 b- defN 80-Jan-01 00:00 searvey/erddap.py
 -rw-r--r--  2.0 unx    12611 b- defN 80-Jan-01 00:00 searvey/ioc.py
 -rw-r--r--  2.0 unx     1389 b- defN 80-Jan-01 00:00 searvey/models.py
 -rw-r--r--  2.0 unx     4405 b- defN 80-Jan-01 00:00 searvey/multi.py
 -rw-r--r--  2.0 unx      975 b- defN 80-Jan-01 00:00 searvey/rate_limit.py
 -rw-r--r--  2.0 unx     5122 b- defN 80-Jan-01 00:00 searvey/stations.py
 -rw-r--r--  2.0 unx     2896 b- defN 80-Jan-01 00:00 searvey/uhslc.py
 -rw-r--r--  2.0 unx     1358 b- defN 80-Jan-01 00:00 searvey/us_states.json
--rw-r--r--  2.0 unx    15313 b- defN 80-Jan-01 00:00 searvey/usgs.py
+-rw-r--r--  2.0 unx    13116 b- defN 80-Jan-01 00:00 searvey/usgs.py
 -rw-r--r--  2.0 unx     4751 b- defN 80-Jan-01 00:00 searvey/utils.py
--rw-r--r--  2.0 unx    35145 b- defN 80-Jan-01 00:00 searvey-0.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4051 b- defN 80-Jan-01 00:00 searvey-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 searvey-0.3.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1342 b- defN 16-Jan-01 00:00 searvey-0.3.3.dist-info/RECORD
-18 files, 131088 bytes uncompressed, 41819 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx    35145 b- defN 80-Jan-01 00:00 searvey-0.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4051 b- defN 80-Jan-01 00:00 searvey-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 searvey-0.3.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1342 b- defN 16-Jan-01 00:00 searvey-0.3.4.dist-info/RECORD
+18 files, 128891 bytes uncompressed, 41103 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: searvey/usgs.py
 Comment: 
 
 Filename: searvey/utils.py
 Comment: 
 
-Filename: searvey-0.3.3.dist-info/LICENSE
+Filename: searvey-0.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: searvey-0.3.3.dist-info/METADATA
+Filename: searvey-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: searvey-0.3.3.dist-info/WHEEL
+Filename: searvey-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: searvey-0.3.3.dist-info/RECORD
+Filename: searvey-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## searvey/usgs.py

```diff
@@ -11,15 +11,14 @@
 """
 from __future__ import annotations
 
 import datetime
 import functools
 import importlib.metadata
 import logging
-import warnings
 from itertools import product
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
@@ -217,17 +216,15 @@
     usgs_stations = _get_all_usgs_stations(normalize=True)
     if region:
         usgs_stations = usgs_stations[usgs_stations.within(region)]
 
     return usgs_stations
 
 
-def normalize_usgs_station_data(df: pd.DataFrame, truncate_seconds: bool) -> pd.DataFrame:
-    # TODO: Does truncate seconds make sense for USGS?
-
+def normalize_usgs_station_data(df: pd.DataFrame) -> pd.DataFrame:
     if df.empty:
         return df
 
     df = df.reset_index()
     df = df.melt(id_vars=["datetime", "site_no"], var_name="output_id")
 
     df["qualifier"] = df.value.where(df.output_id.str.contains("_cd"))
@@ -254,63 +251,55 @@
     df = df.reset_index()
 
     df_parm = _get_usgs_output_info().set_index("parameter_cd")
     df = df[df.code.isin(df_parm.index)]
     df["unit"] = df_parm.parm_unit[df.code.values].values
     df["name"] = df_parm.parm_nm[df.code.values].values
 
-    if truncate_seconds:
-        # Truncate seconds from timestamps: https://stackoverflow.com/a/28783971/592289
-        # WARNING: This can potentially lead to duplicates!
-        df = df.assign(datetime=df.datetime.dt.floor("min"))
-        if df.duplicated(subset=list(USGS_DATA_MULTIIDX)).any():
-            # There are duplicates. Keep the first datapoint per minute.
-            msg = "Duplicate timestamps have been detected after the truncation of seconds. Keeping the first datapoint per minute"
-            warnings.warn(msg)
-            df = df.drop_duplicates(subset=list(USGS_DATA_MULTIIDX)).reset_index(drop=True)
-
     df = df.set_index(list(USGS_DATA_MULTIIDX))
 
     return df
 
 
 def get_usgs_station_data(
     usgs_code: str,
     endtime: DateLike = TODAY,
     period: float = 30,
-    truncate_seconds: bool = True,
     rate_limit: Optional[RateLimit] = RateLimit(),
 ) -> pd.DataFrame:
     """Retrieve the TimeSeries of a single USGS station.
 
     :param usgs_code: USGS station code a.k.a. "site number"
     :param endtime: The end date for the measurement data for fetch. Defaults to `datetime.date.today()`
     :param period: Number of date for which to fetch station data
-    :param truncate_seconds: If ``True`` then timestamps are truncated to minutes (seconds are dropped)
     :param rate_limit: The default rate limit is 5 requests/second.
     :return: ``pandas.DataFrame`` with the a single station measurements
     """
 
     if rate_limit:
         while rate_limit.reached(identifier="USGS"):
             wait()
 
     endtime = resolve_date(endtime)
     starttime = endtime - datetime.timedelta(days=period)
     df_iv, _ = nwis.get_iv(sites=[usgs_code], start=starttime.isoformat(), end=endtime.isoformat())
-    df_iv = normalize_usgs_station_data(df=df_iv, truncate_seconds=truncate_seconds)
+    df_iv = normalize_usgs_station_data(df=df_iv)
     return df_iv
 
 
 def _get_dataset_from_query_results(
-    query_result: Tuple[pd.DataFrame, Metadata], usgs_metadata: pd.DataFrame, truncate_seconds: bool
+    query_result: Tuple[pd.DataFrame, Metadata],
+    usgs_metadata: pd.DataFrame,
 ) -> xr.Dataset:
     df_iv, _ = query_result
+    if len(df_iv) == 0:
+        return xr.Dataset()
+
     df_iv = df_iv.reset_index()
-    df_iv = normalize_usgs_station_data(df=df_iv, truncate_seconds=truncate_seconds)
+    df_iv = normalize_usgs_station_data(df=df_iv)
     st_meta = (
         usgs_metadata.set_index("site_no")
         .loc[df_iv.reset_index().site_no.unique()]
         .reset_index()
         .drop_duplicates(subset="site_no")
         .set_index("site_no")
     )
@@ -327,48 +316,23 @@
     return ds
 
 
 def get_usgs_data(
     usgs_metadata: pd.DataFrame,
     endtime: DateLike = TODAY,
     period: float = 1,  # one day
-    truncate_seconds: bool = True,
     rate_limit: RateLimit = RateLimit(),
     disable_progress_bar: bool = False,
 ) -> xr.Dataset:
     """
     Return the data of the stations specified in ``usgs_metadata`` as an ``xr.Dataset``.
 
-    ``truncate_seconds`` needs some explaining. USGS has more than 1000 stations.
-    When you retrieve data from all (or at least most of) these stations, you
-    end up with thousands of timestamps that only contain a single datapoint.
-    This means that the returned ``xr.Dataset`` will contain a huge number of ``NaN``
-    which means that you will need a huge amount of RAM.
-
-    In order to reduce the amount of the required RAM we reduce the number of timestamps
-    by truncating the seconds. This is how this works:
-
-        2014-01-03 14:53:02 -> 2014-01-03 14:53:00
-        2014-01-03 14:53:32 -> 2014-01-03 14:53:00
-        2014-01-03 14:53:48 -> 2014-01-03 14:53:00
-        2014-01-03 14:54:09 -> 2014-01-03 14:54:00
-        2014-01-03 14:54:48 -> 2014-01-03 14:54:00
-
-    Nevertheless this approach has a downside. If a station returns multiple datapoints
-    within the same minute, then we end up with duplicate timestamps. When this happens
-    we only keep the first datapoint and drop the subsequent ones. So potentially you
-    may not retrieve all of the available data.
-
-    If you don't want this behavior, set ``truncate_seconds`` to ``False`` and you
-    will retrieve the full data.
-
     :param usgs_metadata: A ``pd.DataFrame`` returned by ``get_usgs_stations``.
     :param endtime: The date of the "end" of the data. Defaults to `datetime.date.today()`
     :param period: The number of days to be requested. USGS does not support values greater than 30
-    :param truncate_seconds: If ``True`` then timestamps are truncated to minutes (seconds are dropped)
     :param rate_limit: The default rate limit is 5 requests/second.
     :param disable_progress_bar: If ``True`` then the progress bar is not displayed.
     :return: ``xr.Dataset`` of station measurements
     """
     if rate_limit:
         while rate_limit.reached(identifier="USGS"):
             wait()
@@ -396,16 +360,17 @@
     datasets = []
     for result in results:
         if result.result is None:
             # When the `get_iv` call on station results in exception
             # in `data_retrieval` due to non-existant data
             continue
 
-        ds = _get_dataset_from_query_results(result.result, usgs_metadata, truncate_seconds)
-        datasets.append(ds)
+        ds = _get_dataset_from_query_results(result.result, usgs_metadata)
+        if any((ds.count(ds.dims) > 0)[v] for v in ds.data_vars):
+            datasets.append(ds)
 
     # in order to keep memory consumption low, let's group the datasets
     # and merge them in batches
     while len(datasets) > 5:
         datasets = merge_datasets(datasets)
     # Do the final merging
     ds = xr.merge(datasets)
```

## Comparing `searvey-0.3.3.dist-info/LICENSE` & `searvey-0.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `searvey-0.3.3.dist-info/METADATA` & `searvey-0.3.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searvey
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Home-page: https://github.com/oceanmodeling/searvey.git
 License: GPL-3.0-or-later
 Author: Panos Mavrogiorgos
 Author-email: pmav99@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

## Comparing `searvey-0.3.3.dist-info/RECORD` & `searvey-0.3.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 searvey/ioc.py,sha256=O68KB54QVJCjsNIR15MN8AAzKt23KY31Wjjan8EhLR8,12611
 searvey/models.py,sha256=fmRVoh9pnYE9nUzp1n53fkJVWPvJU3E38qmCZn0u5qk,1389
 searvey/multi.py,sha256=0ueJdcyqVpj3PSEhGQkO1UEVl5jBjrdPaOz7NM-lneg,4405
 searvey/rate_limit.py,sha256=DgvKX8Ww1qej2gZrJquoetHi9vSk4ErI6iTYQ3oGTdA,975
 searvey/stations.py,sha256=nlHO4iu43534t79agbNNWnZDbN13eIw_SJMlob5MN6A,5122
 searvey/uhslc.py,sha256=i4g2O-ie3gj6IPzpsS9ySSbMl9YtU_cGBXs_qoyt1VA,2896
 searvey/us_states.json,sha256=EBZm8uzX4PWgD1kgg2hBR-TEl2QbduSq2tG9sekOywE,1358
-searvey/usgs.py,sha256=pgwtdgbHX4kdB9likjjFFPnmwAwPrHTodwwcftTrfeE,15313
+searvey/usgs.py,sha256=Qpw_DTP8CtGqDcCuKKHvmA2zG1d6jjSUXsYy5_OKfhA,13116
 searvey/utils.py,sha256=xQ_c6SrfYgOutLo2dV9-neD6I6dT-Xk4sdRctiWVjKY,4751
-searvey-0.3.3.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
-searvey-0.3.3.dist-info/METADATA,sha256=yfv5d1keRwyqmWbRcyIttBiTE8buwBm4q7NOPQYJhCw,4051
-searvey-0.3.3.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-searvey-0.3.3.dist-info/RECORD,,
+searvey-0.3.4.dist-info/LICENSE,sha256=CsWICdCWFNMlGUJiXuxfrxFHw1uyVPns0jZJmzcWkjI,35145
+searvey-0.3.4.dist-info/METADATA,sha256=ZQXTuQaAY6YFM6AADfvTqhygn4P8YBNwbDHjXNKwkzI,4051
+searvey-0.3.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+searvey-0.3.4.dist-info/RECORD,,
```

