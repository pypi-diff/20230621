# Comparing `tmp/neon-skill-local_music-0.3.1a1.tar.gz` & `tmp/neon-skill-local_music-0.3.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-local_music-0.3.1a1.tar", last modified: Thu Jun 15 22:07:06 2023, max compression
+gzip compressed data, was "neon-skill-local_music-0.3.1a2.tar", last modified: Wed Jun 21 00:00:39 2023, max compression
```

## Comparing `neon-skill-local_music-0.3.1a1.tar` & `neon-skill-local_music-0.3.1a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:06.760129 neon-skill-local_music-0.3.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-15 22:07:06.760129 neon-skill-local_music-0.3.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:06.756129 neon-skill-local_music-0.3.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:06.756129 neon-skill-local_music-0.3.1a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:06.760129 neon-skill-local_music-0.3.1a1/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/locale/en-us/vocab/local.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:06.760129 neon-skill-local_music-0.3.1a1/neon_skill_local_music.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-15 22:07:06.000000 neon-skill-local_music-0.3.1a1/neon_skill_local_music.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-15 22:07:06.000000 neon-skill-local_music-0.3.1a1/neon_skill_local_music.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:07:06.000000 neon-skill-local_music-0.3.1a1/neon_skill_local_music.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:07:06.000000 neon-skill-local_music-0.3.1a1/neon_skill_local_music.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 22:07:06.000000 neon-skill-local_music-0.3.1a1/neon_skill_local_music.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 22:07:06.000000 neon-skill-local_music-0.3.1a1/neon_skill_local_music.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:07:06.760129 neon-skill-local_music-0.3.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:06.760129 neon-skill-local_music-0.3.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:06.760129 neon-skill-local_music-0.3.1a1/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/ui/music-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:07:06.760129 neon-skill-local_music-0.3.1a1/util/
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:07:03.000000 neon-skill-local_music-0.3.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:00:39.709290 neon-skill-local_music-0.3.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-21 00:00:39.709290 neon-skill-local_music-0.3.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:00:39.705290 neon-skill-local_music-0.3.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:00:39.705290 neon-skill-local_music-0.3.1a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:00:39.705290 neon-skill-local_music-0.3.1a2/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/locale/en-us/vocab/local.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:00:39.705290 neon-skill-local_music-0.3.1a2/neon_skill_local_music.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-21 00:00:39.000000 neon-skill-local_music-0.3.1a2/neon_skill_local_music.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-21 00:00:39.000000 neon-skill-local_music-0.3.1a2/neon_skill_local_music.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:00:39.000000 neon-skill-local_music-0.3.1a2/neon_skill_local_music.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 00:00:39.000000 neon-skill-local_music-0.3.1a2/neon_skill_local_music.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 00:00:39.000000 neon-skill-local_music-0.3.1a2/neon_skill_local_music.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 00:00:39.000000 neon-skill-local_music-0.3.1a2/neon_skill_local_music.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 00:00:39.709290 neon-skill-local_music-0.3.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:00:39.709290 neon-skill-local_music-0.3.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:00:39.709290 neon-skill-local_music-0.3.1a2/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/ui/music-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:00:39.709290 neon-skill-local_music-0.3.1a2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-21 00:00:35.000000 neon-skill-local_music-0.3.1a2/version.py
```

### Comparing `neon-skill-local_music-0.3.1a1/LICENSE.md` & `neon-skill-local_music-0.3.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-0.3.1a1/PKG-INFO` & `neon-skill-local_music-0.3.1a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-local_music
-Version: 0.3.1a1
+Version: 0.3.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-local_music
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-local_music-0.3.1a1/README.md` & `neon-skill-local_music-0.3.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-0.3.1a1/__init__.py` & `neon-skill-local_music-0.3.1a2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from threading import Thread
 from typing import List
 from os.path import join, dirname, expanduser, isdir
 from random import sample
 
 from ovos_plugin_common_play import MediaType, PlaybackType
 from ovos_workshop.skills.common_play import OVOSCommonPlaybackSkill, \
     ocp_search
@@ -82,23 +83,25 @@
         return self._music_library
 
     # TODO: Move to __init__ after ovos-workshop stable release
     def initialize(self):
         # TODO: add intent to update library?
         if self.music_dir and isdir(self.music_dir):
             LOG.debug(f"Load configured directory: {self.music_dir}")
-            self.music_library.update_library(self.music_dir)
+            Thread(target=self.music_library.update_library,
+                   args=(self.music_dir,), daemon=True).start()
         user_dir = expanduser("~/Music")
         if isdir(user_dir):
             LOG.debug(f"Load default directory: {self.music_dir}")
-            self.music_library.update_library(user_dir)
+            Thread(target=self.music_library.update_library, args=(user_dir,),
+                   daemon=True).start()
         if self.demo_url and not isdir(self._demo_dir):
             LOG.info(f"Downloading Demo Music from: {self.demo_url}")
-            self._download_demo_tracks()
-        if isdir(self._demo_dir):
+            Thread(target=self._download_demo_tracks, daemon=True).start()
+        elif isdir(self._demo_dir):
             self.music_library.update_library(self._demo_dir)
 
     @ocp_search()
     def search_music(self, phrase, media_type=MediaType.GENERIC):
         results = self.search_artist(phrase, media_type) + \
             self.search_album(phrase, media_type) + \
             self.search_genre(phrase, media_type) + \
@@ -169,7 +172,8 @@
                    'length': track.duration_ms,
                    'match_confidence': score} for track in tracks]
         return tracks
 
     def _download_demo_tracks(self):
         from ovos_skill_installer import download_extract_zip
         download_extract_zip(self.demo_url, self._demo_dir)
+        self.music_library.update_library(self._demo_dir)
```

### Comparing `neon-skill-local_music-0.3.1a1/neon_skill_local_music.egg-info/PKG-INFO` & `neon-skill-local_music-0.3.1a2/neon_skill_local_music.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-local-music
-Version: 0.3.1a1
+Version: 0.3.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-local_music
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-local_music-0.3.1a1/setup.py` & `neon-skill-local_music-0.3.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-0.3.1a1/skill.json` & `neon-skill-local_music-0.3.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-0.3.1a1/test/test_skill.py` & `neon-skill-local_music-0.3.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-0.3.1a1/util/__init__.py` & `neon-skill-local_music-0.3.1a2/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import hashlib
 import pickle
+from threading import RLock
 from typing import List, Optional
 import ovos_ocp_files_plugin
 
 from dataclasses import dataclass
 from os import walk, makedirs, remove
 from os.path import join, expanduser, isfile, dirname, basename, splitext, isdir
 from ovos_utils.log import LOG
@@ -55,27 +56,29 @@
     def __init__(self, library_path: str, cache_path: str):
         """
         Initialize a Library object for the specified path, optionally loading
         a cached index at the specified `cache_file` path.
         :param library_path: path to scan for music files
         :param cache_path: path to cache directory for library and temp files
         """
+        self._update_lock = RLock()
         self.library_paths = [expanduser(library_path)]
         self.cache_path = expanduser(cache_path)
         if not isdir(self.cache_path):
             makedirs(self.cache_path)
         self._songs = dict()
         self._db_file = join(self.cache_path, "library.pickle")
-        try:
-            if isfile(self._db_file):
-                with open(self._db_file, 'rb') as f:
-                    self._songs = pickle.load(f)
-        except Exception as e:
-            LOG.exception(e)
-            remove(self._db_file)
+        with self._update_lock:
+            try:
+                if isfile(self._db_file):
+                    with open(self._db_file, 'rb') as f:
+                        self._songs = pickle.load(f)
+            except Exception as e:
+                LOG.exception(e)
+                remove(self._db_file)
 
     @property
     def all_songs(self):
         return list(self._songs.values())
 
     def search_songs_for_artist(self, artist: str) -> List[Track]:
         """
@@ -120,25 +123,27 @@
                 elif file.startswith('.'):
                     LOG.debug(f"Ignoring hidden file: {file}")
                     continue
                 elif not splitext(file)[1]:
                     LOG.debug(f"Ignoring file with no extension: {file}")
                     continue
                 abs_path = join(root, file)
-                if abs_path in self._songs:
-                    LOG.debug(f"Ignoring already indexed track: {abs_path}")
-                    continue
-                self._songs[abs_path] = self._parse_track_from_file(abs_path,
-                                                                    album_art)
+                with self._update_lock:
+                    if abs_path in self._songs:
+                        LOG.debug(f"Ignoring already indexed track: {abs_path}")
+                        continue
+                    self._songs[abs_path] = \
+                        self._parse_track_from_file(abs_path, album_art)
         LOG.debug("Updated Library")
-        try:
-            with open(self._db_file, 'wb') as f:
-                pickle.dump(self._songs, f)
-        except Exception as e:
-            LOG.exception(e)
+        with self._update_lock:
+            try:
+                with open(self._db_file, 'wb') as f:
+                    pickle.dump(self._songs, f)
+            except Exception as e:
+                LOG.exception(e)
 
     def _parse_track_from_file(self, file_path: str,
                                album_art: Optional[str] = None):
         try:
             meta = ovos_ocp_files_plugin.load(file_path)
             image_bytes = meta.pictures[0].data if meta.pictures else None
             album = meta.tags['album'][0]
```

### Comparing `neon-skill-local_music-0.3.1a1/version.py` & `neon-skill-local_music-0.3.1a2/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.1a1"
+__version__ = "0.3.1a2"
```

