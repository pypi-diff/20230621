# Comparing `tmp/pygoogalytics-0.4.0.tar.gz` & `tmp/pygoogalytics-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.4.0.tar", last modified: Wed Jun 21 14:49:05 2023, max compression
+gzip compressed data, was "pygoogalytics-0.4.1.tar", last modified: Wed Jun 21 15:17:19 2023, max compression
```

## Comparing `pygoogalytics-0.4.0.tar` & `pygoogalytics-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 14:49:05.625703 pygoogalytics-0.4.0/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.4.0/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.4.0/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-06-21 14:49:05.625497 pygoogalytics-0.4.0/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.4.0/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 14:49:05.623771 pygoogalytics-0.4.0/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-06-21 14:48:42.000000 pygoogalytics-0.4.0/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     3239 2023-06-21 13:16:26.000000 pygoogalytics-0.4.0/pygoogalytics/ads_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)     5678 2023-06-21 13:16:26.000000 pygoogalytics-0.4.0/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 14:49:05.625081 pygoogalytics-0.4.0/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.4.0/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.4.0/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    43489 2023-06-21 14:15:30.000000 pygoogalytics-0.4.0/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    39357 2023-06-21 14:15:30.000000 pygoogalytics-0.4.0/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    42099 2023-05-09 12:29:00.000000 pygoogalytics-0.4.0/pygoogalytics/kwp_wrappers.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 14:49:05.624820 pygoogalytics-0.4.0/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      486 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-06-21 14:49:05.000000 pygoogalytics-0.4.0/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-06-21 14:49:05.625759 pygoogalytics-0.4.0/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-06-21 14:48:42.000000 pygoogalytics-0.4.0/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:17:19.060035 pygoogalytics-0.4.1/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.4.1/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.4.1/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-06-21 15:17:19.059895 pygoogalytics-0.4.1/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.4.1/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:17:19.058637 pygoogalytics-0.4.1/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-06-21 15:16:53.000000 pygoogalytics-0.4.1/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3239 2023-06-21 13:16:26.000000 pygoogalytics-0.4.1/pygoogalytics/ads_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5678 2023-06-21 13:16:26.000000 pygoogalytics-0.4.1/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:17:19.059670 pygoogalytics-0.4.1/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.4.1/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.4.1/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)    43521 2023-06-21 15:15:26.000000 pygoogalytics-0.4.1/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    39437 2023-06-21 15:15:26.000000 pygoogalytics-0.4.1/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    42099 2023-05-09 12:29:00.000000 pygoogalytics-0.4.1/pygoogalytics/kwp_wrappers.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:17:19.059382 pygoogalytics-0.4.1/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-06-21 15:17:19.000000 pygoogalytics-0.4.1/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      486 2023-06-21 15:17:19.000000 pygoogalytics-0.4.1/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-06-21 15:17:19.000000 pygoogalytics-0.4.1/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-06-21 15:17:19.000000 pygoogalytics-0.4.1/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-06-21 15:17:19.000000 pygoogalytics-0.4.1/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-06-21 15:17:19.060075 pygoogalytics-0.4.1/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-06-21 15:16:53.000000 pygoogalytics-0.4.1/setup.py
```

### Comparing `pygoogalytics-0.4.0/LICENCE.txt` & `pygoogalytics-0.4.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.0/LICENSE` & `pygoogalytics-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.0/PKG-INFO` & `pygoogalytics-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.4.0
+Version: 0.4.1
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.4.0/README.md` & `pygoogalytics-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.0/pygoogalytics/__init__.py` & `pygoogalytics-0.4.1/pygoogalytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.4.0/pygoogalytics/ads_wrapper.py` & `pygoogalytics-0.4.1/pygoogalytics/ads_wrapper.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.0/pygoogalytics/client.py` & `pygoogalytics-0.4.1/pygoogalytics/client.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.0/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.4.1/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.0/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.4.1/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.0/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.4.1/pygoogalytics/googalytics_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Union, Optional, Any
 
 from googleapiclient.errors import HttpError as GoogleApiHttpError
 from google.api_core.exceptions import ResourceExhausted, InvalidArgument, PermissionDenied
 import google.analytics.data_v1beta.types as ga_data_types
 
 from . import googlepandas as gpd
-from .utils import utils
+from .utils import general_utils
 from .utils.ga4_parser import parse_ga4_response
 from . import pga_logger
 
 
 class GoogalyticsWrapper:
     """
     The GoogalyticsWrapper requires the following arguments to access data:
@@ -46,17 +46,17 @@
         pga_logger.debug(f"initialising GoogalyticsWrapper object")
 
     # *****************************************************************
     # *** GAPI_WRAPPER STATS ******************************************
 
     def __dict__(self) -> dict:
         _dates_test = self.available_dates
-        gsc_date_range_str = utils.date_range_string(dates=_dates_test.get("GSC"),
+        gsc_date_range_str = general_utils.date_range_string(dates=_dates_test.get("GSC"),
                                                      alternate_text="No dates available from GSC")
-        ga3_date_range_str = utils.date_range_string(dates=_dates_test.get("GA3"),
+        ga3_date_range_str = general_utils.date_range_string(dates=_dates_test.get("GA3"),
                                                      alternate_text="No dates available from GA3")
 
         return {
             "API config": {
                 "GSC sc-domain": self.sc_domain,
                 "GA3 View ID": self.view_id,
                 "GA4 Property ID": self.ga4_property_id
@@ -120,15 +120,15 @@
     def api_test_gsc(self) -> dict:
         if self._api_test_gsc.get('status') is None:
             self._perform_api_test_gsc()
         return self._api_test_gsc
 
     @property
     def api_test_ga3(self) -> dict:
-        if self._api_test_ga3.get('status') is None or not utils.test_time(self._api_test_ga3.get('timestamp'), 3600):
+        if self._api_test_ga3.get('status') is None or not general_utils.test_time(self._api_test_ga3.get('timestamp'), 3600):
             self._perform_api_test_ga3()
         return self._api_test_ga3
 
     def _perform_api_test_ga3(self):
         """test GA API"""
         pga_logger.debug(f"{self.__class__.__name__}.api_test() :: testing GA api")
         _api_error = None
```

### Comparing `pygoogalytics-0.4.0/pygoogalytics/googlepandas.py` & `pygoogalytics-0.4.1/pygoogalytics/googlepandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 import pandas as pd
 import datetime
 
 from google.analytics.data_v1beta.types.analytics_data_api import RunReportResponse
 
 from typing import List, Optional, Union, Pattern
 
-from .utils import utils
+from .utils import general_utils
 from .utils.ga4_parser import parse_ga4_response
 
 gpd_logger = logging.getLogger("googlepandas")
 
 
 def camel_to_snake(string: str):
-    return utils.RE_C2S.sub('_', string).lower()
+    return general_utils.RE_C2S.sub('_', string).lower()
 
 
 GA_Types = {
     'ga:date': str,
     'ga:dateHourMinute': str,
     'ga:landingPagePath': str,
     'ga:pagePath': str,
@@ -299,17 +299,17 @@
                 self.remove_join_dimensions('landingPagePlusQueryString')
                 self.add_join_dimensions('landingPagePath')
 
             if 'itemPurchaseQuantity' in self.columns:
                 self.rename(columns={'itemPurchaseQuantity': 'itemQuantity'}, inplace=True)
 
             if 'landingPagePath' in self.columns:
-                self['landingPagePath'] = self['landingPagePath'].apply(utils.url_strip_domain)
+                self['landingPagePath'] = self['landingPagePath'].apply(general_utils.url_strip_domain)
                 self['landingPage'] = self['landingPagePath'].apply(lambda _u: _u.split('?')[0])
-                self['landingPageParameter'] = self['landingPagePath'].apply(utils.url_extract_parameter)
+                self['landingPageParameter'] = self['landingPagePath'].apply(general_utils.url_extract_parameter)
                 self.rename(columns={'landingPagePath': 'landingPageFull'}, inplace=True)
 
                 self.remove_join_dimensions('landingPagePath')
                 self.add_join_dimensions(['landingPageFull', 'landingPageParameter', 'landingPage'])
 
             if 'transactionsPerSession' in self.columns:
                 self.rename(columns={'transactionsPerSession': 'conversionRate'}, inplace=True)
@@ -643,17 +643,17 @@
                             )
             self.drop(columns='keys', inplace=True)
 
             if 'query' in self.columns:
                 self['query'] = self['query'].apply(lambda s: s.lower())
 
             if 'page' in self.columns:
-                self['landing_page_parameter'] = self['page'].apply(utils.url_extract_parameter)
-                self['landing_page'] = self['page'].apply(utils.strip_url)
-                self['landing_page_nodomain'] = self['page'].apply(utils.url_strip_domain)
+                self['landing_page_parameter'] = self['page'].apply(general_utils.url_extract_parameter)
+                self['landing_page'] = self['page'].apply(general_utils.strip_url)
+                self['landing_page_nodomain'] = self['page'].apply(general_utils.url_strip_domain)
                 self.rename(columns={'page': 'landing_page_full'}, inplace=True)
 
         if from_gsc_response is False and df_input is not None:
             self.dimensions = list(self.columns)
             self.metrics = []
             for metric in ['clicks', 'impressions', 'ctr', 'position']:
                 self.dimensions.remove(metric)
@@ -771,29 +771,29 @@
         if reset_index:
             return binned_df.reset_index()
         else:
             return binned_df
 
 
 def is_question(query: str) -> bool:
-    if utils.RE_QUESTION.match(query):
+    if general_utils.RE_QUESTION.match(query):
         return True
     else:
         return False
 
 
 def is_transactional(query: str) -> bool:
-    if utils.RE_TRANSACTIONAL.match(query):
+    if general_utils.RE_TRANSACTIONAL.match(query):
         return True
     else:
         return False
 
 
 def is_investigation(query: str) -> bool:
-    if utils.RE_INVESTIGATION.match(query):
+    if general_utils.RE_INVESTIGATION.match(query):
         return True
     else:
         return False
 
 
 def is_google_organic(source: str,
                       medium: str) -> bool:
```

### Comparing `pygoogalytics-0.4.0/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.4.1/pygoogalytics/kwp_wrappers.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.0/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.4.1/pygoogalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.4.0
+Version: 0.4.1
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.4.0/setup.py` & `pygoogalytics-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.4.0',
+    version='0.4.1',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

