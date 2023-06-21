# Comparing `tmp/pygoogalytics-0.3.2.tar.gz` & `tmp/pygoogalytics-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.3.2.tar", last modified: Thu Apr 27 14:13:36 2023, max compression
+gzip compressed data, was "pygoogalytics-0.4.0.tar", last modified: Wed Jun 21 14:49:05 2023, max compression
```

## Comparing `pygoogalytics-0.3.2.tar` & `pygoogalytics-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-27 14:13:36.807663 pygoogalytics-0.3.2/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.3.2/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.3.2/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-27 14:13:36.807528 pygoogalytics-0.3.2/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.3.2/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-27 14:13:36.805881 pygoogalytics-0.3.2/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-27 14:13:00.000000 pygoogalytics-0.3.2/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     5386 2023-04-20 08:34:21.000000 pygoogalytics-0.3.2/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-27 14:13:36.807162 pygoogalytics-0.3.2/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.3.2/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.3.2/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    36784 2023-04-13 07:30:02.000000 pygoogalytics-0.3.2/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.3.2/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    42100 2023-04-27 14:09:01.000000 pygoogalytics-0.3.2/pygoogalytics/kwp_wrappers.py
--rw-r--r--   0 joshua     (501) staff       (20)     2485 2023-04-20 09:49:13.000000 pygoogalytics-0.3.2/pygoogalytics/resource_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.3.2/pygoogalytics/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-27 14:13:36.806668 pygoogalytics-0.3.2/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-27 14:13:36.000000 pygoogalytics-0.3.2/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-27 14:13:36.807702 pygoogalytics-0.3.2/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-27 14:13:00.000000 pygoogalytics-0.3.2/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 14:49:05.625703 pygoogalytics-0.4.0/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.4.0/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.4.0/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-06-21 14:49:05.625497 pygoogalytics-0.4.0/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.4.0/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 14:49:05.623771 pygoogalytics-0.4.0/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-06-21 14:48:42.000000 pygoogalytics-0.4.0/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3239 2023-06-21 13:16:26.000000 pygoogalytics-0.4.0/pygoogalytics/ads_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5678 2023-06-21 13:16:26.000000 pygoogalytics-0.4.0/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 14:49:05.625081 pygoogalytics-0.4.0/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.4.0/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.4.0/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)    43489 2023-06-21 14:15:30.000000 pygoogalytics-0.4.0/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    39357 2023-06-21 14:15:30.000000 pygoogalytics-0.4.0/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    42099 2023-05-09 12:29:00.000000 pygoogalytics-0.4.0/pygoogalytics/kwp_wrappers.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 14:49:05.624820 pygoogalytics-0.4.0/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      486 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-06-21 14:49:05.625759 pygoogalytics-0.4.0/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-06-21 14:48:42.000000 pygoogalytics-0.4.0/setup.py
```

### Comparing `pygoogalytics-0.3.2/LICENCE.txt` & `pygoogalytics-0.4.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.2/LICENSE` & `pygoogalytics-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.2/PKG-INFO` & `pygoogalytics-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.3.2
+Version: 0.4.0
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -14,21 +14,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 License-File: LICENSE
 
+<div id="badges">
+   <img src="https://img.shields.io/badge/3.10+-yellow?label=python&style=plastic&logo=python&logoColor=yellow" alt="Python version: 3.10 | 3.11">
+   <img src="https://img.shields.io/badge/UA (GA3) | GA4 | GSC | GoogleAds-green?label=API support&style=plastic&logo=googlecloud&logoColor=green" alt="Application support: GA3 | GSC | GoogleAds | SemRush | ScreamingFrog">
+   <img src="https://img.shields.io/badge/beta-red?label=stage&style=plastic&logoColor=blue" alt="Stage: beta">
+</div>
+
 ### Installation
 
 PyGoogalytics can be installed using [pip](https://pypi.org/project/pygoogalytics/):
 ```shell
 pip install -U pygoogalytics
 ```
 
+### Set-up
+
+Although PyGoogalytics is intended to be user-friendly it is still 
+necessary to set up various accounts and credentials with Google. 
+If you haven't yet setup API access for Universal Analytics, GA4, Search Console or Google Ads, follow [our instructions](setup_instruction.md) to get started.
+
+
 # Google Analytics API wrapper
 
 `client.py` defines the class `Client` which builds `googleapiclient.discovery` resources for accessing 
 Google Search Console and Google Analytics 3 (UA) data from the respective APIs, 
 and also `google.analytics.data_v1beta.BetaAnalyticsDataClient` resource for accessing GA4 data, although 
 currently this is only for testing.
```

### Comparing `pygoogalytics-0.3.2/README.md` & `pygoogalytics-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+<div id="badges">
+   <img src="https://img.shields.io/badge/3.10+-yellow?label=python&style=plastic&logo=python&logoColor=yellow" alt="Python version: 3.10 | 3.11">
+   <img src="https://img.shields.io/badge/UA (GA3) | GA4 | GSC | GoogleAds-green?label=API support&style=plastic&logo=googlecloud&logoColor=green" alt="Application support: GA3 | GSC | GoogleAds | SemRush | ScreamingFrog">
+   <img src="https://img.shields.io/badge/beta-red?label=stage&style=plastic&logoColor=blue" alt="Stage: beta">
+</div>
+
 ### Installation
 
 PyGoogalytics can be installed using [pip](https://pypi.org/project/pygoogalytics/):
 ```shell
 pip install -U pygoogalytics
 ```
 
+### Set-up
+
+Although PyGoogalytics is intended to be user-friendly it is still 
+necessary to set up various accounts and credentials with Google. 
+If you haven't yet setup API access for Universal Analytics, GA4, Search Console or Google Ads, follow [our instructions](setup_instruction.md) to get started.
+
+
 # Google Analytics API wrapper
 
 `client.py` defines the class `Client` which builds `googleapiclient.discovery` resources for accessing 
 Google Search Console and Google Analytics 3 (UA) data from the respective APIs, 
 and also `google.analytics.data_v1beta.BetaAnalyticsDataClient` resource for accessing GA4 data, although 
 currently this is only for testing.
```

### Comparing `pygoogalytics-0.3.2/pygoogalytics/__init__.py` & `pygoogalytics-0.4.0/pygoogalytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.3.2/pygoogalytics/client.py` & `pygoogalytics-0.4.0/pygoogalytics/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import List
 
-from .resource_utils import get_analytics_resources, \
-    googleads_client_from_yaml, googleads_client_from_key_file
+from google.ads.googleads.client import GoogleAdsClient
+
+from pygoogalytics.utils.resource_utils import get_analytics_resources, \
+    googleads_client_from_yaml, googleads_client_from_key_file, parse_ads_id
 from .googalytics_wrapper import GoogalyticsWrapper
 from .kwp_wrappers import KeywordPlanIdeaService, KeywordPlanService
+from .ads_wrapper import AdsWrapper
 from . import pga_logger
 
 
 class GoogalyticsClient:
     """
     The Client class holds the credentials for a project
     which can then be used to create a GoogalyticsWrapper object.
@@ -71,38 +74,33 @@
     def __repr__(self):
         _s = 'PyGoogalytics Client object:\n'
         for _k, _v in self.__dict__().items():
             _s += f" - {_k}: {_v}\n"
         return _s
 
 
-class KwpClient:
+class AdsClient:
     def __init__(self,
-                 key_file_yaml: str = None,
-                 key_file_path: str = None
-                 ):
-        self.googleads_client = None
-        self.default_customer_id = None
+                 googleads_client: GoogleAdsClient,
+                 default_customer_id: str):
+        self.googleads_client = googleads_client
+        self.default_customer_id = default_customer_id
 
-        if key_file_yaml:
-            self._build_from_yaml(yaml_string=key_file_yaml)
+    @classmethod
+    def build(cls, yaml_key: str = None, key_file_path: str = None):
+        if yaml_key:
+            googleads_client, default_customer_id = googleads_client_from_yaml(googleads_yaml_string=yaml_key)
+            pga_logger.info(f"initialised KwpClient object from yaml string")
         elif key_file_path:
-            self._build_from_key_file(path=key_file_path)
+            googleads_client, default_customer_id = googleads_client_from_key_file(path=key_file_path)
+            pga_logger.info(f"initialised KwpClient object from key file")
+        else:
+            raise KeyError("either yaml_key or key_file_path must be supplied")
 
-    def _build_from_yaml(self, yaml_string: str):
-        _googleads_client, _default_customer_id = googleads_client_from_yaml(googleads_yaml_string=yaml_string)
-        self.googleads_client = _googleads_client
-        self.default_customer_id = _default_customer_id
-        pga_logger.info(f"initialised KwpClient object from yaml string")
-
-    def _build_from_key_file(self, path: str):
-        _googleads_client, _default_customer_id = googleads_client_from_key_file(path=path)
-        self.googleads_client = _googleads_client
-        self.default_customer_id = _default_customer_id
-        pga_logger.info(f"initialised KwpClient object from key file")
+        return cls(googleads_client=googleads_client, default_customer_id=default_customer_id)
 
     def __bool__(self):
         if self.googleads_client is not None:
             return True
         else:
             return False
 
@@ -111,25 +109,31 @@
                      location_codes: List[str] = None,
                      language_id: str = None
                      ):
         if customer_id is None:
             customer_id = self.default_customer_id
 
         return KeywordPlanService(googleads_client=self.googleads_client,
-                                  customer_id=customer_id,
+                                  customer_id=parse_ads_id(customer_id),
                                   location_codes=location_codes,
                                   language_id=language_id)
 
     def ideas_service(self,
                       customer_id: str = None,
                       site_url: str = None,
                       location_codes: List[str] = None,
                       language_id: str = None
                       ):
         if customer_id is None:
             customer_id = self.default_customer_id
 
         return KeywordPlanIdeaService(googleads_client=self.googleads_client,
-                                      customer_id=customer_id,
+                                      customer_id=parse_ads_id(customer_id),
                                       site_url=site_url,
                                       location_codes=location_codes,
                                       language_id=language_id)
+
+    def report_service(self, customer_id: str):
+        if customer_id is None:
+            customer_id = self.default_customer_id
+        return AdsWrapper(googleads_client=self.googleads_client,
+                          customer_id=parse_ads_id(customer_id))
```

### Comparing `pygoogalytics-0.3.2/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.4.0/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.2/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.4.0/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.3.2/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.4.0/pygoogalytics/googalytics_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import pandas as pd
 import logging
 import re
 import datetime
 import json
-from typing import List, Union, Optional, Tuple
+from typing import List, Union, Optional, Any
 
 from googleapiclient.errors import HttpError as GoogleApiHttpError
+from google.api_core.exceptions import ResourceExhausted, InvalidArgument, PermissionDenied
 import google.analytics.data_v1beta.types as ga_data_types
 
 from . import googlepandas as gpd
-from . import utils
+from .utils import utils
+from .utils.ga4_parser import parse_ga4_response
 from . import pga_logger
 
 
 class GoogalyticsWrapper:
     """
     The GoogalyticsWrapper requires the following arguments to access data:
     - for GSC data: sc_domain. This is the url-like string you see in the Google Search Console web application
@@ -414,22 +416,46 @@
         if _rows is None:
             pga_logger.debug(f"{self.__class__.__name__}.get_ga3_response() :: empty ga response")
             # raise EmptyResponseError("GA3", start_date=start_date, end_date=end_date)
             return None
 
         return ga3_response
 
+    def _ga4_response_raw(self,
+                         start_date: datetime.date,
+                         end_date: datetime.date,
+                         ga4_dimensions: list[ga_data_types.Dimension],
+                         ga4_metrics: list[ga_data_types.Metric],
+                         limit: int,
+                         offset: int):
+
+        start_date_string = start_date.strftime("%Y-%m-%d")
+        end_date_string = end_date.strftime("%Y-%m-%d")
+
+        request = ga_data_types.RunReportRequest(
+            property=f"properties/{self.ga4_property_id}",
+            dimensions=ga4_dimensions,
+            metrics=ga4_metrics,
+            date_ranges=[ga_data_types.DateRange(start_date=start_date_string, end_date=end_date_string)],
+            limit=limit,
+            offset=offset,
+            return_property_quota=True
+        )
+        ga4_response = self.ga4_resource.run_report(request)
+
+        return ga4_response
+
     def get_ga4_response(self,
-                         start_date: Union[str, datetime.date],
-                         end_date: Optional[Union[str, datetime.date]] = None,
-                         ga4_dimensions: Optional[Union[List[str], str]] = None,
-                         ga4_metrics: Optional[Union[List[str], str]] = None,
+                         start_date: str | datetime.date,
+                         end_date: str | datetime.date | None = None,
+                         ga4_dimensions: list[str] | str | None = None,
+                         ga4_metrics: list[str] | str | None = None,
                          filter_google_organic: bool = False,
                          raise_http_error: bool = False,
-                         return_raw_response: bool = False):
+                         limit: int | None = None) -> (list, dict, Any):
 
         if not self.ga4_property_id:
             # If there is no view_id we stop here and return None,
             # unless raise_http_error is True, in which case we continue to the execution and see what errors come up
             pga_logger.warning(f"{self.__class__.__name__}.get_ga4_response() :: ga4_property_id is not set")
             if not raise_http_error:
                 return None
@@ -438,42 +464,114 @@
             end_date = start_date
 
         if isinstance(start_date, str):
             start_date = datetime.datetime.strptime(start_date, "%Y-%m-%d").date()
         if isinstance(end_date, str):
             end_date = datetime.datetime.strptime(end_date, "%Y-%m-%d").date()
 
-        start_date_string = start_date.strftime("%Y-%m-%d")
-        end_date_string = end_date.strftime("%Y-%m-%d")
-
         if ga4_dimensions is None:
-            ga4_dimensions = ['ga:productName']
+            ga4_dimensions = ["dateHour", "landingPage"]
         elif isinstance(ga4_dimensions, str):
-            ga4_dimensions = [ga4_dimensions]
+            ga4_dimensions = [_.strip() for _ in ga4_dimensions.split(',')]
 
         if ga4_metrics is None:
-            ga4_metrics = ['ga:itemRevenue']
+            ga4_metrics = ["totalUsers"]
         elif isinstance(ga4_metrics, str):
-            ga4_metrics = [ga4_metrics]
+            ga4_metrics = [_.strip() for _ in ga4_metrics.split(',')]
 
         dimensions = [ga_data_types.Dimension(name=_) for _ in ga4_dimensions]
         metrics = [ga_data_types.Metric(name=_) for _ in ga4_metrics]
 
-        request = ga_data_types.RunReportRequest(
-            property=f"properties/{self.ga4_property_id}",
-            dimensions=dimensions,
-            metrics=metrics,
-            date_ranges=[ga_data_types.DateRange(start_date=start_date_string, end_date=end_date_string)],
-        )
-        ga4_response = self.ga4_resource.run_report(request)
-        if return_raw_response:
-            pga_logger.info(f"{self.__class__.__name__}.get_ga4_response() :: returning raw response")
-            return ga4_response
+        request_limit = 100_000
+        if limit is None:
+            limit = 1_000_000_000
+        elif limit < 100_000:
+            request_limit = limit
+
+        offset: int = 0
+        complete: bool = False
+        error_type: str | None = None
+        rows: list[dict] = []
+        metadata: list[dict] = []
+        error = None
+
+        tokens_per_hour_consumed: int = 0
+        tokens_per_day_consumed: int = 0
+
+        while not complete:
+            num_tries = 0
+            success = False
+            _rows, _metadata = [], dict()
+            while num_tries < 3 and not success:
+                error = None
+                try:
+                    ga4_response = self._ga4_response_raw(
+                        start_date=start_date,
+                        end_date=end_date,
+                        ga4_dimensions=dimensions,
+                        ga4_metrics=metrics,
+                        limit=request_limit,
+                        offset=offset
+                    )
+                    _rows, _metadata = parse_ga4_response(ga4_response)
+                    success = True
+                except PermissionDenied as _permission_denied_error:
+                    complete = True
+                    error_type = 'permission_denied'
+                    error = _permission_denied_error
+                    num_tries = 7
+                except ResourceExhausted as _resource_exhausted_error:
+                    error_type = 'quota_reached'
+                    complete = True
+                    error = _resource_exhausted_error
+                    num_tries = 7
+                except InvalidArgument as _invalid_argument_error:
+                    if re.search(r"metrics are incompatible", _invalid_argument_error.message):
+                        error_type = 'invalid_arguments'
+                    complete = True
+                    error = _invalid_argument_error
+                    num_tries = 7
+                except Exception as _e:
+                    error = _e
+                    num_tries += 1
+
+            if success:
+                rows_returned = len(_rows)
+                offset += rows_returned
+                if offset >= limit:
+                    complete = True
+                if rows_returned == 0 or offset >= _metadata.get('meta_row_count', 1_000_000_000):
+                    complete = True
+
+                tokens_per_hour_consumed += _metadata.get('quota', dict()).get('tokens_per_hour', dict()).get('consumed', 0)
+                tokens_per_day_consumed += _metadata.get('quota', dict()).get('tokens_per_day', dict()).get('consumed', 0)
+
+                rows.extend(_rows)
+                metadata.append(_metadata)
+
+        response = dict()
+        if len(metadata) > 0:
+            response = metadata[-1]
+            response['quota']['tokens_per_hour']['consumed'] = tokens_per_hour_consumed
+            response['quota']['tokens_per_day']['consumed'] = tokens_per_day_consumed
+        else:
+            response['response_type'] = 'GA4'
+            response['dimension_headers'] = ga4_dimensions
+            response['metric_headers'] = ga4_metrics
+
+        response['response_type'] = 'GA4'
+        response['start_date'] = start_date
+        response['end_date'] = end_date
+        response['total_rows'] = offset
+        response['rows'] = rows
 
-        return ga4_response
+        response['error'] = error
+        response['error_type'] = error_type
+
+        return response
 
     def get_dates(self,
                   result: str,
                   start_date: Optional[Union[datetime.date, str, int]] = None,
                   end_date: Optional[Union[datetime.date, str]] = None,
                   reverse: bool = False) -> List[datetime.date]:
 
@@ -532,15 +630,16 @@
                end_date: Optional[Union[str, datetime.date]] = None,
                dimensions: Optional[Union[str, List[str]]] = None,
                metrics: Optional[Union[str, List[str]]] = None,
                row_limit: Optional[int] = None,
                url_list: Optional[Union[str, List[str]]] = None,
                filter_google_organic: bool = False,
                filters: List[dict] = None,
-               add_boolean_metrics: bool = False
+               add_boolean_metrics: bool = False,
+               _return_response: bool = False
                ) -> Union[gpd.GADataFrame, gpd.GSCDataFrame, pd.DataFrame]:
         """
         The `get_df` method accepts the following values for the `result` argument:
         - "GSC": for Google Search Console data
         - "GA3": for Google Analytics 3 (UA) data
         - "URL": for Google Search Console URL inspection data
         - "GA4": for Google Analytics 4 data (note, this is not yet available in production)
@@ -570,15 +669,17 @@
         if re.match(r"GA4", result):
             return self._get_ga4_df(start_date=start_date,
                                     end_date=end_date,
                                     ga_dimensions=dimensions,
                                     ga_metrics=metrics,
                                     add_boolean_metrics=add_boolean_metrics,
                                     filter_google_organic=filter_google_organic,
-                                    filters=filters)
+                                    limit=row_limit,
+                                    filters=filters,
+                                    return_response=_return_response)
         elif re.match(r"GA3", result):
             return self._get_ga3_df(start_date=start_date,
                                     end_date=end_date,
                                     ga_dimensions=dimensions,
                                     ga_metrics=metrics,
                                     add_boolean_metrics=add_boolean_metrics,
                                     filter_google_organic=filter_google_organic,
@@ -681,32 +782,99 @@
 
         return gsc_df
 
     def _get_ga4_df(self,
                     start_date: datetime.date,
                     end_date: datetime.date,
                     ga_dimensions: Optional[List[str]] = None,
-                    ga_metrics: Optional[List[str]] = None,
+                    ga_metrics: list[str] | list[list[str]] = None,
                     add_boolean_metrics: bool = True,
                     filters: Optional[dict] = None,
-                    filter_google_organic: bool = False) -> Optional[gpd.GADataFrame]:
-        _df = gpd.GADataFrame(df_input=None,
-                              dimensions=ga_dimensions,
-                              metrics=ga_metrics,
-                              start_date=start_date,
-                              end_date=end_date)
-        return _df
+                    limit: int | None = 100_000_000,
+                    return_response: bool = False,
+                    raise_errors: bool = False,
+                    filter_google_organic: bool = False) -> gpd.GADataFrame:
+
+        if all(isinstance(_, str) for _ in ga_metrics):
+            ga_metrics = [ga_metrics]
+
+        metrics_list: list[list[str]] = []
+        for _list in ga_metrics:
+            metrics_list.extend([_list[10 * i:10 * i + 10] for i in range((len(_list) - 1) // 10 + 1)])
+
+        responses: list = []
+        breaking_error: bool = False
+        breaking_error_type: str | None = None
+        for _ga_metrics in metrics_list:
+            _r = self.get_ga4_response(
+                            start_date=start_date,
+                            end_date=end_date,
+                            ga4_dimensions=ga_dimensions,
+                            ga4_metrics=_ga_metrics,
+                            limit=limit,
+                        )
+            responses.append(_r)
+            if _t := _r.get('error_type') is not None:
+                breaking_error = True
+                breaking_error_type = _t
+                break
+
+        if return_response:
+            return responses
+
+        if raise_errors:
+            _errors = [_r.get('error') for _r in responses if _r.get('error') is not None]
+            if len(_errors) > 0:
+                raise _errors[0]
+
+        if breaking_error:
+            frames = []
+        else:
+            frames = [gpd.from_response(response=_r) for _r in responses]
+
+        if len(frames) == 0:
+            ga4_df = gpd.GADataFrame(df_input=None,
+                                     dimensions=ga_dimensions,
+                                     metrics=ga_metrics,
+                                     start_date=start_date,
+                                     end_date=end_date,
+                                     error = breaking_error_type)
+
+        elif all(len(_frame) == 0 for _frame in frames):
+            ga4_df = gpd.GADataFrame(df_input=None,
+                                     dimensions=ga_dimensions,
+                                     metrics=ga_metrics,
+                                     start_date=start_date,
+                                     end_date=end_date)
+        elif len(frames) == 1:
+            ga4_df = frames[0]
+        else:
+            ga4_df = frames[0]
+            for i in range(1, len(frames)):
+                ga4_df = ga4_df.join_on_dimensions(frames[i], how="outer")
+
+        if add_boolean_metrics:
+            ga4_df.add_google_organic_column()
+            ga4_df.add_has_item_column()
+            ga4_df.add_new_user_column()
+            ga4_df.add_shopping_stage_all_column()
+            ga4_df.add_has_site_search_column()
+
+        ga4_df.fill_nan_with_zeros()
+
+        return ga4_df
+
 
     def _get_ga3_df(self,
                     start_date: datetime.date,
                     end_date: datetime.date,
-                    ga_dimensions: Optional[List[str]] = None,
-                    ga_metrics: Optional[List[str]] = None,
+                    ga_dimensions: list[str] | None = None,
+                    ga_metrics: list[str] | None = None,
                     add_boolean_metrics: bool = True,
-                    filters: Optional[dict] = None,
+                    filters: dict | None = None,
                     filter_google_organic: bool = False) -> Optional[gpd.GADataFrame]:
 
         if ga_dimensions is None:
             ga_dimensions = ['ga:date',
                              'ga:landingPagePath',
                              'ga:productName',
                              'ga:source',
@@ -739,22 +907,24 @@
                 # Make a dataframe of the ga response
                 ga3_df = gpd.from_response(response=ga3_response,
                                            response_type="GA3",
                                            start_date=start_date,
                                            end_date=end_date)
             else:
                 ga3_df = gpd.GADataFrame(df_input=None,
+                                         response_type='GA3',
                                          dimensions=ga_dimensions,
                                          metrics=metrics,
                                          start_date=start_date,
                                          end_date=end_date)
             frames.append(ga3_df)
 
         if all(len(_frame) == 0 for _frame in frames):
             ga3_df = gpd.GADataFrame(df_input=None,
+                                     response_type='GA3',
                                      dimensions=ga_dimensions,
                                      metrics=ga_metrics,
                                      start_date=start_date,
                                      end_date=end_date)
         else:
             join_dimensions = frames[0].join_dimensions
             if not all(set(_df.join_dimensions) == set(join_dimensions) for _df in frames):
@@ -765,14 +935,15 @@
                     print(f"\t\tmetrics:    {_df.metrics}")
                     print(f"\t\tdimensions: {_df.join_dimensions}")
                 raise AssertionError("unmatched join dimensions")
             ga3_df = frames[0]
             for i in range(1, len(frames)):
                 ga3_df = pd.merge(ga3_df, frames[i], how="outer", on=join_dimensions)
             ga3_df = gpd.GADataFrame(df_input=ga3_df,
+                                     response_type='GA3',
                                      dimensions=ga_dimensions,
                                      metrics=ga_metrics,
                                      from_ga_response=False,
                                      join_dimensions=join_dimensions,
                                      start_date=start_date,
                                      end_date=end_date)
```

### Comparing `pygoogalytics-0.3.2/pygoogalytics/googlepandas.py` & `pygoogalytics-0.4.0/pygoogalytics/googlepandas.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 import re
 import csv
 import os
 import numpy as np
 import pandas as pd
 import datetime
 
+from google.analytics.data_v1beta.types.analytics_data_api import RunReportResponse
+
 from typing import List, Optional, Union, Pattern
 
-from . import utils
+from .utils import utils
+from .utils.ga4_parser import parse_ga4_response
 
 gpd_logger = logging.getLogger("googlepandas")
 
 
 def camel_to_snake(string: str):
     return utils.RE_C2S.sub('_', string).lower()
 
@@ -54,15 +57,15 @@
     'ga:productDetailViews': float,
     'ga:productListCTR': float,
     'ga:productListClicks': float,
     'ga:productListViews': float
 }
 
 
-def from_response(response: dict,
+def from_response(response: dict | RunReportResponse,
                   response_type: str = None,
                   report_index: int = 0,
                   gsc_dimensions: Optional[List[str]] = None,
                   start_date: datetime.date = None,
                   end_date: datetime.date = None):
     # We're going to what kind of response this is by making assumptions about what the responses will look like.
     # If the response dictionary includes a 'report' key, we assume it is a GA response.
@@ -76,17 +79,44 @@
         _metric_header_entries = response.get('reports')[report_index] \
             .get('columnHeader') \
             .get('metricHeader') \
             .get('metricHeaderEntries')
         metrics = [_d['name'] for _d in _metric_header_entries]
         gpd_logger.debug(f"from_response: creating GADataFrame. dimensions = [{dimensions}], metrics = [{metrics}]")
         return GADataFrame(df_input=rows,
+                           response_type='GA3',
                            dimensions=dimensions, metrics=metrics,
                            start_date=start_date, end_date=end_date,
                            from_ga_response=True)
+    elif response_type == 'GA4':
+        if isinstance(response, RunReportResponse):
+            rows, metadata = parse_ga4_response(response)
+            return GADataFrame(df_input=rows,
+                               response_type='GA4',
+                               dimensions=metadata.get('dimension_headers'),
+                               metrics=metadata.get('metric_headers'),
+                               row_count=metadata.get('row_count'),
+                               start_date=start_date, end_date=end_date,
+                               from_ga_response=True)
+        else:
+            rows = response.get('rows')
+            from_ga_response = True
+            if len(rows) == 0:
+                rows = None
+                from_ga_response = False
+            return GADataFrame(df_input=rows,
+                               response_type='GA4',
+                               dimensions=response.get('dimension_headers'),
+                               metrics=response.get('metric_headers'),
+                               row_count=response.get('total_row_count'),
+                               start_date=response.get('start_date'),
+                               end_date=response.get('end_date'),
+                               error=response.get('error_type'),
+                               from_ga_response=from_ga_response)
+
     elif response_type == 'GSC':
         rows = response.get('rows', [])
         response_aggregation = response.get('responseAggregationType', None)
         gpd_logger.debug("from_response: creating GSCDataFrame")
         _gsc_df = GSCDataFrame(df_input=rows,
                                gsc_dimensions=gsc_dimensions,
                                from_gsc_response=True)
@@ -122,173 +152,259 @@
         category_regex_dict: dictionary of regex patterns supplied to __init__()
     """
 
     _metadata = ["dimensions",
                  "metrics",
                  "join_dimensions",
                  "date_range",
-                 "date_range_days"]
+                 "date_range_days",
+                 "time_obtained",
+                 "row_count",
+                 "response_type",
+                 "error"]
 
     def __init__(self, df_input,
-                 dimensions: Optional[List[str]] = None,
-                 metrics: Optional[List[str]] = None,
+                 dimensions: list[str] = None,
+                 metrics: list[str] = None,
                  from_ga_response: bool = False,
                  join_dimensions: List[str] = None,
                  start_date: datetime.date = None,
-                 end_date: datetime.date = None
+                 end_date: datetime.date = None,
+                 time_obtained: datetime.datetime = None,
+                 row_count: int = 0,
+                 response_type: str = 'GA4',
+                 error: str | None = None
                  ):
 
+        if time_obtained:
+            self.time_obtained = time_obtained.astimezone(tz=datetime.tzinfo())
+        else:
+            self.time_obtained = datetime.datetime.now(tz=datetime.timezone.utc)
+
         self.dimensions = dimensions
         self.metrics = metrics
+
+        if join_dimensions is None:
+            join_dimensions = dimensions
+
         self.join_dimensions = join_dimensions
-        self.date_range = {'start': start_date, 'end': end_date}
+
+        self.date_range = {
+            'start': start_date or datetime.date.today(),
+            'end': end_date or datetime.date.today()
+        }
+        self.row_count = row_count
+        self.response_type = response_type
+        self.error = error
+
         if start_date and end_date:
             self.date_range_days = (end_date - start_date).days + 1
         else:
             self.date_range_days = None
 
         if df_input is None:
-            join_dimensions = [strip_ga_prefix(_) for _ in self.dimensions]
+            self.join_dimensions = [strip_ga_prefix(_) for _ in self.dimensions]
             super().__init__(None, columns=[strip_ga_prefix(_) for _ in dimensions + metrics])
+
+            if 'landingPagePlusQueryString' in self.columns:
+                self.rename(columns={'landingPagePlusQueryString': 'landingPagePath'}, inplace=True)
+                self.remove_join_dimensions('landingPagePlusQueryString')
+                self.add_join_dimensions('landingPagePath')
+
             if 'landingPagePath' in self.columns:
                 # rename 'landingPagePath' to 'landingPageFull', then add dummy columns for
                 # 'landingPage' and 'landingPageParameter'
                 self.rename(columns={'landingPagePath': 'landingPageFull'}, inplace=True)
                 self['landingPage'] = None
                 self['landingPageParameter'] = None
-                join_dimensions = remove_list_item(join_dimensions, 'landingPagePath')
-                join_dimensions.extend(['landingPage', 'landingPageFull', 'landingPageParameter'])
+                self.remove_join_dimensions('landingPagePath')
+                self.add_join_dimensions(['landingPage', 'landingPageFull', 'landingPageParameter'])
 
             if 'deviceCategory' in self.columns:
                 self.rename(columns={'deviceCategory': 'device'}, inplace=True)
-                join_dimensions = remove_list_item(join_dimensions, 'deviceCategory')
-                join_dimensions.extend(['device'])
+                self.remove_join_dimensions('deviceCategory')
+                self.add_join_dimensions(['device'])
 
             if 'sourceMedium' in self.columns:
                 self['source'] = None
                 self['medium'] = None
                 self.drop(columns='sourceMedium', inplace=True)
-                join_dimensions = remove_list_item(join_dimensions, 'sourceMedium')
-                join_dimensions.extend(['source', 'medium'])
+                self.remove_join_dimensions('sourceMedium')
+                self.add_join_dimensions(['source', 'medium'])
+
+            if 'sessionSourceMedium' in self.columns:
+                self['source'] = None
+                self['medium'] = None
+                self.drop(columns='sessionSourceMedium', inplace=True)
+                self.remove_join_dimensions('sessionSourceMedium')
+                self.add_join_dimensions(['source', 'medium'])
 
             if 'transactionsPerSession' in self.columns:
                 self.rename(columns={'transactionsPerSession': 'conversionRate'}, inplace=True)
 
+            if 'itemPurchaseQuantity' in self.columns:
+                self.rename(columns={'itemPurchaseQuantity': 'itemQuantity'}, inplace=True)
+
             if 'date' in self.columns:
                 self.rename(columns={'date': 'recordDate'}, inplace=True)
-                join_dimensions = remove_list_item(join_dimensions, 'date')
-                join_dimensions.extend(['recordDate'])
+                self.remove_join_dimensions('date')
+                self.add_join_dimensions(['recordDate'])
 
             if 'dateHourMinute' in self.columns:
                 self['recordDate'] = None
                 self['recordTime'] = None
                 self.drop(columns='dateHourMinute', inplace=True)
-                join_dimensions = remove_list_item(join_dimensions, 'dateHourMinute')
-                join_dimensions.extend(['recordDate', 'recordTime'])
+                self.remove_join_dimensions('dateHourMinute')
+                self.add_join_dimensions(['recordDate', 'recordTime'])
 
-            self.join_dimensions = [camel_to_snake(_) for _ in join_dimensions]
+            if 'dateHour' in self.columns:
+                self['recordDate'] = None
+                self['recordTime'] = None
+                self.drop(columns='dateHour', inplace=True)
+                self.remove_join_dimensions('dateHour')
+                self.add_join_dimensions(['recordDate', 'recordTime'])
+
+            self.snake_case_join_dimensions()
 
         else:
             super().__init__(df_input)
 
         if from_ga_response:
-            for _i in range(len(self.metrics) - 1, -1, -1):
-                self.insert(loc=0, column=strip_ga_prefix(self.metrics[_i]),
-                            value=self['metrics'].apply(lambda x: x[0].get('values')[_i]
-                                                        ).astype(GA_Types.get(self.metrics[_i], str))
-                            )
-            self.drop(columns='metrics', inplace=True)
-
-            for _i in range(len(self.dimensions) - 1, -1, -1):
-                self.insert(loc=0, column=strip_ga_prefix(self.dimensions[_i]),
-                            value=self['dimensions'].apply(lambda x: x[_i]
-                                                           ).astype(GA_Types.get(self.dimensions[_i], str))
-                            )
-            self.drop(columns='dimensions', inplace=True)
-            join_dimensions = [strip_ga_prefix(_) for _ in self.dimensions]
+            if response_type == 'GA3':
+                for _i in range(len(self.metrics) - 1, -1, -1):
+                    self.insert(loc=0, column=strip_ga_prefix(self.metrics[_i]),
+                                value=self['metrics'].apply(lambda x: x[0].get('values')[_i]
+                                                            ).astype(GA_Types.get(self.metrics[_i], str))
+                                )
+                self.drop(columns='metrics', inplace=True)
+
+                for _i in range(len(self.dimensions) - 1, -1, -1):
+                    self.insert(loc=0, column=strip_ga_prefix(self.dimensions[_i]),
+                                value=self['dimensions'].apply(lambda x: x[_i]
+                                                               ).astype(GA_Types.get(self.dimensions[_i], str))
+                                )
+                self.drop(columns='dimensions', inplace=True)
+                self.join_dimensions = [strip_ga_prefix(_) for _ in self.dimensions]
 
             if 'productName' in self.columns:
                 self['productName'] = self['productName'].apply(lambda s: s.strip().lower()
                                                                 .replace('-', ' ')
                                                                 .replace('_', ' ')
                                                                 .replace('&amp;', '&')
                                                                 )
                 self['productName'] = self['productName'].apply(lambda s: re.sub(r"\\u[a-f\d]{4}", " ", s))
                 self['productName'] = self['productName'].apply(lambda s: re.sub(r"\s+", " ", s).strip())
 
+            if 'landingPagePlusQueryString' in self.columns:
+                self.rename(columns={'landingPagePlusQueryString': 'landingPagePath'}, inplace=True)
+                self.remove_join_dimensions('landingPagePlusQueryString')
+                self.add_join_dimensions('landingPagePath')
+
+            if 'itemPurchaseQuantity' in self.columns:
+                self.rename(columns={'itemPurchaseQuantity': 'itemQuantity'}, inplace=True)
+
             if 'landingPagePath' in self.columns:
-                self['landingPage'] = self['landingPagePath'].apply(utils.strip_url)
+                self['landingPagePath'] = self['landingPagePath'].apply(utils.url_strip_domain)
+                self['landingPage'] = self['landingPagePath'].apply(lambda _u: _u.split('?')[0])
                 self['landingPageParameter'] = self['landingPagePath'].apply(utils.url_extract_parameter)
                 self.rename(columns={'landingPagePath': 'landingPageFull'}, inplace=True)
 
-                join_dimensions = remove_list_item(join_dimensions, 'landingPagePath')
-                join_dimensions.extend(['landingPageFull', 'landingPageParameter', 'landingPage'])
+                self.remove_join_dimensions('landingPagePath')
+                self.add_join_dimensions(['landingPageFull', 'landingPageParameter', 'landingPage'])
 
             if 'transactionsPerSession' in self.columns:
                 self.rename(columns={'transactionsPerSession': 'conversionRate'}, inplace=True)
 
             if 'deviceCategory' in self.columns:
                 self.rename(columns={'deviceCategory': 'device'}, inplace=True)
-                join_dimensions = remove_list_item(join_dimensions, 'deviceCategory')
-                join_dimensions.extend(['device'])
+                self.remove_join_dimensions('deviceCategory')
+                self.add_join_dimensions('device')
 
             if 'sourceMedium' in self.columns:
                 self['source'] = self.sourceMedium.apply(lambda s: s.split('/')[0].strip())
                 self['medium'] = self.sourceMedium.apply(lambda s: s.split('/')[1].strip() if '/' in s else None)
                 self.drop(columns='sourceMedium', inplace=True)
-                join_dimensions = remove_list_item(join_dimensions, 'sourceMedium')
-                join_dimensions.extend(['source', 'medium'])
+                self.remove_join_dimensions('sourceMedium')
+                self.add_join_dimensions(['source', 'medium'])
+
+            if 'sessionSourceMedium' in self.columns:
+                self['source'] = self['sessionSourceMedium'].apply(lambda s: s.split('/')[0].strip())
+                self['medium'] = self['sessionSourceMedium'].apply(lambda s: s.split('/')[1].strip() if '/' in s else None)
+                self.drop(columns='sessionSourceMedium', inplace=True)
+                self.remove_join_dimensions('sessionSourceMedium')
+                self.add_join_dimensions(['source', 'medium'])
 
             if 'date' in self.columns:
                 self.drop(
                     self[self.date.apply(lambda _date: True if _date == '(other)' else False)].index,
                     inplace=True
                 )
                 self.date = pd.to_datetime(self.date, format="%Y%m%d")
                 self.date = self.date.apply(lambda date_time: datetime.datetime.date(date_time))
                 self.rename(columns={'date': 'recordDate'}, inplace=True)
-                join_dimensions = remove_list_item(join_dimensions, 'date')
-                join_dimensions.extend(['recordDate'])
+                self.remove_join_dimensions('date')
+                self.add_join_dimensions('recordDate')
 
             if 'dateHourMinute' in self.columns:
                 self.drop(
                     self[self.dateHourMinute.apply(lambda _datetime: True if _datetime == '(other)' else False)].index,
                     inplace=True
                 )
                 date_time_series = pd.to_datetime(self.dateHourMinute, format="%Y%m%d%H%M")
                 self['recordDate'] = date_time_series.apply(lambda date_time: datetime.datetime.date(date_time))
                 self['recordTime'] = date_time_series.apply(lambda date_time: date_time.time())
                 self.drop(columns='dateHourMinute', inplace=True)
-                join_dimensions = remove_list_item(join_dimensions, 'dateHourMinute')
-                join_dimensions.extend(['recordDate', 'recordTime'])
+                self.remove_join_dimensions('dateHourMinute')
+                self.add_join_dimensions(['recordDate', 'recordTime'])
+
+            if 'dateHour' in self.columns:
+                self.drop(
+                    self[self['dateHour'].apply(lambda _datetime: True if _datetime == '(other)' else False)].index,
+                    inplace=True
+                )
+                date_time_series = pd.to_datetime(self['dateHour'], format="%Y%m%d%H")
+                self['recordDate'] = date_time_series.apply(lambda date_time: datetime.datetime.date(date_time))
+                self['recordTime'] = date_time_series.apply(lambda date_time: date_time.time())
+                self.drop(columns='dateHour', inplace=True)
+                self.remove_join_dimensions('dateHour')
+                self.add_join_dimensions(['recordDate', 'recordTime'])
 
             if 'countryIsoCode' in self.columns:
                 self.countryIsoCode = self.countryIsoCode.apply(iso_code_2_to_3)
 
-            self.join_dimensions = [camel_to_snake(_) for _ in join_dimensions]
+            if 'countryId' in self.columns:
+                self['countryIsoCode'] = self['countryId'].apply(iso_code_2_to_3)
+                self.drop(columns='countryId', inplace=True)
+                self.remove_join_dimensions('countryId')
+                self.add_join_dimensions(['countryIsoCode'])
+
+            self.snake_case_join_dimensions()
 
         self.snake_case_columns()
 
         if "record_date" not in self.columns:
             if start_date and end_date:
                 self.insert(loc=0, column="record_date", value=end_date)
                 self.insert(loc=0, column="record_date_start", value=start_date)
-                self.join_dimensions.append("record_date")
-                self.join_dimensions.append("record_date_start")
+                self.add_join_dimensions("record_date")
+                self.add_join_dimensions("record_date_start")
             elif end_date:
                 self.insert(loc=0, column="record_date", value=end_date)
-                self.join_dimensions.append("record_date")
+                self.add_join_dimensions("record_date")
             elif start_date:
                 self.insert(loc=0, column="record_date", value=start_date)
-                self.join_dimensions.append("record_date")
+                self.add_join_dimensions("record_date")
 
     def snake_case_columns(self):
         self.rename(columns={old_col_name: camel_to_snake(old_col_name)
                              for old_col_name in self.columns},
                     inplace=True)
+        
+    def snake_case_join_dimensions(self):
+        self.join_dimensions = [camel_to_snake(_) for _ in self.join_dimensions]
 
     def add_brand_column(self,
                          brand_function: Optional[str],
                          brands_dict: Optional[dict] = None):
         if 'product_name' in self.columns:
             _loc = self.columns.get_loc('product_name') + 1
             if brand_function == "first word":
@@ -399,15 +515,15 @@
         if 'item_quantity' in self.columns:
             _loc = self.columns.get_loc('item_quantity') + 1
             if len(self) == 0:
                 self['has_item'] = None
             else:
                 self.insert(loc=_loc,
                             column='has_item',
-                            value=self.item_quantity.apply(lambda quantity: False if quantity == 0 else True)
+                            value=self.item_quantity.apply(lambda quantity: True if quantity else False)
                             )
         else:
             pass
 
     def add_landing_page_subdomains(self):
         if 'landing_page' in self.columns:
             _loc = self.columns.get_loc('landing_page') + 1
@@ -430,14 +546,47 @@
             self._update_inplace(obj)
         else:
             return obj
 
     def bool_column_to_int(self, column_name):
         if column_name in self.columns:
             self[column_name] = self[column_name].apply(lambda b: 1 if b else 0)
+            
+    
+    def add_join_dimensions(self, dimensions: str | list[str]):
+        if isinstance(dimensions, str):
+            dimensions = [dimensions]
+        self.join_dimensions.extend(dimensions)
+        
+    def remove_join_dimensions(self, dimensions: str | list[str]):
+        if isinstance(dimensions, str):
+            dimensions = [dimensions]
+        for _d in dimensions:
+            self.join_dimensions = remove_list_item(self.join_dimensions, _d)
+
+    def fill_nan_with_zeros(self):
+        values = {_col: 0 for _col, _type in self.dtypes.items() if _type == 'float' or _type == 'int'}
+        self.fillna(value=values, inplace=True)
+
+    def join_on_dimensions(self, dataframe, how: str = "outer"):
+        if not set(self.join_dimensions) == set(dataframe.join_dimensions):
+            raise ValueError("Input dataframe must have same join_dimensions")
+
+        _out = GADataFrame(
+            df_input=pd.merge(self, dataframe, how=how, on=self.join_dimensions),
+            response_type=self.response_type,
+            dimensions=list(set(self.dimensions + dataframe.dimensions)),
+            metrics=list(set(self.metrics + dataframe.metrics)),
+            from_ga_response=False,
+            join_dimensions=self.join_dimensions,
+            start_date=min(self.date_range.get('start'), dataframe.date_range.get('start')),
+            end_date=max(self.date_range.get('end'), dataframe.date_range.get('end'))
+        )
+
+        return _out
 
 
 class GSCDataFrame(pd.DataFrame):
     """
     Subclass of pandas.DataFrame specifically for use with Google Search Console responses.
     The subclass must be initialized with a GSC response object and will create a dataframe
     from the report.
@@ -700,20 +849,26 @@
         return s
     elif s[:3] == 'ga:':
         return s[3:]
     else:
         return s
 
 
-def get_response_type(response: dict):
-    # Check for GA response
+def get_response_type(response: dict | RunReportResponse):
+    if isinstance(response, RunReportResponse):
+        return 'GA4'
+
+    if _t := response.get('response_type'):
+        return _t
+
+    # Check for GA3 response
     try:
         rows = response.get('reports', [])[0]['data']['rows']
         dimensions = response.get('reports')[0].get('columnHeader')['dimensions']
-        return 'GA'
+        return 'GA3'
     except (TypeError, IndexError, KeyError, AttributeError):
         pass
 
     # Check for GSC response
     try:
         if {'clicks', 'impressions', 'ctr', 'position'} < set(response.get('rows', [])[0].keys()):
             return 'GSC'
@@ -763,7 +918,8 @@
 
 def get_sub2(page_path: str):
     return get_sub_domain(page_path=page_path, n=2)
 
 
 def remove_list_item(_list, _item) -> list:
     return [_ for _ in _list if _ != _item]
+
```

### Comparing `pygoogalytics-0.3.2/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.4.0/pygoogalytics/kwp_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -633,15 +633,15 @@
         keyword_plan_campaign = operation.create
 
         keyword_plan_campaign.name = f"Keyword plan campaign {uuid.uuid4()}"
         keyword_plan_campaign.cpc_bid_micros = cpc_bid_micros
         keyword_plan_campaign.keyword_plan = keyword_plan
         keyword_plan_campaign.keyword_plan_network = network
 
-        # Other geo target constants can be referenced here:
+        # Other geotarget constants can be referenced here:
         # https://developers.google.com/google-ads/api/reference/data/geotargets
         for _loc in location_resources:
             geo_target = self.client.get_type("KeywordPlanGeoTarget", version="v12")
             # print('geo_target type: ')
             # print(type(geo_target))
             geo_target.geo_target_constant = _loc
             keyword_plan_campaign.geo_targets.append(geo_target)
```

### Comparing `pygoogalytics-0.3.2/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.4.0/pygoogalytics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.3.2
+Version: 0.4.0
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -14,21 +14,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 License-File: LICENSE
 
+<div id="badges">
+   <img src="https://img.shields.io/badge/3.10+-yellow?label=python&style=plastic&logo=python&logoColor=yellow" alt="Python version: 3.10 | 3.11">
+   <img src="https://img.shields.io/badge/UA (GA3) | GA4 | GSC | GoogleAds-green?label=API support&style=plastic&logo=googlecloud&logoColor=green" alt="Application support: GA3 | GSC | GoogleAds | SemRush | ScreamingFrog">
+   <img src="https://img.shields.io/badge/beta-red?label=stage&style=plastic&logoColor=blue" alt="Stage: beta">
+</div>
+
 ### Installation
 
 PyGoogalytics can be installed using [pip](https://pypi.org/project/pygoogalytics/):
 ```shell
 pip install -U pygoogalytics
 ```
 
+### Set-up
+
+Although PyGoogalytics is intended to be user-friendly it is still 
+necessary to set up various accounts and credentials with Google. 
+If you haven't yet setup API access for Universal Analytics, GA4, Search Console or Google Ads, follow [our instructions](setup_instruction.md) to get started.
+
+
 # Google Analytics API wrapper
 
 `client.py` defines the class `Client` which builds `googleapiclient.discovery` resources for accessing 
 Google Search Console and Google Analytics 3 (UA) data from the respective APIs, 
 and also `google.analytics.data_v1beta.BetaAnalyticsDataClient` resource for accessing GA4 data, although 
 currently this is only for testing.
```

### Comparing `pygoogalytics-0.3.2/setup.py` & `pygoogalytics-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.3.2',
+    version='0.4.0',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

