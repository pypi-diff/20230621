# Comparing `tmp/TruMusic-1.1.6.tar.gz` & `tmp/TruMusic-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TruMusic-1.1.6.tar", last modified: Sat May 20 00:33:04 2023, max compression
+gzip compressed data, was "TruMusic-1.1.7.tar", last modified: Wed Jun 21 20:47:03 2023, max compression
```

## Comparing `TruMusic-1.1.6.tar` & `TruMusic-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:33:04.198783 TruMusic-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 00:33:04.198783 TruMusic-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-20 00:32:49.000000 TruMusic-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:33:04.198783 TruMusic-1.1.6/TruMusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-20 00:32:49.000000 TruMusic-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:33:04.198783 TruMusic-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-20 00:32:49.000000 TruMusic-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:33:04.198783 TruMusic-1.1.6/tru_music/
--rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-05-20 00:32:49.000000 TruMusic-1.1.6/tru_music/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:33:04.198783 TruMusic-1.1.6/tru_music/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:32:49.000000 TruMusic-1.1.6/tru_music/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-20 00:32:49.000000 TruMusic-1.1.6/tru_music/scripts/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-20 00:32:49.000000 TruMusic-1.1.6/tru_music/scripts/trumusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:47:03.050670 TruMusic-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-21 20:47:03.050670 TruMusic-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-21 20:46:52.000000 TruMusic-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:47:03.050670 TruMusic-1.1.7/TruMusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-21 20:47:03.000000 TruMusic-1.1.7/TruMusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-21 20:47:03.000000 TruMusic-1.1.7/TruMusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:47:03.000000 TruMusic-1.1.7/TruMusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-21 20:47:03.000000 TruMusic-1.1.7/TruMusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 20:47:03.000000 TruMusic-1.1.7/TruMusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 20:47:03.000000 TruMusic-1.1.7/TruMusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-21 20:46:52.000000 TruMusic-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:47:03.050670 TruMusic-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-21 20:46:52.000000 TruMusic-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:47:03.050670 TruMusic-1.1.7/tru_music/
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-21 20:46:52.000000 TruMusic-1.1.7/tru_music/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:47:03.050670 TruMusic-1.1.7/tru_music/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:52.000000 TruMusic-1.1.7/tru_music/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-21 20:46:52.000000 TruMusic-1.1.7/tru_music/scripts/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-21 20:46:52.000000 TruMusic-1.1.7/tru_music/scripts/trumusic.py
```

### Comparing `TruMusic-1.1.6/PKG-INFO` & `TruMusic-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.6
+Version: 1.1.7
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.6/TruMusic.egg-info/PKG-INFO` & `TruMusic-1.1.7/TruMusic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.6
+Version: 1.1.7
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.6/pyproject.toml` & `TruMusic-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = 'TruMusic'
-version = '1.1.6'
+version = '1.1.7'
 description='Audio file auto-tagger'
 
 authors = [
     {name = "Jacob Truman", email="jacob.truman@gmail.com"},
 ]
 
 dependencies = [
```

### Comparing `TruMusic-1.1.6/tru_music/__init__.py` & `TruMusic-1.1.7/tru_music/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,35 +113,38 @@
     # pylint: disable=too-many-branches,too-many-locals)
     def _get_album_info(self, album_artist: str, album_title: str):
         network = pylast.LastFMNetwork(
             api_key=os.environ.get('LASTFM_API_KEY', None),
             api_secret=os.environ.get('LASTFM_API_SECRET', None),
         )
 
-        album_search = network.search_for_album(album_title)
+        album_search = network.search_for_artist(album_artist)
         results = album_search.get_next_page()
         matching_results = []
         for res in results:
-            if str(res.artist).casefold() == album_artist.casefold():
-                try:
-                    album_tracks = res.get_tracks()
-                except pylast.WSError as pye:
-                    self.logger.debug(pye)
-                    continue
-                release_date = None
-                mbid = res.get_mbid()
-                if mbid is not None:
-                    release = musicbrainzngs.get_release_by_id(id=mbid)
-                    release_date = release['release']['date']
-                # this is hacky...
-                res.release_date = release_date
-                matching_results.append(res)
-                if not self.quiet:
-                    print(f"\t{len(matching_results)}. {album_artist} {res.title} ({len(album_tracks)} tracks) "
-                          f"({res.release_date})")
+            if res.name == album_artist:
+                for top_item in res.get_top_albums():
+                    item = top_item.item
+                    if str(item.title).casefold() == album_title.casefold():
+                        try:
+                            album_tracks = item.get_tracks()
+                        except pylast.WSError as pye:
+                            self.logger.debug(pye)
+                            continue
+                        release_date = None
+                        mbid = item.get_mbid()
+                        if mbid is not None:
+                            release = musicbrainzngs.get_release_by_id(id=mbid)
+                            release_date = release['release']['date']
+                        # this is hacky...
+                        item.release_date = release_date
+                        matching_results.append(item)
+                        if not self.quiet:
+                            print(f"\t{len(matching_results)}. {album_artist} {item.title} ({len(album_tracks)} tracks)"
+                                  f" ({item.release_date})")
 
         album = None
         match_count = len(matching_results)
         if match_count == 1 or (match_count > 0 and self.quiet):
             album = matching_results[0]
         elif match_count > 1:
             while album is None:
```

### Comparing `TruMusic-1.1.6/tru_music/scripts/cleanup.py` & `TruMusic-1.1.7/tru_music/scripts/cleanup.py`

 * *Files identical despite different names*

### Comparing `TruMusic-1.1.6/tru_music/scripts/trumusic.py` & `TruMusic-1.1.7/tru_music/scripts/trumusic.py`

 * *Files identical despite different names*

