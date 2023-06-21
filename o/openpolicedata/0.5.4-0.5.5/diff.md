# Comparing `tmp/openpolicedata-0.5.4.tar.gz` & `tmp/openpolicedata-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpolicedata-0.5.4.tar", last modified: Thu May 25 22:23:39 2023, max compression
+gzip compressed data, was "openpolicedata-0.5.5.tar", last modified: Wed Jun 21 00:37:17 2023, max compression
```

## Comparing `openpolicedata-0.5.4.tar` & `openpolicedata-0.5.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 22:23:39.062993 openpolicedata-0.5.4/
--rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.4/LICENSE
--rw-rw-rw-   0        0        0    14953 2023-05-25 22:23:39.062993 openpolicedata-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0    13810 2023-05-25 21:58:14.000000 openpolicedata-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 22:23:39.038732 openpolicedata-0.5.4/openpolicedata/
--rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.4/openpolicedata/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-25 21:52:33.000000 openpolicedata-0.5.4/openpolicedata/_version.py
--rw-rw-rw-   0        0        0    27852 2023-05-25 21:49:05.000000 openpolicedata-0.5.4/openpolicedata/data.py
--rw-rw-rw-   0        0        0    76703 2023-05-25 21:52:20.000000 openpolicedata-0.5.4/openpolicedata/data_loaders.py
--rw-rw-rw-   0        0        0    10789 2023-05-25 22:01:01.000000 openpolicedata-0.5.4/openpolicedata/datasets.py
--rw-rw-rw-   0        0        0     8688 2023-05-25 21:49:05.000000 openpolicedata-0.5.4/openpolicedata/defs.py
--rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.4/openpolicedata/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:23:39.050165 openpolicedata-0.5.4/openpolicedata.egg-info/
--rw-rw-rw-   0        0        0    14953 2023-05-25 22:23:38.000000 openpolicedata-0.5.4/openpolicedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-05-25 22:23:39.000000 openpolicedata-0.5.4/openpolicedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 22:23:38.000000 openpolicedata-0.5.4/openpolicedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-25 22:23:38.000000 openpolicedata-0.5.4/openpolicedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-25 22:23:38.000000 openpolicedata-0.5.4/openpolicedata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      426 2023-02-11 00:12:22.000000 openpolicedata-0.5.4/pyproject.toml
--rw-rw-rw-   0        0        0     1369 2023-05-25 22:23:39.063996 openpolicedata-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:23:39.060994 openpolicedata-0.5.4/tests/
--rw-rw-rw-   0        0        0    21379 2023-05-17 22:48:02.000000 openpolicedata-0.5.4/tests/test_data_loaders.py
--rw-rw-rw-   0        0        0     9154 2023-05-17 22:48:02.000000 openpolicedata-0.5.4/tests/test_datasets.py
--rw-rw-rw-   0        0        0    11172 2023-05-17 22:48:02.000000 openpolicedata-0.5.4/tests/test_opd_data1.py
--rw-rw-rw-   0        0        0     7997 2023-05-17 22:48:02.000000 openpolicedata-0.5.4/tests/test_opd_data2.py
--rw-rw-rw-   0        0        0    11428 2023-05-25 21:49:05.000000 openpolicedata-0.5.4/tests/test_opd_data3.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:37:17.897311 openpolicedata-0.5.5/
+-rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0    14967 2023-06-21 00:37:17.897311 openpolicedata-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13825 2023-06-21 00:05:22.000000 openpolicedata-0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 00:37:17.851312 openpolicedata-0.5.5/openpolicedata/
+-rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.5/openpolicedata/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-06-21 00:04:59.000000 openpolicedata-0.5.5/openpolicedata/_version.py
+-rw-rw-rw-   0        0        0    30791 2023-06-16 21:55:53.000000 openpolicedata-0.5.5/openpolicedata/data.py
+-rw-rw-rw-   0        0        0    77576 2023-06-19 21:11:56.000000 openpolicedata-0.5.5/openpolicedata/data_loaders.py
+-rw-rw-rw-   0        0        0    11480 2023-06-19 21:25:39.000000 openpolicedata-0.5.5/openpolicedata/datasets.py
+-rw-rw-rw-   0        0        0     8688 2023-06-03 12:50:40.000000 openpolicedata-0.5.5/openpolicedata/defs.py
+-rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.5/openpolicedata/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:37:17.887314 openpolicedata-0.5.5/openpolicedata.egg-info/
+-rw-rw-rw-   0        0        0    14967 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 00:37:17.000000 openpolicedata-0.5.5/openpolicedata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      426 2023-02-11 00:12:22.000000 openpolicedata-0.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1377 2023-06-21 00:37:17.898312 openpolicedata-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 00:37:17.896312 openpolicedata-0.5.5/tests/
+-rw-rw-rw-   0        0        0    21379 2023-05-17 22:48:02.000000 openpolicedata-0.5.5/tests/test_data_loaders.py
+-rw-rw-rw-   0        0        0     9438 2023-06-20 11:16:04.000000 openpolicedata-0.5.5/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    11536 2023-06-21 00:35:42.000000 openpolicedata-0.5.5/tests/test_opd_data1.py
+-rw-rw-rw-   0        0        0     7998 2023-06-16 21:56:15.000000 openpolicedata-0.5.5/tests/test_opd_data2.py
+-rw-rw-rw-   0        0        0    11429 2023-06-15 23:29:48.000000 openpolicedata-0.5.5/tests/test_opd_data3.py
```

### Comparing `openpolicedata-0.5.4/LICENSE` & `openpolicedata-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.4/PKG-INFO` & `openpolicedata-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.4
+Version: 0.5.5
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: rapidfuzz
+Provides-Extra: optional
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-OpenPoliceData is a Python package that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
```

### Comparing `openpolicedata-0.5.4/README.md` & `openpolicedata-0.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-OpenPoliceData is a Python package that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
```

### Comparing `openpolicedata-0.5.4/openpolicedata/__init__.py` & `openpolicedata-0.5.5/openpolicedata/__init__.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.4/openpolicedata/data.py` & `openpolicedata-0.5.5/openpolicedata/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 import numbers
 import os.path as path
 import pandas as pd
 from datetime import datetime
 from dateutil.parser._parser import ParserError
 from packaging import version
 import re
+from typing import Iterator, List, Optional, Union
 import warnings
 
-if __name__ == '__main__':
-    import data_loaders
-    import datasets
-    # import preproc
-    from defs import TableType, DataType, MULTI, NA
-    from _version import __version__
-    import exceptions
-else:
-    from . import data_loaders
-    from . import datasets
-    from . import __version__
-    # from . import preproc
-    from .defs import TableType, DataType, MULTI, NA
-    from . import exceptions
+from . import data_loaders
+from . import datasets
+from . import __version__
+# from . import preproc
+from .defs import TableType, DataType, MULTI, NA
+from . import exceptions
 
 class Table:
     """
     A class that contains a DataFrame for a dataset along with meta information
 
     Attributes
     ----------
@@ -51,33 +44,40 @@
     -------
     to_csv(output_dir=None, filename=None)
         Convert table to CSV file
     get_csv_filename()
         Get default name of CSV file
     """
 
-    details = None
-    state = None
-    source_name = None
-    agency = None
-    table_type = None
-    year = None
-    description = None
-    url = None
+    details: str= None
+    state: str = None
+    source_name: str = None
+    agency: str = None
+    table_type: TableType = None
+    year: Union[int, str, List[int]] = None
+    description: str = None
+    url: str = None
+    source_url: str = None
+    readme: Optional[str] = None
 
     # Data
-    table = None
+    table: Optional[pd.DataFrame] = None
 
     # From source
-    _data_type = None
-    _dataset_id = None
-    _date_field = None
-    _agency_field = None
-
-    def __init__(self, source, table=None, year_filter=None, agency=None):
+    _data_type: str = None
+    _dataset_id: Optional[str] = None
+    _date_field: Optional[str] = None
+    _agency_field: Optional[str] = None
+
+    def __init__(self, 
+        source: Union[pd.DataFrame, pd.Series], 
+        table: Optional[pd.DataFrame] = None, 
+        year_filter: Union[str, int, List[int]] = None, 
+        agency: Optional[str] = None
+        ) -> None:
         '''Construct Table object
         This is intended to be generated by the Source.load_from_url and Source.load_from_csv classes
 
         Parameters
         ----------
         source : pandas or geopandas Series
             Series containing information on the source
@@ -126,20 +126,29 @@
 
         if not pd.isnull(source["date_field"]):
             self._date_field = source["date_field"]
         
         if not pd.isnull(source["agency_field"]):
             self._agency_field = source["agency_field"]
 
+        if not pd.isnull(source["source_url"]):
+            self.source_url = source["source_url"]
+
+        if not pd.isnull(source["readme"]):
+            self.readme = source["readme"]
+
 
     def __repr__(self) -> str:
         skip = ["details", "table"]
         return ',\n'.join("%s: %s" % item for item in vars(self).items() if (item[0] not in skip and item[0][0] != "_"))
 
-    def to_csv(self, output_dir=None, filename=None):
+    def to_csv(self, 
+               output_dir: Optional[str] = None, 
+               filename: Optional[str] = None
+               ) -> str:
         '''Export table to CSV file. Use default filename for data that will
         be reloaded as an openpolicedata Table object
 
         Parameters
         ----------
         output_dir - str
             (Optional) Output directory. Default: current directory
@@ -154,15 +163,15 @@
             raise ValueError("There is no table to save to CSV")
 
         self.table.to_csv(filename, index=False, errors="surrogateescape")
 
         return filename
 
 
-    def get_csv_filename(self):
+    def get_csv_filename(self) -> str:
         '''Generate default filename based on table parameters
 
         Returns
         -------
         str
             Filename
         '''
@@ -190,18 +199,21 @@
         Get agencies available for 1 or more datasets
     load_from_url()
         Load data from URL
     load_from_csv()
         Load data from a previously saved CSV file
     """
 
-    datasets = None
+    datasets: pd.DataFrame = None
     __loader = None
 
-    def __init__(self, source_name, state=None):
+    def __init__(self, 
+                source_name: str, 
+                state: Optional[str] =None
+                ) -> None:
         '''Constructor for Source class
 
         Parameters
         ----------
         source_name - str
             Source name from datasets table
         state - str
@@ -220,26 +232,30 @@
             raise ValueError("Not all sources are from the same state")
 
 
     def __repr__(self) -> str:
         return str(self.datasets)
 
 
-    def get_tables_types(self):
+    def get_tables_types(self) -> List[str]:
         '''Get types of data availble from the source
 
         Returns
         -------
         list
             List containing types of data available from source
         '''
         return list(self.datasets["TableType"].unique())
 
 
-    def get_years(self, table_type, force=False, manual=False):
+    def get_years(self, 
+        table_type: Union[str, TableType], 
+        force: bool = False, 
+        manual: bool = False
+        ) -> List[int]:
         '''Get years available for 1 or more datasets
 
         Parameters
         ----------
         table_type - str or TableType enum
             Only returns years for requested table type
         force - bool
@@ -252,48 +268,50 @@
         list
             List of years available for 1 or more datasets
         '''
         dfs = self.__find_datasets(table_type)
 
         cur_year = datetime.now().year
         all_years = list(dfs["Year"])
-        years = set()
-        for k in range(len(all_years)):
-            if all_years[k] != MULTI:
-                years.add(all_years[k])
-            else:
-                df = dfs.iloc[k]
-                _check_version(df)
-                data_type =DataType(df["DataType"])
-                url = df["URL"]
-                date_field = df["date_field"] if pd.notnull(df["date_field"]) else None
-                
-                loader = self.__get_loader(data_type, url, dataset_id=df["dataset_id"], date_field=date_field)
+        years = {x for x in all_years if isinstance(x,numbers.Number) or x==NA}
+        for k in [k for k,x in enumerate(all_years) if x==MULTI]:
+            df = dfs.iloc[k]
+            _check_version(df)
+            data_type =DataType(df["DataType"])
+            url = df["URL"]
+            date_field = df["date_field"] if pd.notnull(df["date_field"]) else None
+            
+            loader = self.__get_loader(data_type, url, dataset_id=df["dataset_id"], date_field=date_field)
 
-                check = None
-                if not manual and pd.notnull(df["coverage_start"]) and pd.notnull(df["coverage_end"]) and \
-                    hasattr(df["coverage_start"], 'year') and hasattr(df["coverage_end"], 'year'):
-                    years.update(range(df["coverage_start"].year, df["coverage_end"].year+1))
-                    if df["coverage_end"].year >= cur_year-2:
-                        # Check for updates
-                        check = [x for x in range(df["coverage_end"].year+1,cur_year+1)]
-                        if len(check)>0:
-                            new_years = loader.get_years(force=force, check=check)
-                            years.update(new_years)
-                else:
-                    new_years = loader.get_years(force=force)
-                    years.update(new_years)
+            check = None
+            if not manual and pd.notnull(df["coverage_start"]) and pd.notnull(df["coverage_end"]) and \
+                hasattr(df["coverage_start"], 'year') and hasattr(df["coverage_end"], 'year'):
+                years.update(range(df["coverage_start"].year, df["coverage_end"].year+1))
+                max_year = max(years)
+                if  cur_year-2 <= max_year < cur_year:
+                    # Check for updates
+                    check = [x for x in range(max_year+1,cur_year+1)]
+                    if len(check)>0:
+                        new_years = loader.get_years(force=force, check=check)
+                        years.update(new_years)
+            else:
+                new_years = loader.get_years(force=force)
+                years.update(new_years)
             
         years = list(years)
         years.sort()
 
         return years
 
 
-    def get_agencies(self, table_type=None, year=None, partial_name=None):
+    def get_agencies(self, 
+                     table_type: Union[str, TableType, None] = None, 
+                     year: Union[str, int, None] = None, 
+                     partial_name: Optional[str] = None
+                     ) -> List[str]:
         '''Get agencies available for 1 or more datasets
 
         Parameters
         ----------
         table_type - str or TableType enum
             (Optional) If set, only returns agencies for requested table type
         year - int or the strings opd.defs.MULTI or opd.defs.NONE
@@ -344,15 +362,20 @@
                 return list(agency_set)
             else:
                 raise ValueError(f"Unknown data type: {data_type}")
         else:
             return [src["Agency"]]
 
 
-    def get_count(self, year=None, table_type=None, agency=None, force=False):
+    def get_count(self, 
+                  year: Union[str, int, List[int], None] = None,
+                  table_type: Union[str, TableType, None] = None, 
+                  agency: Optional[str] = None, 
+                  force: bool = False
+                  ) -> int:
         '''Get number of records for a data request
 
         Parameters
         ----------
         year (Optional) - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
@@ -373,15 +396,23 @@
         Table
             Table object containing the requested data
         '''
 
         return self.__load(year, table_type, agency, True, pbar=False, return_count=True, force=force)
     
     
-    def load_from_url_gen(self, year, table_type=None, agency=None, pbar=False, nbatch=10000, offset=0, force=False):
+    def load_from_url_gen(self, 
+                          year: Union[str, int, List[int]], 
+                          table_type: Union[str, TableType, None] = None, 
+                          agency: Optional[str] = None, 
+                          pbar: bool = False, 
+                          nbatch: int = 10000, 
+                          offset: int = 0, 
+                          force: bool =False
+                          ) -> Iterator[Table]:
         '''Get generator to load data from URL in batches
 
         Parameters
         ----------
         year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
@@ -410,16 +441,22 @@
         '''
 
         count = self.get_count(year, table_type, agency, force)
         for k in range(offset, count, nbatch):
             yield self.__load(year, table_type, agency, True, pbar, nrows=min(nbatch, count-k), offset=k)
     
         
-
-    def load_from_url(self, year, table_type=None, agency=None, pbar=True, nrows=None, offset=0):
+    def load_from_url(self, 
+                      year: Union[str, int, List[int]], 
+                      table_type: Union[str, TableType, None] = None, 
+                      agency: Optional[str] = None,
+                      pbar: bool = True,
+                      nrows: Optional[int] = None, 
+                      offset: int = 0
+                      ) -> Table:
         '''Load data from URL
 
         Parameters
         ----------
         year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
@@ -530,22 +567,28 @@
                 agency = agency.replace("'","''")
                 opt_filter = agency_field + " = '" + agency + "'"
             
             if return_count:
                 return loader.get_count(year=year_filter, agency=agency, opt_filter=opt_filter, force=force)
             else:
                 table = loader.load(year=year_filter, agency=agency, opt_filter=opt_filter, nrows=nrows, pbar=pbar, offset=offset)
-                table = _check_date(table, date_field)                        
+                date_field = self.__fix_date_field(table, date_field, src.name)
+                table = _check_date(table, date_field)
         else:
             table = None
 
         return Table(src, table, year_filter=table_year, agency=table_agency)
 
 
-    def load_from_csv(self, year, output_dir=None, table_type=None, agency=None):
+    def load_from_csv(self, 
+                      year: Union[str, int, List[int]],
+                      output_dir: Optional[str] = None, 
+                      table_type: Union[str, TableType, None] = None,
+                      agency: Optional[str] = None
+                      ) -> Table:
         '''Load data from previously saved CSV file
         
         Parameters
         ----------
         year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
@@ -568,19 +611,25 @@
         table = self.__load(year, table_type, agency, False)
 
         filename = table.get_csv_filename()
         if output_dir != None:
             filename = path.join(output_dir, filename)            
 
         table.table = pd.read_csv(filename, parse_dates=True)
+        table._date_field = self.__fix_date_field(table.table, table._date_field, table.details.name)
         table.table = _check_date(table.table, table._date_field)  
 
         return table
 
-    def get_csv_filename(self, year, output_dir=None, table_type=None, agency=None):
+    def get_csv_filename(self, 
+                         year: Union[str, int, List[int]],
+                         output_dir: Optional[str] = None, 
+                         table_type: Union[str, TableType, None] = None,
+                         agency: Optional[str] = None
+                         ) -> str:
         '''Get auto-generated CSV filename
         
         Parameters
         ----------
         year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
@@ -627,14 +676,26 @@
             loader = data_loaders.Carto(url, dataset_id, date_field=date_field)
         else:
             raise ValueError(f"Unknown data type: {data_type}")
 
         self.__loader = (params, loader)
 
         return loader
+    
+    def __fix_date_field(self, table, date_field, loc):
+        if date_field != None and table is not None and len(table)>0 and date_field not in table and \
+            any([x.lower()==date_field.lower() for x in table.columns]):
+            # Instances have been found where capitalization changes
+            date_field = [x for x in table.columns if x.lower()==date_field.lower()][0]
+            # Correct date field in tables
+            self.datasets.loc[loc, "date_field"] = date_field
+            datasets.datasets.loc[loc, "date_field"] = date_field
+
+        return date_field
+
 
 def _check_date(table, date_field):
     if date_field != None and table is not None and len(table)>0:
         dts = table[date_field]
         dts = dts[dts.notnull()]
         if len(dts) > 0:
             one_date = dts.iloc[0]  
@@ -661,15 +722,21 @@
             # Replace bad dates with NaT
             table[date_field].replace(datetime.strptime('1900-01-01 00:00:00', '%Y-%m-%d %H:%M:%S'), pd.NaT, inplace=True)
 
 
     return table
 
 
-def get_csv_filename(state, source_name, agency, table_type, year):
+def get_csv_filename(
+    state: str, 
+    source_name: str, 
+    agency: str, 
+    table_type: Union[str, TableType], 
+    year: Union[str, int, List[int]]
+    ) -> str:
     '''Get default CSV filename for the given parameters. Enables reloading of data from CSV.
     
     Parameters
     ----------
     state - str
         Name of state
     source_name - str
@@ -710,15 +777,15 @@
 def _check_version(df):
     min_version = df["min_version"] 
     if pd.notnull(min_version):
         src_name = df["SourceName"]
         state = df["State"]
         table_type = df["TableType"]
         year = df["Year"]
-        if min_version == "-1":
+        if min_version.strip() == "-1":
             raise exceptions.OPD_FutureError(
                 f"Year {year} {table_type} data for {src_name} in {state} cannot be loaded in this version. " + \
                     "It will be made available in a future release"
             )
         elif version.parse(__version__) < version.parse(min_version):
             raise exceptions.OPD_MinVersionError(
                 f"Year {year} {table_type} data for {src_name} in {state} cannot be loaded in version {__version__} of openpolicedata. " + \
```

### Comparing `openpolicedata-0.5.4/openpolicedata/data_loaders.py` & `openpolicedata-0.5.5/openpolicedata/data_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_datetime64_any_dtype as is_datetime
 from numpy import nan
 import requests
 import urllib
 import urllib3
-import ssl
 from abc import ABC, abstractmethod
 from sodapy import Socrata as SocrataClient
-from pyproj.exceptions import CRSError
-from pyproj import CRS
 import warnings
 from time import sleep
 from tqdm import tqdm
 from math import ceil
 import re
 from xlrd.biffh import XLRDError
+from zipfile import ZipFile
 
 try:
     import geopandas as gpd
     from shapely.geometry import Point
     _has_gpd = True
 except:
     _has_gpd = False
@@ -81,14 +79,19 @@
 
     def init_poolmanager(self, connections, maxsize, block=False):
         self.poolmanager = urllib3.poolmanager.PoolManager(
             num_pools=connections, maxsize=maxsize,
             block=block, ssl_context=self.ssl_context)
         
 def get_legacy_session():
+    try:
+        import ssl
+    except:
+        raise ImportError(f"Loading this dataset requires the SSL package, which typically comes with the Python installation" + 
+                          " but is not for some Python versions like the one used by Jupyter Lite. To install, run 'pip install ssl'")
     ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
     ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
     session = requests.session()
     session.mount('https://', CustomHttpAdapter(ctx))
     return session
 
 
@@ -406,15 +409,26 @@
         '''
         
         self.url = url
         self.date_field = date_field
         self.agency_field = agency_field
         
         try:
-            self.excel_file = pd.ExcelFile(url)
+            if ".zip" in self.url:
+                # Download file to temporary file
+                r = requests.get(url)
+                r.raise_for_status()
+                with tempfile.TemporaryFile(suffix=".zip") as fp:
+                    fp.write(r.content)
+                    fp.seek(0)
+
+                    z = ZipFile(fp, 'r')
+                    self.excel_file = pd.ExcelFile(BytesIO(z.read(z.namelist()[0])))
+            else:
+                self.excel_file = pd.ExcelFile(url)
         except urllib.error.HTTPError as e:
             if str(e) in ["HTTP Error 406: Not Acceptable", 'HTTP Error 403: Forbidden']:
                 # 406 error: https://stackoverflow.com/questions/34832970/http-error-406-not-acceptable-python-urllib2
                 # File-like input for URL: https://stackoverflow.com/questions/57815780/how-can-i-directly-handle-excel-file-link-python/57815864#57815864
                 headers = {'User-agent' : 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14 (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'}
                 r = requests.get(url, stream=True, headers=headers)
                 r.raise_for_status()
@@ -1172,14 +1186,18 @@
                     if not _has_gpd and _use_gpd_force:
                         raise ValueError("User cannot force GeoPandas usage when it is not installed")
                     use_gpd = _use_gpd_force
                 else:
                     use_gpd = _has_gpd
 
                 if use_gpd:
+                    # pyproj installs with geopandas
+                    from pyproj.exceptions import CRSError
+                    from pyproj import CRS
+
                     geometry = []
                     for feat in features:
                         if "geometry" not in feat:
                             geometry.append(None)
                         elif feat["geometry"]["x"]=="NaN":
                             geometry.append(Point(nan, nan))
                         else:
@@ -1753,15 +1771,15 @@
     if date_field != None and not hasattr(df[date_field], "dt"):
         with warnings.catch_warnings():
             # Ignore future warning about how this operation will be attempted to be done inplace:
             # In a future version, `df.iloc[:, i] = newvals` will attempt to set the values inplace instead of always setting a new array. 
             # To retain the old behavior, use either `df[df.columns[i]] = newvals` or, if columns are non-unique, `df.isetitem(i, newvals)`
             warnings.simplefilter("ignore", category=FutureWarning)
             if date_field.lower()!="year":
-                df.loc[:, date_field] = pd.to_datetime(df[date_field])
+                df[date_field] = pd.to_datetime(df[date_field])
     
     if year_filter != None and date_field != None:
         if isinstance(year_filter, list):
             df = df[(df[date_field].dt.year >= year_filter[0]) & (df[date_field].dt.year <= year_filter[1])]
         else:
             date_col = pd.to_datetime(df[date_field])
             df = df[date_col.dt.year == year_filter]
```

### Comparing `openpolicedata-0.5.4/openpolicedata/datasets.py` & `openpolicedata-0.5.5/openpolicedata/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pandas as pd
 import numpy as np
 import re
+from typing import Optional, Union
 import warnings
 
-try:
-    from . import defs
-except:
-    import defs
+from . import defs
 
 # Location of table where datasets available in opd are stored
 csv_file = "https://raw.github.com/openpolicedata/opd-data/main/opd_source_table.csv"
 
 def _build(csv_file):
     # Check columns
     columns = {
@@ -77,15 +75,20 @@
         df["coverage_end"] = df["coverage_end"].apply(lambda x: pd.to_datetime(x) if pd.notnull(x) and p.search(x) else x)
 
     return df
 
 
 datasets = _build(csv_file)
 
-def query(source_name=None, state=None, agency=None, table_type=None):
+def query(
+    source_name: Optional[str] = None, 
+    state: Optional[str] = None, 
+    agency: Optional[str] = None,
+    table_type: Union[str,defs.TableType,None] = None
+) -> pd.DataFrame:
     """Query for available datasets.
     Request a DataFrame containing available datasets based on input filters.
     Returns all datasets if no filters applied.
     
     Parameters
     ----------
     source_name : str
@@ -117,26 +120,39 @@
         query_str += "TableType == '" + table_type + "' and "
 
     if len(query_str) == 0:
         return datasets.copy()
     else:
         return datasets.query(query_str[0:-5]).copy()
 
-def num_unique():
+def num_unique() -> int:
+    """_summary_
+
+    Returns:
+        int: _description_
+    """
     return len(query().drop_duplicates(["State","SourceName","Agency","TableType"]))
 
-def num_sources(full_states_only=False):
+def num_sources(full_states_only: bool = False) -> int:
+    """_summary_
+
+    Args:
+        full_states_only (bool, optional): _description_. Defaults to False.
+
+    Returns:
+        int: _description_
+    """
     d = query().drop_duplicates(subset=["State","SourceName","Agency"])
 
     if full_states_only:
         return ((d["State"]==d["SourceName"]) & (d["Agency"]==defs.MULTI)).sum()
     else:
         return len(d)
 
-def summary_by_state(by=None):
+def summary_by_state(by: Optional[str] = None) -> pd.DataFrame:
     df = query()
     df_unique = df.drop_duplicates(["State","SourceName","Agency","TableType"])
     s = df_unique.groupby("State").size()
     out = pd.DataFrame(s,columns=["Total"])
 
     by_year = type(by)==str and by.lower() == "year"
     by_table = type(by)==str and by.lower() == "table"
@@ -192,15 +208,15 @@
             k = len(out_start) + len(out_cur) 
         else:
             k+=1
 
     out.index.name = "State"
     return out
 
-def summary_by_table_type(by_year=False):
+def summary_by_table_type(by_year: bool = False) -> pd.DataFrame:
     df = query()
     s = df.drop_duplicates(["State","SourceName","Agency","TableType"]).groupby("TableType").size()
     out = pd.DataFrame(s,columns=["Total"])
     if by_year:
         s = df.drop_duplicates(["State","SourceName","Agency","TableType","Year"]).groupby(["TableType","Year"]).size().unstack()
         s = s.fillna(0).convert_dtypes(convert_integer=True)
         s = s[s.columns[::-1]]
@@ -215,55 +231,60 @@
         except:
             warnings.warn(f"{x} is not a known table type in defs.TableType")
             definitions.append("")
 
     out["Definition"] = definitions
 
     # Group related tables
-    groups = ["STOPS", "CITATIONS","ARRESTS","WARNINGS","OFFICER-INVOLVED SHOOTINGS","USE OF FORCE"]
+    groups = ["STOPS", "CITATIONS","ARRESTS","WARNINGS","OFFICER-INVOLVED SHOOTINGS","USE OF FORCE",
+              "CRASHES", "COMPLAINTS"]
     k = 0
     empty_row = ["" for _ in out.columns]
     while k < len(out):
         cur_group = [x for x in groups if x in out.index[k]]
         if len(cur_group)==0:
             k+=1
             continue
         elif len(cur_group)>1:
             raise ValueError("Multiple groups found")
         
         cur_group = cur_group[0]
 
         matches = [x for x in out.index if cur_group in x]
-        multi_table = any(["INCIDENT" in x for x in matches]) and \
-            (any(["OFFICER" in x for x in matches]) or any(["CIVILIAN" in x for x in matches]))
+        multi_table = any(["INCIDENT" in x for x in matches]) or \
+            any(["OFFICER" in x for x in matches]) or any(["CIVILIAN" in x for x in matches])
 
         out_start = out.iloc[0:k]
         out_end = out.iloc[k:].drop(index=matches)
         out_cur = out.loc[matches]
 
         if multi_table: 
-            index = [cur_group, "  Single Table", "    "+cur_group, "  Multiple Tables"]
-            index.extend(["    "+x for x in matches if x!=cur_group])
+            index = [cur_group+"-RELATED", "  Single Table  ", "    "+cur_group, "  Multi-Table  "]
+            index.extend(["    "+x+"    " for x in matches if x!=cur_group])
             out_cur = pd.concat([
                 pd.DataFrame([empty_row,empty_row],columns=out.columns),
                 pd.DataFrame([out_cur.loc[cur_group]],columns=out.columns),
                 pd.DataFrame([empty_row],columns=out.columns),
                 out_cur.loc[[x for x in matches if x!=cur_group]]
                 ],ignore_index=True)  
             out_cur.index = index  
         else:
             out_cur.rename(index={cur_group : cur_group+" (All)"}, inplace=True)
             out_cur.rename(index={x:x+" (Only)" for x in out_cur.index if "(All)" not in x}, inplace=True)
-            out_cur.rename(index={x:"  "+x for x in out_cur.index}, inplace=True)
+            out_cur.rename(index={x:"  "+x+"  " for x in out_cur.index}, inplace=True)
             # Add empty row for spacing
-            out_cur  = pd.concat([pd.DataFrame([empty_row],index=[cur_group],columns=out.columns),out_cur],axis=0)
+            out_cur  = pd.concat([pd.DataFrame([empty_row],index=[cur_group+"-RELATED"],columns=out.columns),out_cur],axis=0)
             # Find all indices for group
         
         out = pd.concat([out_start,out_cur,out_end],axis=0)
         k = len(out_start) + len(out_cur)
 
     out.index.name = "TableType"
     return out
 
-
-if __name__=="__main__":
-    print(summary_by_state(by="table").head(10))
+def get_table_types(contains=None):
+    df = query()
+    table_types = df["TableType"].unique()
+    if contains is not None:
+        table_types = [x for x in table_types if contains.lower() in x.lower()]
+    table_types.sort()
+    return table_types
```

### Comparing `openpolicedata-0.5.4/openpolicedata/defs.py` & `openpolicedata-0.5.5/openpolicedata/defs.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.4/openpolicedata/exceptions.py` & `openpolicedata-0.5.5/openpolicedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.4/openpolicedata.egg-info/PKG-INFO` & `openpolicedata-0.5.5/openpolicedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.4
+Version: 0.5.5
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: rapidfuzz
+Provides-Extra: optional
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://openpolicedata.streamlit.app)
 
 # OpenPoliceData
-OpenPoliceData is a Python package that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python library that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
```

### Comparing `openpolicedata-0.5.4/openpolicedata.egg-info/SOURCES.txt` & `openpolicedata-0.5.5/openpolicedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.4/setup.cfg` & `openpolicedata-0.5.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -68,19 +68,20 @@
 00000430: 0d0a 093d 202e 0d0a 7061 636b 6167 6573  ...= ...packages
 00000440: 203d 206f 7065 6e70 6f6c 6963 6564 6174   = openpolicedat
 00000450: 610d 0a70 7974 686f 6e5f 7265 7175 6972  a..python_requir
 00000460: 6573 203d 203e 3d33 2e37 0d0a 696e 7374  es = >=3.7..inst
 00000470: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
 00000480: 0a09 6f70 656e 7079 786c 0d0a 096e 756d  ..openpyxl...num
 00000490: 7079 0d0a 0970 6163 6b61 6769 6e67 0d0a  py...packaging..
-000004a0: 0970 616e 6461 730d 0a09 7079 7072 6f6a  .pandas...pyproj
-000004b0: 0d0a 0972 6571 7565 7374 730d 0a09 736f  ...requests...so
-000004c0: 6461 7079 0d0a 0974 7164 6d0d 0a09 786c  dapy...tqdm...xl
-000004d0: 7264 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rd....[options.e
-000004e0: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
-000004f0: 7261 7069 6466 757a 7a20 3d20 7261 7069  rapidfuzz = rapi
-00000500: 6466 757a 7a0d 0a0d 0a5b 6f70 7469 6f6e  dfuzz....[option
-00000510: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000520: 0d0a 7768 6572 6520 3d20 2e0d 0a0d 0a5b  ..where = .....[
-00000530: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000540: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000550: 6520 3d20 300d 0a0d 0a                   e = 0....
+000004a0: 0970 616e 6461 730d 0a09 7265 7175 6573  .pandas...reques
+000004b0: 7473 0d0a 0973 6f64 6170 790d 0a09 7471  ts...sodapy...tq
+000004c0: 646d 0d0a 0978 6c72 640d 0a0d 0a5b 6f70  dm...xlrd....[op
+000004d0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+000004e0: 7569 7265 5d0d 0a6f 7074 696f 6e61 6c20  uire]..optional 
+000004f0: 3d20 7261 7069 6466 757a 7a3b 206d 736f  = rapidfuzz; mso
+00000500: 6666 6372 7970 746f 2d74 6f6f 6c0d 0a0d  ffcrypto-tool...
+00000510: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000520: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+00000530: 3d20 2e0d 0a0d 0a5b 6567 675f 696e 666f  = .....[egg_info
+00000540: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000550: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000560: 0a                                       .
```

### Comparing `openpolicedata-0.5.4/tests/test_data_loaders.py` & `openpolicedata-0.5.5/tests/test_data_loaders.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.4/tests/test_datasets.py` & `openpolicedata-0.5.5/tests/test_datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,16 +188,19 @@
         opd.datasets.summary_by_state(by="TABLE")
         opd.datasets.summary_by_table_type()
         opd.datasets.summary_by_table_type(by_year=True)
 
         opd.datasets.datasets.loc[0,"TableType"] = "TEST"
         with pytest.warns(UserWarning):
             opd.datasets.summary_by_table_type()
-        
-        
+
+    def test_get_table_types(self, csvfile, source, last, skip, loghtml):    
+        opd.datasets.get_table_types()
+        assert opd.datasets.get_table_types(contains="STOPS") == ["PEDESTRIAN STOPS","STOPS","TRAFFIC STOPS"]
 
 if __name__ == "__main__":
     csvfile = None
-    csvfile = "C:\\Users\\matth\\repos\\opd-data\\opd_source_table.csv"
+    # csvfile = "C:\\Users\\matth\\repos\\opd-data\\opd_source_table.csv"
+    TestDatasets().test_get_table_types(csvfile,None,None,None,None)
     TestDatasets().test_table_for_nulls(csvfile,None,None,None,None)
     # TestDatasets().test_years_multi(csvfile,None,None,None,None)
     # TestDatasets().test_table_types(csvfile,None,None,None,None)
```

### Comparing `openpolicedata-0.5.4/tests/test_opd_data1.py` & `openpolicedata-0.5.5/tests/test_opd_data1.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 warn_errors = (OPD_DataUnavailableError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError)
 
 def get_datasets(csvfile):
     if csvfile != None:
         datasets.datasets = datasets._build(csvfile)
 
-    return datasets.query()
+    return datasets.datasets
 
 class TestData:
 	def check_table_type_warning(self, csvfile, source, last, skip, loghtml):
 		sources = datasets.query().copy().iloc[0]
 		sources["TableType"] = "TEST"
 		with pytest.warns(UserWarning):
 			data.Table(sources)
@@ -286,20 +286,29 @@
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
 	csvfile = r"..\opd-data\opd_source_table.csv"
 	last = None
-	last = 873-290+1
+	# last = 875-1+1
 	skip = None
-	skip = "Bloomington"
+	skip = "Beloit"
 	source = None
 	# source = "Mesa"
-	tp.check_table_type_warning(csvfile, source, last, skip, None) 
-	tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
-	tp.test_check_version(csvfile, None, last, skip, None) #
+	# tp.check_table_type_warning(csvfile, source, last, skip, None) 
+	# tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
+	# tp.test_check_version(csvfile, None, last, skip, None) #
 	tp.test_source_download_limitable(csvfile, source, last, skip, None) 
 	
-	tp.test_get_count(csvfile, None, last, skip, None)
-	tp.test_load_gen(csvfile, source, last, skip, None) 
+	# tp.test_get_count(csvfile, None, last, skip, None)
+	# tp.test_load_gen(csvfile, source, last, skip, None) 
+
+	last = None
+	import test_opd_data2
+	tp = test_opd_data2.TestData()
+	tp.test_get_years(csvfile, source, last, skip, None)
+	tp.test_get_agencies(csvfile, None, None, skip, None)
+	tp.test_get_agencies_name_match(csvfile, None, None, skip, None)
+	tp.test_agency_filter(csvfile, None, None, skip, None)
+	tp.test_to_csv(csvfile, None, None, skip, None)
```

### Comparing `openpolicedata-0.5.4/tests/test_opd_data2.py` & `openpolicedata-0.5.5/tests/test_opd_data2.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 warn_errors = (OPD_DataUnavailableError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError)
 
 def get_datasets(csvfile):
     if csvfile != None:
         datasets.datasets = datasets._build(csvfile)
 
-    return datasets.query()
+    return datasets.datasets
 
 class TestData:
 	def test_get_years(self, csvfile, source, last, skip, loghtml):
 		if last == None:
 			last = float('inf')
 		datasets = get_datasets(csvfile)
 		caught_exceptions = []
```

### Comparing `openpolicedata-0.5.4/tests/test_opd_data3.py` & `openpolicedata-0.5.5/tests/test_opd_data3.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 warn_errors = (OPD_DataUnavailableError, OPD_SocrataHTTPError, OPD_FutureError, OPD_MinVersionError)
 
 def get_datasets(csvfile):
     if csvfile != None:
         datasets.datasets = datasets._build(csvfile)
 
-    return datasets.query()
+    return datasets.datasets
 
 class TestData:
 	@pytest.mark.slow(reason="This is a slow test that should be run before a major commit.")
 	def test_load_year(self, csvfile, source, last, skip, loghtml):
 		max_count = 1e5
 		if last == None:
 			last = float('inf')
```

