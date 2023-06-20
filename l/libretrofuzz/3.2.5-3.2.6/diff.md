# Comparing `tmp/libretrofuzz-3.2.5.tar.gz` & `tmp/libretrofuzz-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.2.5.tar", max compression
+gzip compressed data, was "libretrofuzz-3.2.6.tar", max compression
```

## Comparing `libretrofuzz-3.2.5.tar` & `libretrofuzz-3.2.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-19 22:57:22.042057 libretrofuzz-3.2.5/LICENSE
--rw-r--r--   0        0        0     7554 2023-06-19 22:57:22.042057 libretrofuzz-3.2.5/README.rst
--rw-r--r--   0        0        0       22 2023-06-19 22:57:22.042057 libretrofuzz-3.2.5/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    56164 2023-06-19 22:57:22.042057 libretrofuzz-3.2.5/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-19 22:57:22.046057 libretrofuzz-3.2.5/pyproject.toml
--rw-r--r--   0        0        0     8735 2023-06-19 22:57:30.851495 libretrofuzz-3.2.5/setup.py
--rw-r--r--   0        0        0     8743 2023-06-19 22:57:30.852433 libretrofuzz-3.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-20 22:21:22.485369 libretrofuzz-3.2.6/LICENSE
+-rw-r--r--   0        0        0     7554 2023-06-20 22:21:22.485369 libretrofuzz-3.2.6/README.rst
+-rw-r--r--   0        0        0       22 2023-06-20 22:21:22.485369 libretrofuzz-3.2.6/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    56238 2023-06-20 22:21:22.485369 libretrofuzz-3.2.6/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-20 22:21:22.485369 libretrofuzz-3.2.6/pyproject.toml
+-rw-r--r--   0        0        0     8735 2023-06-20 22:21:35.243968 libretrofuzz-3.2.6/setup.py
+-rw-r--r--   0        0        0     8743 2023-06-20 22:21:35.245027 libretrofuzz-3.2.6/PKG-INFO
```

### Comparing `libretrofuzz-3.2.5/LICENSE` & `libretrofuzz-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.5/README.rst` & `libretrofuzz-3.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.5/libretrofuzz/__main__.py` & `libretrofuzz-3.2.6/libretrofuzz/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1233,15 +1233,16 @@
     reset again and only waits once per game
     """
     while True:
         try:
             async with client.stream("GET", url, timeout=15) as r:
                 if r.status_code == 521:  # cloudflare exploded, skip the whole playlist
                     raise StopPlaylist()
-                if r.status_code == 404:  # broken image or symlink link, skip just this thumb
+                # broken image or symlink link, skip just this thumb
+                if r.status_code == 400 or r.status_code == 404 or r.status_code == 410:
                     return False
                 r.raise_for_status()  # error before reading the header goes into retrying
                 length = int(r.headers["Content-Length"])
                 if length < 100:  # obviously corrupt 'thumbnail', skip this thumb
                     return False
                 if not dryrun:  # test
                     with open(destination, "w+b") as f:
@@ -1256,17 +1257,17 @@
                             leave=False,
                         ) as w:
                             async for chunk in r.aiter_raw(4096):
                                 with handleContinueDownload():
                                     checkDownload()
                                 w.write(chunk)
             return True
-        except (RequestError, HTTPStatusError):
+        except (RequestError, HTTPStatusError) as e:
             if max_retries <= 0:
-                error("Download max retries exceeded, exiting")
+                error(f"Download max retries exceeded, exiting: {e}")
                 raise Exit(code=1)
             max_retries -= 1
 
 
 def displayImages(downloaded: dict):
     """dict has all the tuple (old, new)
     with the key of the thumbnail type str (the files may not exist)
```

### Comparing `libretrofuzz-3.2.5/pyproject.toml` & `libretrofuzz-3.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.2.5"
+version = "3.2.6"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.2.5/setup.py` & `libretrofuzz-3.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.2.5',
+    'version': '3.2.6',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 15 --delay-after 15`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use ``--min 100``.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload because the glob used matches all names that start with 'Ishar' or 'ishar'.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no delay or image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.2.5/PKG-INFO` & `libretrofuzz-3.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.2.5
+Version: 3.2.6
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

