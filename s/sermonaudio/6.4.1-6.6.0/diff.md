# Comparing `tmp/sermonaudio-6.4.1.tar.gz` & `tmp/sermonaudio-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sermonaudio-6.4.1.tar", last modified: Mon Jun 15 15:50:16 2020, max compression
+gzip compressed data, was "sermonaudio-6.6.0.tar", last modified: Wed Jan 27 18:37:23 2021, max compression
```

## Comparing `sermonaudio-6.4.1.tar` & `sermonaudio-6.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-15 15:50:16.221818 sermonaudio-6.4.1/
--rw-r--r--   0 root         (0) root         (0)     4288 2020-06-15 15:50:16.221818 sermonaudio-6.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3136 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      249 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-15 15:50:16.221818 sermonaudio-6.4.1/sermonaudio/
--rw-rw-rw-   0 root         (0) root         (0)     6218 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/sermonaudio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-15 15:50:16.221818 sermonaudio-6.4.1/sermonaudio/broadcaster/
--rw-rw-rw-   0 root         (0) root         (0)       55 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/sermonaudio/broadcaster/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12591 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/sermonaudio/broadcaster/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    24951 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/sermonaudio/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-15 15:50:16.221818 sermonaudio-6.4.1/sermonaudio/node/
--rw-rw-rw-   0 root         (0) root         (0)       28 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/sermonaudio/node/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26716 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/sermonaudio/node/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/sermonaudio/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-06-15 15:50:16.221818 sermonaudio-6.4.1/sermonaudio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4288 2020-06-15 15:50:16.000000 sermonaudio-6.4.1/sermonaudio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      404 2020-06-15 15:50:16.000000 sermonaudio-6.4.1/sermonaudio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-06-15 15:50:16.000000 sermonaudio-6.4.1/sermonaudio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2020-06-15 15:50:16.000000 sermonaudio-6.4.1/sermonaudio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2020-06-15 15:50:16.000000 sermonaudio-6.4.1/sermonaudio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-06-15 15:50:16.221818 sermonaudio-6.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      892 2020-06-15 15:49:02.000000 sermonaudio-6.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-27 18:37:23.447590 sermonaudio-6.6.0/
+-rw-r--r--   0 root         (0) root         (0)     4288 2021-01-27 18:37:23.447590 sermonaudio-6.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3136 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      249 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-27 18:37:23.447590 sermonaudio-6.6.0/sermonaudio/
+-rw-rw-rw-   0 root         (0) root         (0)     6218 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/sermonaudio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-27 18:37:23.447590 sermonaudio-6.6.0/sermonaudio/broadcaster/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/sermonaudio/broadcaster/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12607 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/sermonaudio/broadcaster/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    26527 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/sermonaudio/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-27 18:37:23.447590 sermonaudio-6.6.0/sermonaudio/node/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/sermonaudio/node/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26868 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/sermonaudio/node/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/sermonaudio/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-27 18:37:23.447590 sermonaudio-6.6.0/sermonaudio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4288 2021-01-27 18:37:23.000000 sermonaudio-6.6.0/sermonaudio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      404 2021-01-27 18:37:23.000000 sermonaudio-6.6.0/sermonaudio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-27 18:37:23.000000 sermonaudio-6.6.0/sermonaudio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2021-01-27 18:37:23.000000 sermonaudio-6.6.0/sermonaudio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2021-01-27 18:37:23.000000 sermonaudio-6.6.0/sermonaudio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-01-27 18:37:23.447590 sermonaudio-6.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      892 2021-01-27 18:35:40.000000 sermonaudio-6.6.0/setup.py
```

### Comparing `sermonaudio-6.4.1/PKG-INFO` & `sermonaudio-6.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sermonaudio
-Version: 6.4.1
+Version: 6.6.0
 Summary: The official Python client library for accessing the SermonAudio.com APIs
 Home-page: http://api.sermonaudio.com/
 Author: SermonAudio.com
 Author-email: info@sermonaudio.com
 License: MIT
 Description: SermonAudio.com API Client Library
         ==================================
```

### Comparing `sermonaudio-6.4.1/README.md` & `sermonaudio-6.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sermonaudio-6.4.1/sermonaudio/__init__.py` & `sermonaudio-6.6.0/sermonaudio/__init__.py`

 * *Files identical despite different names*

### Comparing `sermonaudio-6.4.1/sermonaudio/broadcaster/requests.py` & `sermonaudio-6.6.0/sermonaudio/broadcaster/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,17 @@
         if event_type:
             params["audioEventType"] = event_type.value
 
         return cls.patch(path, data=params, parse_func=check_response_code_or_throw)
 
     @classmethod
     def set_highlighted_sort_order(
-        cls, broadcaster_id: str, sort_order: models.HighlightedSortOrders,
+        cls,
+        broadcaster_id: str,
+        sort_order: models.HighlightedSortOrders,
     ) -> bool:  # pragma: no cover
         """Sets a broadcaster's highlighted sort order.
 
         Broadcasters have a short list of sermons on their home page,
         and this sort order controls how they are sorted. See the
         HighlightedSortOrders enum for more details.
```

### Comparing `sermonaudio-6.4.1/sermonaudio/models.py` & `sermonaudio-6.6.0/sermonaudio/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,17 @@
 
         self.welcome_video_id = obj["welcomeVideoID"]
         assert isinstance_or_none(self.welcome_video_id, str)
 
         self.country_iso_code = obj["countryISOCode"]
         assert isinstance_or_none(self.country_iso_code, str)
 
+        self.language_code = obj["languageCode"]
+        assert isinstance_or_none(self.language_code, str)
+
     def get_album_art_url(self, size: int):  # pragma: no cover
         """Returns a URL for the square album art with a with and height equal to the provided size argument"""
         return self.album_art_url_format.replace("{size}", str(size))
 
     def __str__(self):  # pragma: no cover
         return f'<Broadcaster {self.broadcaster_id} "{self.display_name}">'
 
@@ -252,14 +255,19 @@
 
         self.download_url = obj.get("downloadURL")
         assert isinstance_or_none(self.download_url, str)
 
         self.bitrate = obj["bitrate"]
         assert isinstance_or_none(self.bitrate, int)
 
+        try:
+            self.file_size_bytes = obj["fileSizeBytes"]
+        except ValueError:
+            self.file_size_bytes = None
+
         self.duration = obj["duration"]
         assert isinstance_or_none(self.duration, int)
 
         self.audio_codec = obj["audioCodec"]
         assert isinstance_or_none(self.audio_codec, str)
 
         self.video_codec = obj["videoCodec"]
@@ -304,20 +312,31 @@
         assert isinstance_or_none(self.subtitle, str)
 
         self.series = SermonSeries.parse(obj["series"]) if obj.get("series") else None
 
         self.preach_date = datetime.datetime.strptime(obj["preachDate"], "%Y-%m-%d").date()
         assert isinstance(self.preach_date, datetime.date)
 
+        # A sermon may be picked as a staff pick by SermonAudio.
         try:
             self.staff_pick_date = datetime.datetime.strptime(obj["pickDate"], "%Y-%m-%d").date()
             assert isinstance_or_none(self.staff_pick_date, datetime.date)
         except (TypeError, ValueError):
             self.staff_pick_date = None
 
+        # A sermon may be featured by a broadcaster by going to a sermon's page
+        # and selecting the option to feature it. This given the sermon a high
+        # level of visibility at SermonAudio. The last feature date is reported
+        # by the API, since a sermon can be featured more than once.
+        try:
+            self.last_feature_date = datetime.datetime.strptime(obj["lastFeatureDate"], "%Y-%m-%d").date()
+            assert isinstance_or_none(self.last_feature_date, datetime.date)
+        except (TypeError, ValueError):
+            self.last_feature_date = None
+
         timestamp = obj["publishTimestamp"]
         self.publish_timestamp = datetime.datetime.fromtimestamp(timestamp, pytz.utc) if timestamp is not None else None
 
         update_date = obj["updateDate"]
         self.update_date = datetime.datetime.fromtimestamp(update_date, pytz.utc)
 
         self.language_code = obj["languageCode"]
@@ -400,17 +419,28 @@
         assert isinstance(self.total_tune_in_count, int)
 
         self.total_listen_line_count = obj["totalListenLineCount"]
         assert isinstance(self.total_listen_line_count, int)
 
         self.media = MediaSet.parse(obj["media"])
 
+        # The field archived_sermon_id has been deprecated. Originally, one
+        # webcast could be archived to one sermon. By popular demand, we
+        # relaxed this requirement so one webcast could be archived to multiple
+        # sermons. If your webcast is linked to one sermon, this field will
+        # have the sermon ID of that sermon for backwards
+        # compatibility. Otherwise, it will be None. We recommend that you use
+        # the archived_sermons field, which is a list of sermon IDs that have
+        # been created from this webcast.
         self.archived_sermon_id = obj["archivedSermonID"]
         assert isinstance_or_none(self.archived_sermon_id, str)
 
+        self.archived_sermons = obj["archivedSermons"]
+        assert isinstance_or_none(self.archived_sermons, list)
+
     def __str__(self):  # pragma: no cover
         return f'<WebcastInfo {self.broadcaster_id} "{self.display_name}"">'
 
 
 class RelativeBroadcasterLocation(Model):
     def __init__(self, obj: dict):
         super().__init__(obj)
@@ -652,15 +682,15 @@
         pass it to Node.get_sermons().
 
         Example:
             highlighted_sermons  = Node.get_highlighted_sermons()
             params = highlighted_sermons.sort_order.sermon_parameters
             # ... update params...
             sermons = Node.get_sermons(**params)
-            """
+        """
 
         if self is self.ADDED:
             return {"sort_by": SermonSortOption.ADDED}
         elif self is self.NEWEST_PICKS:
             return {"listener_recommended": True, "sort_by": SermonSortOption.NEWEST}
         elif self is self.RANDOM_PICKS:
             return {"listener_recommended": True, "sort_by": SermonSortOption.RANDOM}
```

### Comparing `sermonaudio-6.4.1/sermonaudio/node/requests.py` & `sermonaudio-6.6.0/sermonaudio/node/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         series: Optional[str] = None,
         broadcaster_id: str = None,
         sermon_ids: [str] = None,
         speaker_name: str = None,
         year: Optional[int] = None,
         sort_by: Optional[Union[models.HighlightedSortOrders, models.SermonSortOption]] = None,
         staff_pick: bool = False,
+        featured: bool = False,
         listener_recommended: bool = False,
         updated: bool = False,
         include_drafts: bool = False,
         include_scheduled: bool = False,
         include_published: bool = True,
         **kwargs,
     ) -> PaginatedResponse:  # noqa: F821
@@ -109,14 +110,15 @@
         :param series: The series to limit results to (may be an ID or name).
         :param broadcaster_id: The ID of the broadcaster to limit results to.
         :param sermon_ids: A set of sermon IDs to return. This option ignores most others.
         :param speaker_name: The speaker name to limit results to.
         :param year: The year to limit results to (preach date, not upload date).
         :param sort_by: A sort to apply to the results. Defaults to preach date descending.
         :param staff_pick: List only sermons that are SermonAudio staff picks.
+        :param featured: List only sermons that were featured by the broadcaster.
         :param listener_recommended: List only sermons that have been recommended by listeners.
         :param include_drafts: If true, include sermons with no publish date.
         :param include_scheduled: If true, include sermons set to be published in the future.
         :param include_published: If true, include published sermons.
         :param highlighted_sermon_sort: If included, use the sort order determined by the
         value of this parameter. If a highlighted sermon sort is included, it overrides
         other sort/filter options.
@@ -159,14 +161,15 @@
                 "series": series,
                 "broadcasterID": broadcaster_id,
                 "sermonIDs": ",".join(sermon_ids) if sermon_ids else None,
                 "speakerName": speaker_name,
                 "year": year,
                 "sortBy": sort_by.value if sort_by else None,
                 "staffPick": staff_pick,
+                "featured": featured,
                 "listenerRecommended": listener_recommended,
                 "includeDrafts": include_drafts,
                 "includeScheduled": include_scheduled,
                 "includePublished": include_published,
             },
         )
```

### Comparing `sermonaudio-6.4.1/sermonaudio/utils.py` & `sermonaudio-6.6.0/sermonaudio/utils.py`

 * *Files identical despite different names*

### Comparing `sermonaudio-6.4.1/sermonaudio.egg-info/PKG-INFO` & `sermonaudio-6.6.0/sermonaudio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sermonaudio
-Version: 6.4.1
+Version: 6.6.0
 Summary: The official Python client library for accessing the SermonAudio.com APIs
 Home-page: http://api.sermonaudio.com/
 Author: SermonAudio.com
 Author-email: info@sermonaudio.com
 License: MIT
 Description: SermonAudio.com API Client Library
         ==================================
```

### Comparing `sermonaudio-6.4.1/setup.py` & `sermonaudio-6.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as fp:
     readme = fp.read()
 
 setup(
     name="sermonaudio",
-    version="6.4.1",
+    version="6.6.0",
     description="The official Python client library for accessing the SermonAudio.com APIs",
     long_description=readme,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

