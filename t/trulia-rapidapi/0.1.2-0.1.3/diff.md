# Comparing `tmp/trulia_rapidapi-0.1.2.tar.gz` & `tmp/trulia_rapidapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trulia_rapidapi-0.1.2.tar", last modified: Mon Jun 19 20:01:09 2023, max compression
+gzip compressed data, was "trulia_rapidapi-0.1.3.tar", last modified: Wed Jun 21 08:43:19 2023, max compression
```

## Comparing `trulia_rapidapi-0.1.2.tar` & `trulia_rapidapi-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.254065 trulia_rapidapi-0.1.2/
--rw-rw-rw-   0        0        0     1848 2023-06-19 20:01:09.254065 trulia_rapidapi-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1232 2023-06-14 20:14:23.000000 trulia_rapidapi-0.1.2/README.md
--rw-rw-rw-   0        0        0      399 2023-06-19 20:01:09.257067 trulia_rapidapi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-06-19 20:00:46.000000 trulia_rapidapi-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.211466 trulia_rapidapi-0.1.2/trulia_rapidapi/
-drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.243458 trulia_rapidapi-0.1.2/trulia_rapidapi/src/
--rw-rw-rw-   0        0        0     6879 2023-06-19 19:59:49.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_api.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.253071 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/
--rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/base.py
--rw-rw-rw-   0        0        0     3207 2023-06-19 19:54:24.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/details_model.py
--rw-rw-rw-   0        0        0     3175 2023-06-14 19:13:10.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/enums.py
--rw-rw-rw-   0        0        0     1497 2023-06-14 18:52:49.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/listing_model.py
--rw-rw-rw-   0        0        0      539 2023-06-14 19:49:05.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/search_token_model.py
--rw-rw-rw-   0        0        0     2113 2023-06-19 19:58:43.000000 trulia_rapidapi-0.1.2/trulia_rapidapi/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:01:09.241459 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-06-19 20:01:09.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-06-19 20:01:09.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 20:01:09.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 20:08:36.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-19 20:01:09.000000 trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.410568 trulia_rapidapi-0.1.3/
+-rw-rw-rw-   0        0        0     1848 2023-06-21 08:43:19.411570 trulia_rapidapi-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1232 2023-06-14 20:14:23.000000 trulia_rapidapi-0.1.3/README.md
+-rw-rw-rw-   0        0        0      399 2023-06-21 08:43:19.413568 trulia_rapidapi-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-06-21 08:42:58.000000 trulia_rapidapi-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.373566 trulia_rapidapi-0.1.3/trulia_rapidapi/
+drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.397569 trulia_rapidapi-0.1.3/trulia_rapidapi/src/
+-rw-rw-rw-   0        0        0    11423 2023-06-21 08:30:23.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_api.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.409566 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/
+-rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/base.py
+-rw-rw-rw-   0        0        0     3207 2023-06-19 19:54:24.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/details_model.py
+-rw-rw-rw-   0        0        0     3175 2023-06-14 19:13:10.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/enums.py
+-rw-rw-rw-   0        0        0     1497 2023-06-14 18:52:49.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/listing_model.py
+-rw-rw-rw-   0        0        0      624 2023-06-21 08:13:36.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/search_token_model.py
+-rw-rw-rw-   0        0        0     2511 2023-06-21 08:34:04.000000 trulia_rapidapi-0.1.3/trulia_rapidapi/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:43:19.393568 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-21 08:43:19.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-06-21 08:43:19.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 08:43:19.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 20:08:36.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-06-21 08:43:19.000000 trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/top_level.txt
```

### Comparing `trulia_rapidapi-0.1.2/PKG-INFO` & `trulia_rapidapi-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulia_rapidapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Trulia Real Estate API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/trulia-real-estate-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Project-URL: Documentation, https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper/
 Project-URL: Bug Reports, https://github.com/letsscrape/python_trulia_rapidapi/issues
 Project-URL: Source Code, https://github.com/letsscrape/python_trulia_rapidapi
```

### Comparing `trulia_rapidapi-0.1.2/README.md` & `trulia_rapidapi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.2/setup.py` & `trulia_rapidapi-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='trulia_rapidapi',
-    version='0.1.2',
+    version='0.1.3',
     description='Trulia Real Estate API on RapidAPI',
     packages=['trulia_rapidapi', 'trulia_rapidapi.src', 'trulia_rapidapi.src.trulia_models'],
     author_email='hello@letsscrape.com',
     zip_safe=False,
     author='LetsScrape',
     keywords=['trulia', 'real estate api', 'trulia real estate', 'trulia api', 'parsing', 'scraper'],
     classifiers=[],
```

### Comparing `trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/details_model.py` & `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/details_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/enums.py` & `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/enums.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/listing_model.py` & `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/listing_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.2/trulia_rapidapi/src/trulia_models/search_token_model.py` & `trulia_rapidapi-0.1.3/trulia_rapidapi/src/trulia_models/search_token_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,11 +12,15 @@
 class Data(BaseModelORM):
     places: List[Place]
 
 class SearchTokenModel(BaseModelORM):
     description: str
     status: int
     data: Optional[Data] = None
+
+    def get_first_token(self):
+        return self.data.places[0].search_token
+
     def __str__(self):
         if len(self.data.places) == 0:
             return None
         return self.data.places[0].search_token
```

### Comparing `trulia_rapidapi-0.1.2/trulia_rapidapi/tests.py` & `trulia_rapidapi-0.1.3/trulia_rapidapi/tests.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,43 +14,55 @@
 api = TruliaAPI('____YOUR_RAPIDAPI_KEY____')
 
 async def test_get_listing_by_url():
     r = await api.get_listing_by_url("https://www.trulia.com/AZ/Scottsdale/", 1)
     assert r.status == 200
     assert len(r.data.homes) > 0
 
+async def test_search_by_token():
+    token = await api.get_search_token(TruliaSearchType.ForSale, "Scottsdale")
+    r = await api.search_for_sale_by_token(token.get_first_token(), 1)
+    assert r.status == 200
+    assert len(r.data.homes) > 0
+
+async def test_details_by_url():
+    r = await api.details_by_url('https://www.trulia.com/p/az/paradise-valley/9316-n-58th-st-paradise-valley-az-85253--2113546226')
+    assert r.status == 200
+    assert len(r.data.tags) > 0
+
 async def test_get_search_token():
     r = await api.get_search_token(TruliaSearchType.ForSale, "Scottsdale")
     assert r.status == 200
     
-async def test_search_by_place():
-    r = await api.search_by_place(TruliaSearchType.ForSale, "Scottsdale", 1)
+async def test_search_for_sale_by_place():
+    r = await api.search_for_sale_by_place("Scottsdale", 1)
     assert r.status == 200
     assert len(r.data.homes) > 0
 
-async def test_search_by_token():
-    token = await api.get_search_token(TruliaSearchType.ForSale, "Scottsdale")
-    r = await api.search_by_token(TruliaSearchType.ForSale, token.data.places[0].search_token, 1)
+async def test_search_for_sold_by_place():
+    r = await api.search_for_sold_by_place("Scottsdale", 1)
     assert r.status == 200
     assert len(r.data.homes) > 0
 
-async def test_details_by_url():
-    r = await api.details_by_url('https://www.trulia.com/p/az/paradise-valley/9316-n-58th-st-paradise-valley-az-85253--2113546226')
-    print(r)
+async def test_search_for_rent_by_place():
+    r = await api.search_for_rent_by_place("Scottsdale", 1)
     assert r.status == 200
-    assert len(r.data.tags) > 0
-
+    assert len(r.data.homes) > 0
 
 async def main():
-  await test_get_listing_by_url()
-  await test_get_search_token()
-  await test_search_by_place()
-  await test_search_by_token()
-  await test_details_by_url()
-  return None
+    await test_get_listing_by_url()
+    await test_get_search_token()
+    await test_search_by_token()
+    await test_details_by_url()
+
+    await test_search_for_sale_by_place()
+    await test_search_for_sold_by_place()
+    await test_search_for_rent_by_place()
+
+    return None
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
```

### Comparing `trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/PKG-INFO` & `trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulia-rapidapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Trulia Real Estate API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/trulia-real-estate-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Project-URL: Documentation, https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper/
 Project-URL: Bug Reports, https://github.com/letsscrape/python_trulia_rapidapi/issues
 Project-URL: Source Code, https://github.com/letsscrape/python_trulia_rapidapi
```

### Comparing `trulia_rapidapi-0.1.2/trulia_rapidapi.egg-info/SOURCES.txt` & `trulia_rapidapi-0.1.3/trulia_rapidapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

