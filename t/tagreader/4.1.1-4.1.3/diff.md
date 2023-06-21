# Comparing `tmp/tagreader-4.1.1.tar.gz` & `tmp/tagreader-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-4.1.1.tar", max compression
+gzip compressed data, was "tagreader-4.1.3.tar", max compression
```

## Comparing `tagreader-4.1.1.tar` & `tagreader-4.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.1.1/LICENSE
--rw-r--r--   0        0        0     2779 2023-06-14 10:40:53.495633 tagreader-4.1.1/README.md
--rw-r--r--   0        0        0     1633 2023-06-14 13:27:23.957086 tagreader-4.1.1/pyproject.toml
--rw-r--r--   0        0        0      351 2023-06-14 10:40:53.499388 tagreader-4.1.1/tagreader/__init__.py
--rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.1.1/tagreader/__version__.py
--rw-r--r--   0        0        0    12723 2023-06-14 10:40:53.499996 tagreader-4.1.1/tagreader/cache.py
--rw-r--r--   0        0        0    22839 2023-06-14 13:05:07.540054 tagreader-4.1.1/tagreader/clients.py
--rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.1.1/tagreader/logger.py
--rw-r--r--   0        0        0    25164 2023-06-14 13:05:07.540885 tagreader-4.1.1/tagreader/odbc_handlers.py
--rw-r--r--   0        0        0     8215 2023-06-14 13:05:07.541522 tagreader-4.1.1/tagreader/utils.py
--rw-r--r--   0        0        0    32868 2023-06-14 10:54:03.255470 tagreader-4.1.1/tagreader/web_handlers.py
--rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 tagreader-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.1.3/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-15 12:41:41.851734 tagreader-4.1.3/README.md
+-rw-r--r--   0        0        0     1633 2023-06-21 14:18:50.115817 tagreader-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0      351 2023-06-14 10:40:53.499388 tagreader-4.1.3/tagreader/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.1.3/tagreader/__version__.py
+-rw-r--r--   0        0        0    12723 2023-06-14 10:40:53.499996 tagreader-4.1.3/tagreader/cache.py
+-rw-r--r--   0        0        0    23397 2023-06-21 14:18:50.116275 tagreader-4.1.3/tagreader/clients.py
+-rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.1.3/tagreader/logger.py
+-rw-r--r--   0        0        0    25164 2023-06-21 08:33:16.577206 tagreader-4.1.3/tagreader/odbc_handlers.py
+-rw-r--r--   0        0        0     8215 2023-06-14 13:05:07.541522 tagreader-4.1.3/tagreader/utils.py
+-rw-r--r--   0        0        0    32717 2023-06-21 14:05:09.371900 tagreader-4.1.3/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 tagreader-4.1.3/PKG-INFO
```

### Comparing `tagreader-4.1.1/LICENSE` & `tagreader-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tagreader-4.1.1/README.md` & `tagreader-4.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # tagreader-python <!-- omit in toc -->
 
 ![GitHub Build Status](https://github.com/equinor/tagreader-python/workflows/Test/badge.svg)
-[![Devops Build Status](https://dev.azure.com/EIIDS/tagreader/_apis/build/status/equinor.tagreader-python?branchName=master)](https://dev.azure.com/EIIDS/tagreader/_build/latest?definitionId=5&branchName=master)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader) 
-![PyPI](https://img.shields.io/pypi/v/tagreader) 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader)
+![PyPI](https://img.shields.io/pypi/v/tagreader)
 [![Downloads](https://pepy.tech/badge/tagreader)](https://pepy.tech/project/tagreader)
 
 Tagreader is a Python package for reading trend data from the OSIsoft
-PI and Aspen Infoplus.21 IMS systems. It is intended to be easy to use, 
+PI and Aspen Infoplus.21 IMS systems. It is intended to be easy to use,
 and present as similar interfaces as possible to the backend historians.
 
 While originally developed for Windows, Tagreader can since release 3.0.0
 also be used on Linux and Windows platforms.
 
 Queries can be performed using either REST API (preferred) or ODBC queries.
 The use of ODBC queries require installation of proprietary drivers from
@@ -36,20 +35,20 @@
 Microsoft Windows. Pyodbc will therefore not be installed for non-Windows
 systems.
 
 ## Installation
 
 To install and/or upgrade:
 
-``` 
+```
 pip install --upgrade tagreader
 ```
 
-If you wish to use ODBC connections to the IMS servers, you will also need 
-to install some proprietary drivers. There is more information in the 
+If you wish to use ODBC connections to the IMS servers, you will also need
+to install some proprietary drivers. There is more information in the
 [manual](docs/manual.md#odbc-drivers). Please note that the web APIs should
 normally be preferred.
 
 ## Usage example
 
 ```
 import tagreader
```

### Comparing `tagreader-4.1.1/pyproject.toml` & `tagreader-4.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tagreader"
-version = "4.1.1"
+version = "4.1.3"
 description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
 authors = ["Einar S. Idsø <eiids@equinor.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tagreader"}]
 keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
 homepage = "https://github.com/equinor/tagreader-python"
```

### Comparing `tagreader-4.1.1/tagreader/cache.py` & `tagreader-4.1.3/tagreader/cache.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.1.1/tagreader/clients.py` & `tagreader-4.1.3/tagreader/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import concurrent
 import os
-import warnings
+from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from itertools import groupby
 from operator import itemgetter
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
@@ -328,15 +329,15 @@
 
     def connect(self) -> None:
         self.handler.connect()
 
     def search_tag(
         self, tag: Optional[str] = None, desc: Optional[str] = None
     ) -> List[Tuple[str, str]]:
-        warnings.warn("This function is deprecated. Please call 'search()' instead")
+        logger.warning("This function is deprecated. Please call 'search()' instead")
         return self.search(tag=tag, desc=desc)
 
     def search(
         self, tag: Optional[str] = None, desc: Optional[str] = None
     ) -> List[Tuple[str, str]]:
         return self.handler.search(tag=tag, desc=desc)
 
@@ -598,28 +599,39 @@
         oldtags = tags
         tags = list(dict.fromkeys(tags))
         if len(oldtags) > len(tags):
             duplicates = set([x for n, x in enumerate(oldtags) if x in oldtags[:n]])
             logger.warning(
                 f"Duplicate tags found, removed duplicates: {', '.join(duplicates)}"
             )
-        cols = []
-        for tag in tags:
-            cols.append(
-                self._read_single_tag(
-                    tag=tag,
-                    start_time=start_time,
-                    stop_time=end_time,
-                    ts=ts,
-                    read_type=read_type,
-                    get_status=get_status,
-                    cache=self.cache,
+
+        # Fixme: Temporary reading from IMS using Threads to improve performance. Need to use batch queries or at least
+        #     keep the same connection between queries.
+        results = []
+        with ThreadPoolExecutor(
+            max_workers=min(10, (os.cpu_count() or 1) + 4)
+        ) as executor:
+            for i, tag in enumerate(tags):
+                results.append(
+                    executor.submit(
+                        self._read_single_tag,
+                        tag=tag,
+                        start_time=start_time,
+                        stop_time=end_time,
+                        ts=ts,
+                        read_type=read_type,
+                        get_status=get_status,
+                        cache=self.cache,
+                    )
                 )
-            )
-        return pd.concat(cols, axis=1)
+
+        return pd.concat(
+            [result.result() for result in concurrent.futures.as_completed(results)],
+            axis=1,
+        )
 
     def query_sql(self, query: str, parse: bool = True):
         """[summary]
         Args:
             query (str): [description]
             parse (bool, optional): Whether to attempt to parse query return
                                     value as table. Defaults to True.
```

### Comparing `tagreader-4.1.1/tagreader/odbc_handlers.py` & `tagreader-4.1.3/tagreader/odbc_handlers.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.1.1/tagreader/utils.py` & `tagreader-4.1.3/tagreader/utils.py`

 * *Files identical despite different names*

### Comparing `tagreader-4.1.1/tagreader/web_handlers.py` & `tagreader-4.1.3/tagreader/web_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,27 @@
+import json
 import re
 import urllib.parse
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
+from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pytz
 import requests
 import urllib3
-from requests import Response
 from requests_kerberos import OPTIONAL, HTTPKerberosAuth
 
 from tagreader.cache import BaseCache
 from tagreader.logger import logger
 from tagreader.utils import ReaderType, is_mac, is_windows, urljoin
 
-# Requests will use simplejson if it has been installed, so handle both errors here
-try:
-    from simplejson.errors import JSONDecodeError
-except ImportError:
-    from json.decoder import JSONDecodeError
-
 
 def get_verifySSL() -> Union[bool, str]:
     if is_windows() or is_mac():
         return True
     return "/etc/ssl/certs/ca-bundle.trust.crt"
 
 
@@ -124,22 +119,39 @@
         self.base_url = url
         self.session = requests.Session()
         self.session.auth = auth if auth is not None else get_auth_aspen()
         if verifySSL is False:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
 
-    def fetch(
-        self, url, params: Optional[Union[str, Dict[str, str]]] = None
-    ) -> Response:
-        if not self.session.verify:
-            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+    def fetch(self, url, params: Optional[Union[str, Dict[str, str]]] = None) -> Dict:
+        res = self.session.get(url, params=params)
+        res.raise_for_status()
+
+        if len(res.text) == 0:
+            logger.warning(f"No data found for {url} {params}")
+            return {}
+
+        try:
+            return res.json()
+        except JSONDecodeError:
+            # AspenOne sometimes returns completely and utterly invalid -nan.
+            # Since json/simplejson has no mechanism to handle this, we need to
+            # pre-process
+
+            txt = res.text.replace('"v":nan', '"v":NaN').replace('"v":-nan', '"v":NaN')
+            return json.loads(txt)
 
+    def fetch_text(
+        self, url, params: Optional[Union[str, Dict[str, str]]] = None
+    ) -> str:
         res = self.session.get(url, params=params)
-        return res
+        res.raise_for_status()
+
+        return res.text
 
     def connect(self):
         try:
             self.verify_connection(self.datasource)
         except requests.ConnectionError:
             raise ConnectionError(
                 f"Not able to connect to {self.base_url}. Check network connection."
@@ -293,17 +305,16 @@
         :type datasource: String
         :raises ConnectionError: If connection fails
         :return: True if datasource exists, False if not.
         :rtype: Bool
         """
         url = urljoin(self.base_url, "Datasources")
         params = {"service": "ProcessData", "allQuotes": 1}
-        r = self.fetch(url=url, params=params)
-        j = r.json()
-        for item in j["data"]:
+        data = self.fetch(url=url, params=params)
+        for item in data["data"]:
             if item["n"] == datasource:
                 return True
         return False
 
     @staticmethod
     def split_tagmap(tagmap) -> Tuple[Optional[str], ...]:
         return tuple(tagmap.split(";") if ";" in tagmap else (tagmap, None))
@@ -340,22 +351,21 @@
             "</Q>",
         ]
         return "".join(parts)
 
     def _get_maps(self, tagname: str):
         params = self.generate_get_map_query(tagname)
         url = urljoin(self.base_url, "TagInfo")
-        res = self.fetch(url, params=params)
-        j = res.json()
+        data = self.fetch(url, params=params)
 
-        if "tags" not in j["data"]:
+        if "tags" not in data["data"]:
             return {}
 
         ret = {}
-        for item in j["data"]["tags"][0]["categories"][0]["ta"]:
+        for item in data["data"]["tags"][0]["categories"][0]["ta"]:
             ret[item["m"]] = True if item["d"] == "True" else False
         return ret
 
     def _get_default_mapname(self, tagname: str):
         (tagname, _) = self.split_tagmap(tagname)
         allmaps = self._get_maps(tagname)
         for k, v in allmaps.items():
@@ -378,23 +388,21 @@
         # unencoded. Otherwise searches for tags containing spaces break, as do wildcard
         # searches.
         encoded_params = urllib.parse.urlencode(
             params, safe="*", quote_via=urllib.parse.quote
         )
         url = urljoin(self.base_url, "Browse?")
         url += encoded_params
-        res = self.fetch(url)
-
-        j = res.json()
+        data = self.fetch(url)
 
-        if "tags" not in j["data"]:
+        if "tags" not in data["data"]:
             return []
 
         ret = []
-        for item in j["data"]["tags"]:
+        for item in data["data"]["tags"]:
             tagname = item["t"]
             description = self._get_tag_description(tagname)
             ret.append((tagname, description))
 
         if not desc:
             return ret
 
@@ -404,20 +412,19 @@
 
     def _get_tag_metadata(self, tag: str):
         return {}  # FIXME
 
     def _get_tag_unit(self, tag: str):
         query = self.generate_get_unit_query(tag)
         url = urljoin(self.base_url, "TagInfo")
-        res = self.fetch(url, params=query)
-        j = res.json()
+        data = self.fetch(url, params=query)
         try:
-            attrdata = j["data"]["tags"][0]["attrData"]
+            attrdata = data["data"]["tags"][0]["attrData"]
         except Exception:
-            print(f"Error. I got this: {j}")
+            print(f"Error. I got this: {data}")
             raise KeyError
         unit = ""
         for a in attrdata:
             if a["g"] == "Units":
                 unit = a["samples"][0]["v"]
                 break
         return unit
@@ -439,18 +446,17 @@
             "</Q>",
         ]
         return "".join(parts)
 
     def _get_tag_description(self, tag: str):
         query = self.generate_get_description_query(tag)
         url = urljoin(self.base_url, "TagInfo")
-        res = self.fetch(url, params=query)
-        j = res.json()
+        data = self.fetch(url, params=query)
         try:
-            desc = j["data"]["tags"][0]["attrData"][0]["samples"][0]["v"]
+            desc = data["data"]["tags"][0]["attrData"][0]["samples"][0]["v"]
         except Exception:
             desc = ""
         return desc
 
     def read_tag(
         self,
         tag: str,
@@ -497,43 +503,32 @@
             start_time=start_time,
             stop_time=stop_time,
             sample_time=sample_time,
             read_type=read_type,
             metadata={},
         )
 
-        res = self.fetch(url, params=params)
+        data = self.fetch(url, params=params)
 
-        if len(res.text) == 0:  # res.text='' for timestamps in future
+        if len(data) == 0:  # Normally for timestamps in future
             return pd.DataFrame(columns=[tag])
 
-        try:
-            j = res.json()
-        except JSONDecodeError:
-            # AspenOne sometimes returns completely and utterly invalid -nan.
-            # Since json/simplejson has no mechanism to handle this, we need to
-            # pre-process
-            import json
-
-            txt = res.text.replace('"v":nan', '"v":NaN').replace('"v":-nan', '"v":NaN')
-            j = json.loads(txt)
-
-        if "er" in j["data"][0]["samples"][0]:
-            logger.warning(j["data"][0]["samples"][0]["es"])
+        if "er" in data["data"][0]["samples"][0]:
+            logger.warning(data["data"][0]["samples"][0]["es"])
             return pd.DataFrame(columns=[tag])
         if get_status:
             # The "l" field maps 1:1 to ODBC status field values 0, 1, 2, 4, 5, 6
             df = (
-                pd.DataFrame.from_dict(j["data"][0]["samples"])
+                pd.DataFrame.from_dict(data["data"][0]["samples"])
                 .drop(labels=["s", "V"], axis="columns")
                 .rename(columns={"t": "Timestamp", "v": "Value", "l": "Status"})
             )
         else:
             df = (
-                pd.DataFrame.from_dict(j["data"][0]["samples"])
+                pd.DataFrame.from_dict(data["data"][0]["samples"])
                 .drop(labels=["l", "s", "V"], axis="columns")
                 .rename(columns={"t": "Timestamp", "v": "Value"})
             )
 
         # Ensure non-numericals like "1.#QNAN" are returned as NaN
         df["Value"] = pd.to_numeric(df.Value, errors="coerce")
 
@@ -588,21 +583,21 @@
         else:
             params = self.generate_sql_query(
                 connection_string=self._connection_string,
                 query=query,
                 max_rows=self._max_rows,
                 datasource=None,
             )
-        res = self.fetch(url, params=params)
+        res_text = self.fetch_text(url, params=params)
         # For now just return result as text regardless of value of parse
         if parse:
             raise NotImplementedError(
                 "Use parse=False to receive and handle text result instead"
             )
-        return res.text
+        return res_text
 
 
 class PIHandlerWeb(BaseHandlerWeb):
     def __init__(
         self,
         url: Optional[str],
         datasource: Optional[str],
@@ -768,65 +763,61 @@
         :param datasource: Data source to look for
         :type datasource: String
         :raises ConnectionError: If connection fails
         :return: True if data source exists, False if not.
         :rtype: Bool
         """
         url = urljoin(self.base_url, "dataservers")
-        res = self.fetch(url)
-        j = res.json()
-        for item in j["Items"]:
+        data = self.fetch(url)
+        for item in data["Items"]:
             if item["Name"] == datasource:
                 return True
         return False
 
     def search(
         self, tag: Optional[str] = None, desc: Optional[str] = None
     ) -> List[Tuple]:
         params = self.generate_search_query(
             tag=tag, desc=desc, datasource=self.datasource
         )
         url = urljoin(self.base_url, "search", "query")
         done = False
         ret = []
         while not done:
-            res = self.fetch(url, params=params)
+            data = self.fetch(url, params=params)
 
-            j = res.json()
-            for item in j["Items"]:
+            for item in data["Items"]:
                 description = item["Description"] if "Description" in item else ""
                 ret.append((item["Name"], description))
-            next_start = int(j["Links"]["Next"].split("=")[-1])
-            if int(j["Links"]["Last"].split("=")[-1]) >= next_start:
+            next_start = int(data["Links"]["Next"].split("=")[-1])
+            if int(data["Links"]["Last"].split("=")[-1]) >= next_start:
                 params["start"] = next_start
             else:
                 done = True
         return ret
 
     def _get_tag_metadata(self, tag: str) -> Dict[str, str]:
         return {}  # FIXME
 
     def _get_tag_unit(self, tag: str) -> Optional[str]:
         webid = self.tag_to_webid(tag)
         if webid is None:
             return None
         url = urljoin(self.base_url, "points", webid)
-        res = self.fetch(url)
-        j = res.json()
-        unit = j["EngineeringUnits"]
+        data = self.fetch(url)
+        unit = data["EngineeringUnits"]
         return unit
 
     def _get_tag_description(self, tag: str) -> Optional[str]:
         webid = self.tag_to_webid(tag)
         if webid is None:
             return None
         url = urljoin(self.base_url, "points", webid)
-        res = self.fetch(url)
-        j = res.json()
-        description = j["Descriptor"]
+        data = self.fetch(url)
+        description = data["Descriptor"]
         return description
 
     def tag_to_webid(self, tag: str) -> Optional[str]:
         """Given a tag, returns the WebId.
 
         :param tag: The tag
         :type tag: str
@@ -836,34 +827,33 @@
         """
         if tag not in self.webidcache:
             params = self.generate_search_query(
                 tag=tag, datasource=self.datasource, desc=None
             )
             params["fields"] = "name;webid"
             url = urljoin(self.base_url, "search", "query")
-            res = self.fetch(url, params=params)
-            j = res.json()
+            data = self.fetch(url, params=params)
 
-            if len(j["Errors"]) > 0:
-                msg = f"Received error from server when searching for WebId for {tag}: {j['Errors']}"
+            if len(data["Errors"]) > 0:
+                msg = f"Received error from server when searching for WebId for {tag}: {data['Errors']}"
                 raise ValueError(msg)
 
-            if len(j["Items"]) > 1:
+            if len(data["Items"]) > 1:
                 # Compare elements and if same, return the first
-                first = j["Items"][0]
-                for item in j["Items"][1:]:
+                first = data["Items"][0]
+                for item in data["Items"][1:]:
                     if item != first:
                         raise AssertionError(
-                            f"Received {len(j['Items'])} results when trying to find unique WebId for {tag}."
+                            f"Received {len(data['Items'])} results when trying to find unique WebId for {tag}."
                         )
-            elif len(j["Items"]) == 0:
+            elif len(data["Items"]) == 0:
                 logger.warning(f"Tag {tag} not found")
                 return None
 
-            webid = j["Items"][0]["WebId"]
+            webid = data["Items"][0]["WebId"]
             self.webidcache[tag] = webid
         return self.webidcache[tag]
 
     @staticmethod
     def _is_summary(read_type: ReaderType) -> bool:
         if read_type in [
             ReaderType.AVG,
@@ -896,22 +886,21 @@
             stop_time=stop_time,
             sample_time=sample_time,
             read_type=read_type,
             metadata={},
             get_status=get_status,
         )
         url = urljoin(self.base_url, url)
-        res = self.fetch(url, params=params)
+        data = self.fetch(url, params=params)
 
-        j = res.json()
         if read_type == ReaderType.SNAPSHOT:
-            df = pd.DataFrame.from_dict([j])  # noqa
+            df = pd.DataFrame.from_dict([data])  # noqa
         else:
             # Summary (aggregated) data and DigitalSets return Value as dict
-            df = pd.json_normalize(data=j, record_path="Items")
+            df = pd.json_normalize(data=data, record_path="Items")
 
         # Can happen for RAW reads w/o data in interval
         if df.empty:
             return df
 
         # Summary data, digitalset or invalid data
         if "Value" not in df.columns:
```

### Comparing `tagreader-4.1.1/PKG-INFO` & `tagreader-4.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagreader
-Version: 4.1.1
+Version: 4.1.3
 Summary: Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems.
 Home-page: https://github.com/equinor/tagreader-python
 License: MIT
 Keywords: Aspen InfoPlus.21,OSIsoft PI
 Author: Einar S. Idsø
 Author-email: eiids@equinor.com
 Requires-Python: >=3.8,<4.0
@@ -39,21 +39,20 @@
 Requires-Dist: requests-kerberos (>=0,<1)
 Project-URL: Repository, https://github.com/equinor/tagreader-python
 Description-Content-Type: text/markdown
 
 # tagreader-python <!-- omit in toc -->
 
 ![GitHub Build Status](https://github.com/equinor/tagreader-python/workflows/Test/badge.svg)
-[![Devops Build Status](https://dev.azure.com/EIIDS/tagreader/_apis/build/status/equinor.tagreader-python?branchName=master)](https://dev.azure.com/EIIDS/tagreader/_build/latest?definitionId=5&branchName=master)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader) 
-![PyPI](https://img.shields.io/pypi/v/tagreader) 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader)
+![PyPI](https://img.shields.io/pypi/v/tagreader)
 [![Downloads](https://pepy.tech/badge/tagreader)](https://pepy.tech/project/tagreader)
 
 Tagreader is a Python package for reading trend data from the OSIsoft
-PI and Aspen Infoplus.21 IMS systems. It is intended to be easy to use, 
+PI and Aspen Infoplus.21 IMS systems. It is intended to be easy to use,
 and present as similar interfaces as possible to the backend historians.
 
 While originally developed for Windows, Tagreader can since release 3.0.0
 also be used on Linux and Windows platforms.
 
 Queries can be performed using either REST API (preferred) or ODBC queries.
 The use of ODBC queries require installation of proprietary drivers from
@@ -78,20 +77,20 @@
 Microsoft Windows. Pyodbc will therefore not be installed for non-Windows
 systems.
 
 ## Installation
 
 To install and/or upgrade:
 
-``` 
+```
 pip install --upgrade tagreader
 ```
 
-If you wish to use ODBC connections to the IMS servers, you will also need 
-to install some proprietary drivers. There is more information in the 
+If you wish to use ODBC connections to the IMS servers, you will also need
+to install some proprietary drivers. There is more information in the
 [manual](docs/manual.md#odbc-drivers). Please note that the web APIs should
 normally be preferred.
 
 ## Usage example
 
 ```
 import tagreader
```

