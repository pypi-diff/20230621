# Comparing `tmp/libretrofuzz-3.2.7.tar.gz` & `tmp/libretrofuzz-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.2.7.tar", max compression
+gzip compressed data, was "libretrofuzz-3.2.8.tar", max compression
```

## Comparing `libretrofuzz-3.2.7.tar` & `libretrofuzz-3.2.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-20 23:03:31.440023 libretrofuzz-3.2.7/LICENSE
--rw-r--r--   0        0        0     7554 2023-06-20 23:03:31.440023 libretrofuzz-3.2.7/README.rst
--rw-r--r--   0        0        0       22 2023-06-20 23:03:31.440023 libretrofuzz-3.2.7/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    56546 2023-06-20 23:03:31.440023 libretrofuzz-3.2.7/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-20 23:03:31.440023 libretrofuzz-3.2.7/pyproject.toml
--rw-r--r--   0        0        0     8735 2023-06-20 23:03:43.286915 libretrofuzz-3.2.7/setup.py
--rw-r--r--   0        0        0     8743 2023-06-20 23:03:43.287989 libretrofuzz-3.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 08:36:06.704917 libretrofuzz-3.2.8/LICENSE
+-rw-r--r--   0        0        0     7554 2023-06-21 08:36:06.704917 libretrofuzz-3.2.8/README.rst
+-rw-r--r--   0        0        0       22 2023-06-21 08:36:06.708917 libretrofuzz-3.2.8/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    56530 2023-06-21 08:36:06.708917 libretrofuzz-3.2.8/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-21 08:36:06.708917 libretrofuzz-3.2.8/pyproject.toml
+-rw-r--r--   0        0        0     8735 2023-06-21 08:36:24.404552 libretrofuzz-3.2.8/setup.py
+-rw-r--r--   0        0        0     8743 2023-06-21 08:36:24.405743 libretrofuzz-3.2.8/PKG-INFO
```

### Comparing `libretrofuzz-3.2.7/LICENSE` & `libretrofuzz-3.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.7/README.rst` & `libretrofuzz-3.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.7/libretrofuzz/__main__.py` & `libretrofuzz-3.2.8/libretrofuzz/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
 # -------------------------------------------------------------------
 class TitleScorer(object):
     def __init__(self, normcache, normcache2, hack):
         self.normcache = normcache
         self.normcache2 = normcache2
         self.hack = hack
 
-    def __call__(self, name, other, processor=None, score_cutoff=None):
+    def __call__(self, name, other, score_cutoff=None):
         if name == other:
             return MAX_SCORE
         (_, name_ns, _, _, digits) = self.normcache[name]
         (_, other_ns, _, other_ns_subs, other_digits) = self.normcache2[other]
         if name_ns == other_ns:
             return MAX_SCORE
```

### Comparing `libretrofuzz-3.2.7/pyproject.toml` & `libretrofuzz-3.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.2.7"
+version = "3.2.8"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 beautifulsoup4 = "^4.10.0"
 questionary = "^1.10.0"
 typer = {extras = ["all"], version = "^0.9.0"}
-rapidfuzz = "^2.4.2"
+rapidfuzz = "^3.1.1"
 httpx = "^0.23.0"
 tqdm = "^4.65.0"
 prompt_toolkit = "^3.0.30"
 pillow = "^9.2.0"
 regex = "^2023.6.3"
 
 [tool.black]
```

### Comparing `libretrofuzz-3.2.7/setup.py` & `libretrofuzz-3.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 install_requires = \
 ['beautifulsoup4>=4.10.0,<5.0.0',
  'httpx>=0.23.0,<0.24.0',
  'pillow>=9.2.0,<10.0.0',
  'prompt_toolkit>=3.0.30,<4.0.0',
  'questionary>=1.10.0,<2.0.0',
- 'rapidfuzz>=2.4.2,<3.0.0',
+ 'rapidfuzz>=3.1.1,<4.0.0',
  'regex>=2023.6.3,<2024.0.0',
  'tqdm>=4.65.0,<5.0.0',
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.2.7',
+    'version': '3.2.8',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 15 --delay-after 15`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use ``--min 100``.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload because the glob used matches all names that start with 'Ishar' or 'ishar'.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no delay or image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.2.7/PKG-INFO` & `libretrofuzz-3.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.2.7
+Version: 3.2.8
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: pillow (>=9.2.0,<10.0.0)
 Requires-Dist: prompt_toolkit (>=3.0.30,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Requires-Dist: rapidfuzz (>=2.4.2,<3.0.0)
+Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/i30817/libretrofuzz/issues
 Project-URL: Repository, https://github.com/i30817/libretrofuzz
 Project-URL: documentation, https://github.com/i30817/libretrofuzz#readme
 Project-URL: homepage, https://github.com/i30817/libretrofuzz
```

