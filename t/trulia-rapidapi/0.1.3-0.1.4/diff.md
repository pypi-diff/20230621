# Comparing `tmp/trulia_rapidapi-0.1.3.tar.gz` & `tmp/trulia_rapidapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trulia_rapidapi-0.1.3.tar", last modified: Wed Jun 21 08:43:19 2023, max compression
+gzip compressed data, was "trulia_rapidapi-0.1.4.tar", last modified: Wed Jun 21 12:57:01 2023, max compression
```

## Comparing `trulia_rapidapi-0.1.3.tar` & `trulia_rapidapi-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.410568 trulia_rapidapi-0.1.3/
--rw-rw-rw-   0        0        0     1848 2023-06-21 08:43:19.411570 trulia_rapidapi-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1232 2023-06-14 20:14:23.000000 trulia_rapidapi-0.1.3/README.md
--rw-rw-rw-   0        0        0      399 2023-06-21 08:43:19.413568 trulia_rapidapi-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-06-21 08:42:58.000000 trulia_rapidapi-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.373566 trulia_rapidapi-0.1.3/trulia_rapidapi/
-drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.397569 trulia_rapidapi-0.1.3/trulia_rapidapi/src/
--rw-rw-rw-   0        0        0    11423 2023-06-21 08:30:23.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_api.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.409566 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/
--rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/base.py
--rw-rw-rw-   0        0        0     3207 2023-06-19 19:54:24.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/details_model.py
--rw-rw-rw-   0        0        0     3175 2023-06-14 19:13:10.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/enums.py
--rw-rw-rw-   0        0        0     1497 2023-06-14 18:52:49.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/listing_model.py
--rw-rw-rw-   0        0        0      624 2023-06-21 08:13:36.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/search_token_model.py
--rw-rw-rw-   0        0        0     2511 2023-06-21 08:34:04.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.393568 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-06-21 08:43:19.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-06-21 08:43:19.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 08:43:19.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 20:08:36.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-21 08:43:19.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 12:57:01.658883 trulia_rapidapi-0.1.4/
+-rw-rw-rw-   0        0        0     1848 2023-06-21 12:57:01.658883 trulia_rapidapi-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1232 2023-06-14 20:14:23.000000 trulia_rapidapi-0.1.4/README.md
+-rw-rw-rw-   0        0        0      399 2023-06-21 12:57:01.665884 trulia_rapidapi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-06-21 12:56:42.000000 trulia_rapidapi-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:57:01.613877 trulia_rapidapi-0.1.4/trulia_rapidapi/
+drwxrwxrwx   0        0        0        0 2023-06-21 12:57:01.650893 trulia_rapidapi-0.1.4/trulia_rapidapi/src/
+-rw-rw-rw-   0        0        0    11363 2023-06-21 12:54:57.000000 trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_api.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:57:01.657878 trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/
+-rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/base.py
+-rw-rw-rw-   0        0        0     3207 2023-06-19 19:54:24.000000 trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/details_model.py
+-rw-rw-rw-   0        0        0     3175 2023-06-14 19:13:10.000000 trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/enums.py
+-rw-rw-rw-   0        0        0     1497 2023-06-14 18:52:49.000000 trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/listing_model.py
+-rw-rw-rw-   0        0        0      624 2023-06-21 08:13:36.000000 trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/search_token_model.py
+-rw-rw-rw-   0        0        0     2511 2023-06-21 08:34:04.000000 trulia_rapidapi-0.1.4/trulia_rapidapi/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:57:01.640893 trulia_rapidapi-0.1.4/trulia_rapidapi.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-21 12:57:01.000000 trulia_rapidapi-0.1.4/trulia_rapidapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-06-21 12:57:01.000000 trulia_rapidapi-0.1.4/trulia_rapidapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 12:57:01.000000 trulia_rapidapi-0.1.4/trulia_rapidapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 20:08:36.000000 trulia_rapidapi-0.1.4/trulia_rapidapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-06-21 12:57:01.000000 trulia_rapidapi-0.1.4/trulia_rapidapi.egg-info/top_level.txt
```

### Comparing `trulia_rapidapi-0.1.3/PKG-INFO` & `trulia_rapidapi-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulia_rapidapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Trulia Real Estate API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/trulia-real-estate-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Project-URL: Documentation, https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper/
 Project-URL: Bug Reports, https://github.com/letsscrape/python_trulia_rapidapi/issues
 Project-URL: Source Code, https://github.com/letsscrape/python_trulia_rapidapi
```

### Comparing `trulia_rapidapi-0.1.3/README.md` & `trulia_rapidapi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.3/setup.py` & `trulia_rapidapi-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='trulia_rapidapi',
-    version='0.1.3',
+    version='0.1.4',
     description='Trulia Real Estate API on RapidAPI',
     packages=['trulia_rapidapi', 'trulia_rapidapi.src', 'trulia_rapidapi.src.trulia_models'],
     author_email='hello@letsscrape.com',
     zip_safe=False,
     author='LetsScrape',
     keywords=['trulia', 'real estate api', 'trulia real estate', 'trulia api', 'parsing', 'scraper'],
     classifiers=[],
```

### Comparing `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_api.py` & `trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,15 @@
         """
         path = f"/search/for_sale?search_token={token}&page={page}&sort={sort}&beds={beds}&min_price={min_price}&max_price={max_price}&house_type={house_type}&for_sale_by_agent={for_sale_by_agent}&for_sale_by_owner={for_sale_by_owner}&new_construction={new_construction}"
         path = path.replace('=None', '=')
         response_data = await self.__get_request(path=path)
         response = ListingModel.parse_obj(response_data)
         return response
      
-    async def search_for_sold_by_place(self, place: str, page: int, 
-        sort: TruliaSort=None, beds: TruliaBeds=None, sold_date: TruliaSoldDate=None) -> ListingModel:
+    async def search_for_sold_by_place(self, place: str, page: int, beds: TruliaBeds=None, sold_date: TruliaSoldDate=None) -> ListingModel:
         """
         This function automatically generates a search token based on the variable {place}. 
         If {place} returns multiple search tokens, the first element will be passed to 
         the search query. Therefore, in this function, full control is not assured since we 
         might want to use, for example, the second token that matches a different place. 
         At the same time, this function will often be sufficient for the user.
 
@@ -159,18 +158,17 @@
         token = await self.get_search_token(TruliaSearchType.Sold, place)
 
         if len(token.data.places) == 0:
             return ListingModel(data=None, status=200, description="No places have been found!")
 
         search_token = token.get_first_token()
 
-        return await self.search_for_sold_by_token(search_token, page, sort, beds, sold_date)
+        return await self.search_for_sold_by_token(search_token, page, beds, sold_date)
 
-    async def search_for_sold_by_token(self, token: str, page: int, 
-        sort: TruliaSort=None, beds: TruliaBeds=None, sold_date: TruliaSoldDate=None) -> ListingModel:
+    async def search_for_sold_by_token(self, token: str, page: int, beds: TruliaBeds=None, sold_date: TruliaSoldDate=None) -> ListingModel:
         """
         This function accepts a token, in contrast to the search_for_sold_by_place, 
         where we have to manually pass the token. Hence, it's necessary 
         to first generate it with get_search_token, choose the appropriate token,
         and then pass it to the function.
 
         Parameters:
@@ -212,14 +210,14 @@
         where we have to manually pass the token. Hence, it's necessary 
         to first generate it with get_search_token, choose the appropriate token,
         and then pass it to the function.
 
         Parameters:
         page (int): The page number you want to work with. If you want the first page, pass in 1.
         """
-        path = f"/search/for_rent?search_token={token}&page={page}&beds={beds}&min_price={min_price}&max_price={max_price}&cats_allowed={cats_allowed}&dogs_allowed={dogs_allowed}&rental_type={rental_type}"
+        path = f"/search/for_rent?search_token={token}&page={page}&sort={sort}&beds={beds}&min_price={min_price}&max_price={max_price}&cats_allowed={cats_allowed}&dogs_allowed={dogs_allowed}&rental_type={rental_type}"
         path = path.replace('=None', '=')
         response_data = await self.__get_request(path=path)
         response = ListingModel.parse_obj(response_data)
         return response
```

### Comparing `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/details_model.py` & `trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/details_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/enums.py` & `trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/enums.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/listing_model.py` & `trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/listing_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/search_token_model.py` & `trulia_rapidapi-0.1.4/trulia_rapidapi/src/trulia_models/search_token_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.3/trulia_rapidapi/tests.py` & `trulia_rapidapi-0.1.4/trulia_rapidapi/tests.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/PKG-INFO` & `trulia_rapidapi-0.1.4/trulia_rapidapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulia-rapidapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Trulia Real Estate API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/trulia-real-estate-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Project-URL: Documentation, https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper/
 Project-URL: Bug Reports, https://github.com/letsscrape/python_trulia_rapidapi/issues
 Project-URL: Source Code, https://github.com/letsscrape/python_trulia_rapidapi
```

### Comparing `trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/SOURCES.txt` & `trulia_rapidapi-0.1.4/trulia_rapidapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

