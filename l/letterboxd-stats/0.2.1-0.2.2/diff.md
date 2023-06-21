# Comparing `tmp/letterboxd_stats-0.2.1.tar.gz` & `tmp/letterboxd_stats-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.2.1.tar", last modified: Tue Jun 13 14:02:50 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.2.2.tar", last modified: Mon Jun 19 14:33:36 2023, max compression
```

## Comparing `letterboxd_stats-0.2.1.tar` & `letterboxd_stats-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-13 14:02:50.267445 letterboxd_stats-0.2.1/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.1/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-13 14:02:50.267445 letterboxd_stats-0.2.1/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.1/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-13 14:02:50.267445 letterboxd_stats-0.2.1/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1745 2023-06-11 15:06:39.000000 letterboxd_stats-0.2.1/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5222 2023-06-13 14:00:37.000000 letterboxd_stats-0.2.1/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-13 13:59:51.000000 letterboxd_stats-0.2.1/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:00:30.000000 letterboxd_stats-0.2.1/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-05-08 18:03:39.000000 letterboxd_stats-0.2.1/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     6360 2023-06-11 15:20:14.000000 letterboxd_stats-0.2.1/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-13 14:02:50.267445 letterboxd_stats-0.2.1/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-13 14:02:50.000000 letterboxd_stats-0.2.1/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-06-13 14:02:50.000000 letterboxd_stats-0.2.1/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-06-13 14:02:50.000000 letterboxd_stats-0.2.1/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-06-13 14:02:50.000000 letterboxd_stats-0.2.1/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-06-13 14:02:50.000000 letterboxd_stats-0.2.1/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-06-13 14:02:50.000000 letterboxd_stats-0.2.1/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-06-13 14:02:25.000000 letterboxd_stats-0.2.1/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-06-13 14:02:50.267445 letterboxd_stats-0.2.1/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.2/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.2/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1745 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.2/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5222 2023-06-13 14:00:37.000000 letterboxd_stats-0.2.2/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.2/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.2/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-05-08 18:03:39.000000 letterboxd_stats-0.2.2/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     6353 2023-06-19 14:31:28.000000 letterboxd_stats-0.2.2/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-06-19 14:33:36.000000 letterboxd_stats-0.2.2/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-06-19 14:33:09.000000 letterboxd_stats-0.2.2/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-06-19 14:33:36.464228 letterboxd_stats-0.2.2/setup.cfg
```

### Comparing `letterboxd_stats-0.2.1/LICENCE` & `letterboxd_stats-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.1/PKG-INFO` & `letterboxd_stats-0.2.2/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: letterboxd_stats
-Version: 0.2.1
+Name: letterboxd-stats
+Version: 0.2.2
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.1/README.md` & `letterboxd_stats-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.1/letterboxd_stats/__init__.py` & `letterboxd_stats-0.2.2/letterboxd_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.1/letterboxd_stats/cli.py` & `letterboxd_stats-0.2.2/letterboxd_stats/cli.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.1/letterboxd_stats/data.py` & `letterboxd_stats-0.2.2/letterboxd_stats/data.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.1/letterboxd_stats/main.py` & `letterboxd_stats-0.2.2/letterboxd_stats/main.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.1/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.2.2/letterboxd_stats/tmdb.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.1/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.2.2/letterboxd_stats/web_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     "search": lambda s: f"/search/films/{s}/?adult",
     "diary": lambda s: f"/csi/film/{s}/sidebar-user-actions/?esiAllowUser=true",
     "add_watchlist": lambda s: f"/film/{s}/add-to-watchlist/",
     "remove_watchlist": lambda s: f"/film/{s}/remove-from-watchlist/",
     "film_page": lambda s: f"/film/{s}",
 }
 
+cache_path = os.path.expanduser(os.path.join(config["root_folder"], "static", "cache.csv"))
+tmdb_id_df = pd.read_csv(cache_path, header=0, index_col=0)
+
 
 class Downloader:
     def __init__(self):
         self.session = requests.Session()
         self.session.get(URL)
 
     def login(self):
@@ -89,16 +92,14 @@
 
 
 def create_movie_url(title: str, operation: str):
     return URL + OPERATIONS_URLS[operation](title)
 
 
 def get_tmdb_id(link: str, is_diary: bool):
-    cache_path = os.path.expanduser(os.path.join(config["root_folder"], "static", "cache.csv"))
-    tmdb_id_df = pd.read_csv(cache_path, header=0, index_col=0)
     if link in tmdb_id_df.index:
         return int(tmdb_id_df.loc[link]["Id"])
     res = requests.get(link)
     movie_page = html.fromstring(res.text)
     if is_diary:
         title_link = movie_page.xpath("//span[@class='film-title-wrapper']/a")
         if len(title_link) == 0:
```

### Comparing `letterboxd_stats-0.2.1/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: letterboxd-stats
-Version: 0.2.1
+Name: letterboxd_stats
+Version: 0.2.2
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.1/pyproject.toml` & `letterboxd_stats-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.2.1"
+version = "0.2.2"
 authors = [{ name = "mBaratta96" }]
 description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
```

