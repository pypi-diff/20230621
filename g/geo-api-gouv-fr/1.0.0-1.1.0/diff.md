# Comparing `tmp/geo_api_gouv_fr-1.0.0.tar.gz` & `tmp/geo_api_gouv_fr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_api_gouv_fr-1.0.0.tar", max compression
+gzip compressed data, was "geo_api_gouv_fr-1.1.0.tar", max compression
```

## Comparing `geo_api_gouv_fr-1.0.0.tar` & `geo_api_gouv_fr-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      364 2023-04-26 09:43:22.519370 geo_api_gouv_fr-1.0.0/README.md
--rw-r--r--   0        0        0      279 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/__init__.py
--rw-r--r--   0        0        0       90 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/adress/__init__.py
--rw-r--r--   0        0        0     2768 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/adress/api.py
--rw-r--r--   0        0        0     4114 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/adress/schemas.py
--rw-r--r--   0        0        0       75 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/api.py
--rw-r--r--   0        0        0     1862 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/schemas.py
--rw-r--r--   0        0        0       78 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/department/__init__.py
--rw-r--r--   0        0        0     1268 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/department/api.py
--rw-r--r--   0        0        0      962 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/department/schemas.py
--rw-r--r--   0        0        0       74 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/__init__.py
--rw-r--r--   0        0        0      864 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/api.py
--rw-r--r--   0        0        0      552 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/schemas.py
--rw-r--r--   0        0        0        0 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/__init__.py
--rw-r--r--   0        0        0      195 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/data/reverse.csv
--rw-r--r--   0        0        0      294 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/data/search.csv
--rw-r--r--   0        0        0     4435 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_adresse.py
--rw-r--r--   0        0        0     1335 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_commune.py
--rw-r--r--   0        0        0      982 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_department.py
--rw-r--r--   0        0        0      751 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_region.py
--rw-r--r--   0        0        0     1636 2023-04-26 10:14:49.091133 geo_api_gouv_fr-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 geo_api_gouv_fr-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      364 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/README.md
+-rw-r--r--   0        0        0      279 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/adress/__init__.py
+-rw-r--r--   0        0        0     2768 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/adress/api.py
+-rw-r--r--   0        0        0     4142 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/adress/schemas.py
+-rw-r--r--   0        0        0       75 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/commune/__init__.py
+-rw-r--r--   0        0        0     1544 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/commune/api.py
+-rw-r--r--   0        0        0     1862 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/commune/schemas.py
+-rw-r--r--   0        0        0       78 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/department/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/department/api.py
+-rw-r--r--   0        0        0      962 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/department/schemas.py
+-rw-r--r--   0        0        0       74 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/region/__init__.py
+-rw-r--r--   0        0        0      864 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/region/api.py
+-rw-r--r--   0        0        0      552 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/region/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/data/lbb-search.csv
+-rw-r--r--   0        0        0      195 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/data/reverse.csv
+-rw-r--r--   0        0        0      294 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/data/search.csv
+-rw-r--r--   0        0        0     4872 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/test_adresse.py
+-rw-r--r--   0        0        0     1335 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/test_commune.py
+-rw-r--r--   0        0        0      982 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/test_department.py
+-rw-r--r--   0        0        0      751 2023-06-21 13:50:13.071093 geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/test_region.py
+-rw-r--r--   0        0        0     1636 2023-06-21 13:50:45.935703 geo_api_gouv_fr-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 geo_api_gouv_fr-1.1.0/PKG-INFO
```

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/adress/api.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/adress/api.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/adress/schemas.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/adress/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         lon:
 
     """
     q: Optional[str]
     limit: Optional[int]
     autocomplete: Optional[int]
     type: Optional[str]
-    postcode: Optional[int]
+    postcode: Optional[str]
+    citycode: Optional[str]
     lat: Optional[float]
     lon: Optional[float]
 
     @validator('q')
     def add_smaller_than_200(cls, v):
         """Validator for query to be smaller than 200 characters
         """
```

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/api.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/commune/api.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/schemas.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/commune/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,14 @@
         codeEpci:
         codeDepartement:
         codeRegion:
         population:
         _score:
     """
     nom: str
-    code: int
+    code: str
     codePostaux: Optional[List[str]]
     codeEpci: Optional[str]
     codeDepartement: Optional[str]
     codeRegion: Optional[str]
     population: Optional[str]
     _score: Optional[float]
```

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/department/api.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/department/api.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/department/schemas.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/department/schemas.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/api.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/region/api.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/schemas.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/region/schemas.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_adresse.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/test_adresse.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,7 +112,15 @@
 
     def test_adress_feature(self) -> None:
 
         geo = Geometry(type="any", coordinates=[1.6, 9.2])
         addr = AddressFeature(geometry=geo)
 
         self.assertTrue(addr.get_coords() == GpsCoordinate(latitude=1.6, longitude=9.2))
+
+    def test_issue_with_07500_postcode(self):
+        time.sleep(WAIT_TIME)
+        r = self.api.search_csv(csv="./geo_api_gouv_fr/tests/data/lbb-search.csv", columns=["streetnumber", "street", "postcode"], citycode="citycode", result_columns=["latitude", "longitude", "result_city"])
+        self.assertTrue(r.status_code == 200)
+
+        with open("./testResults/issue_with_07500_postcode.txt", "w") as f:
+            f.write(r.text)
```

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_commune.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/test_commune.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_department.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/test_department.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_region.py` & `geo_api_gouv_fr-1.1.0/geo_api_gouv_fr/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-1.0.0/pyproject.toml` & `geo_api_gouv_fr-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geo-api-gouv-fr"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python package to use geoapi.gouv.fr api"
 authors = ["La Bonne Boite <labonneboite@pole-emploi.fr>"]
 license  = "GPL-3.0-only"
 keywords = ["geoapi", "geoapi.gouv", "geoapi.gouv.fr"]
 readme = "README.md"
 packages = [
     { include = "geo_api_gouv_fr" }
```

### Comparing `geo_api_gouv_fr-1.0.0/PKG-INFO` & `geo_api_gouv_fr-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: geo-api-gouv-fr
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python package to use geoapi.gouv.fr api
 Home-page: https://github.com/StartupsPoleEmploi/geo-api-gouv-fr
 License: GPL-3.0-only
 Keywords: geoapi,geoapi.gouv,geoapi.gouv.fr
 Author: La Bonne Boite
 Author-email: labonneboite@pole-emploi.fr
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: pydantic[email] (>=1.10.4,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/StartupsPoleEmploi/geo-api-gouv-fr
 Description-Content-Type: text/markdown
 
 # GeoApi for data.gouv - Python Package
```

