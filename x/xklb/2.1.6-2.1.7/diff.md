# Comparing `tmp/xklb-2.1.6.tar.gz` & `tmp/xklb-2.1.7.tar.gz`

## Comparing `xklb-2.1.6.tar` & `xklb-2.1.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.6/.gitattributes
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.6/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.6/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-2.1.6/pdm.lock
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.6/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/books.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/consts.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/dl_config.py
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/gui.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/hn_extract.py
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/lb.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/media.py
--rw-r--r--   0        0        0    25386 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/play_actions.py
--rw-r--r--   0        0        0    34451 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/playlists.py
--rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/praw_extract.py
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/subtitle.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/tube_backend.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/tube_extract.py
--rw-r--r--   0        0        0    83349 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/usage.py
--rw-r--r--   0        0        0    41240 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.6/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.6/LICENSE
--rw-r--r--   0        0        0    94113 2020-02-02 00:00:00.000000 xklb-2.1.6/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.6/pyproject.toml
--rw-r--r--   0        0        0    97739 2020-02-02 00:00:00.000000 xklb-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.7/.gitattributes
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.7/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.7/Windows.md
+-rw-r--r--   0        0        0   490400 2020-02-02 00:00:00.000000 xklb-2.1.7/pdm.lock
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.7/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/books.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/consts.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/dl_config.py
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/gui.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/lb.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/media.py
+-rw-r--r--   0        0        0    25386 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/play_actions.py
+-rw-r--r--   0        0        0    34705 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/playlists.py
+-rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/subtitle.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/tube_extract.py
+-rw-r--r--   0        0        0    83349 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/usage.py
+-rw-r--r--   0        0        0    41240 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.7/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.7/LICENSE
+-rw-r--r--   0        0        0    94113 2020-02-02 00:00:00.000000 xklb-2.1.7/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0    97739 2020-02-02 00:00:00.000000 xklb-2.1.7/PKG-INFO
```

### Comparing `xklb-2.1.6/TODO` & `xklb-2.1.7/TODO`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/Windows.md` & `xklb-2.1.7/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/pdm.lock` & `xklb-2.1.7/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -641,15 +641,15 @@
 name = "pillow"
 version = "9.5.0"
 requires_python = ">=3.7"
 summary = "Python Imaging Library (Fork)"
 
 [[package]]
 name = "platformdirs"
-version = "3.6.0"
+version = "3.7.0"
 requires_python = ">=3.7"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 requires_python = ">=3.6"
@@ -881,15 +881,15 @@
     "markdown-it-py>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.272"
+version = "0.0.274"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
 name = "scalene"
 version = "1.5.19"
 requires_python = ">=3.8"
@@ -1243,15 +1243,15 @@
 dependencies = [
     "idna>=2.0",
     "multidict>=4.0",
 ]
 
 [[package]]
 name = "yt-dlp"
-version = "2023.3.4"
+version = "2023.6.21"
 requires_python = ">=3.7"
 summary = "A youtube-dl fork with additional features and patches"
 dependencies = [
     "brotli; platform_python_implementation == \"CPython\"",
     "brotlicffi; platform_python_implementation != \"CPython\"",
     "certifi",
     "mutagen",
@@ -2519,17 +2519,17 @@
     {url = "https://files.pythonhosted.org/packages/d9/0e/7c6f054022235830dc2c37ec83e947d9ca09b0b0361e1e5e29983da92294/Pillow-9.5.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb841572862f629b99725ebaec3287fc6d275be9b14443ea746c1dd325053cbd"},
     {url = "https://files.pythonhosted.org/packages/db/5c/ba9e291850f594f89436cdca93d36c6f8610d4fb7833a6c257f4481d4174/Pillow-9.5.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:662da1f3f89a302cc22faa9f14a262c2e3951f9dbc9617609a47521c69dd9f8f"},
     {url = "https://files.pythonhosted.org/packages/e7/2a/f3ed578595f8486ee2cc07434460097d89aedd406a3db849b890ca8ec416/Pillow-9.5.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:a127ae76092974abfbfa38ca2d12cbeddcdeac0fb71f9627cc1135bedaf9d51a"},
     {url = "https://files.pythonhosted.org/packages/ec/7d/01404982db598f271ac7c0d0207860f60ab9288cfacce9872eb567cfbfe3/Pillow-9.5.0-cp37-cp37m-macosx_10_10_x86_64.whl", hash = "sha256:5d4ebf8e1db4441a55c509c4baa7a0587a0210f7cd25fcfe74dbbce7a4bd1906"},
     {url = "https://files.pythonhosted.org/packages/f2/43/0892913d499c8df2c88dee69d59e77de19e0c51754a9be82023880641c09/Pillow-9.5.0-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8aca1152d93dcc27dc55395604dcfc55bed5f25ef4c98716a928bacba90d33a3"},
     {url = "https://files.pythonhosted.org/packages/ff/fc/48a51c0fe2a00d5def57b9981a1e0f8339b516351da7a51500383d833bc8/Pillow-9.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:608488bdcbdb4ba7837461442b90ea6f3079397ddc968c31265c1e056964f1ef"},
 ]
-"platformdirs 3.6.0" = [
-    {url = "https://files.pythonhosted.org/packages/05/31/793923615e85deef0c25abf5d044b3f99f1348b620122ab184b7d3f70f21/platformdirs-3.6.0.tar.gz", hash = "sha256:57e28820ca8094678b807ff529196506d7a21e17156cb1cddb3e74cebce54640"},
-    {url = "https://files.pythonhosted.org/packages/a7/4d/00f9fe4bbb3459da0d6c790b1526e5edebaeff2a80166eabb0a42f9e0a05/platformdirs-3.6.0-py3-none-any.whl", hash = "sha256:ffa199e3fbab8365778c4a10e1fbf1b9cd50707de826eb304b50e57ec0cc8d38"},
+"platformdirs 3.7.0" = [
+    {url = "https://files.pythonhosted.org/packages/14/62/d8277379c30fc6b0347aaf8ff63e5c9e013e0da95f40ba957c5e098b06c2/platformdirs-3.7.0-py3-none-any.whl", hash = "sha256:cfd065ba43133ff103ab3bd10aecb095c2a0035fcd1f07217c9376900d94ba07"},
+    {url = "https://files.pythonhosted.org/packages/a1/45/ff5224bbf1a9f23d95f70890659a7c2639a25d594adfe4a5ca9221f6cae5/platformdirs-3.7.0.tar.gz", hash = "sha256:87fbf6473e87c078d536980ba970a472422e94f17b752cfad17024c18876d481"},
 ]
 "pluggy 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/9e/01/f38e2ff29715251cf25532b9082a1589ab7e4f571ced434f98d0139336dc/pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
     {url = "https://files.pythonhosted.org/packages/a1/16/db2d7de3474b6e37cbb9c008965ee63835bba517e22cdb8c35b5116b5ce1/pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
 ]
 "praw 7.7.0" = [
     {url = "https://files.pythonhosted.org/packages/b3/93/55ae62910b94b46ecdd0ee8765289304f8df8deeaa1df7a96b0831c637ff/praw-7.7.0-py3-none-any.whl", hash = "sha256:22155c4b3006733a5ab0754136cf2226917747b61ec037ee335246fe0db5420e"},
@@ -2900,32 +2900,32 @@
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
 "rich 13.4.2" = [
     {url = "https://files.pythonhosted.org/packages/e3/12/67d0098eb77005f5e068de639e6f4cfb8f24e6fcb0fd2037df0e1d538fee/rich-13.4.2.tar.gz", hash = "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"},
     {url = "https://files.pythonhosted.org/packages/fc/1e/482e5eec0b89b593e81d78f819a9412849814e22225842b598908e7ac560/rich-13.4.2-py3-none-any.whl", hash = "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec"},
 ]
-"ruff 0.0.272" = [
-    {url = "https://files.pythonhosted.org/packages/1f/12/1b0b513ccf7a0ea19430843bf3a82b51704a1c8001900ca99066b69270ec/ruff-0.0.272-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:691d72a00a99707a4e0b2846690961157aef7b17b6b884f6b4420a9f25cd39b5"},
-    {url = "https://files.pythonhosted.org/packages/2e/96/1a4b3b9c658bf2a04ba7820aefa24d8561f73379bf0d79c2f01321c4dd84/ruff-0.0.272-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:d5a208f8ef0e51d4746930589f54f9f92f84bb69a7d15b1de34ce80a7681bc00"},
-    {url = "https://files.pythonhosted.org/packages/48/cb/2e8b7d690eec62a16971f15ca018248bc9058fb2d6abf0588f1fcc9fafb4/ruff-0.0.272-py3-none-win_arm64.whl", hash = "sha256:06b8ee4eb8711ab119db51028dd9f5384b44728c23586424fd6e241a5b9c4a3b"},
-    {url = "https://files.pythonhosted.org/packages/4a/8f/66590b978ceeb3d62eee4f46eeabff4a4967cde81c05e9d4e8a28ca18f7d/ruff-0.0.272-py3-none-win_amd64.whl", hash = "sha256:a37ec80e238ead2969b746d7d1b6b0d31aa799498e9ba4281ab505b93e1f4b28"},
-    {url = "https://files.pythonhosted.org/packages/4b/f8/50874f1992355a8c565bc6322659abf7cc86ce2e929ea4930d14768a022b/ruff-0.0.272-py3-none-musllinux_1_2_i686.whl", hash = "sha256:19643d448f76b1eb8a764719072e9c885968971bfba872e14e7257e08bc2f2b7"},
-    {url = "https://files.pythonhosted.org/packages/67/d5/ce76ab5f37f647bdbed63b857c47c275620ad34b1a062529c5514675c5ee/ruff-0.0.272.tar.gz", hash = "sha256:273a01dc8c3c4fd4c2af7ea7a67c8d39bb09bce466e640dd170034da75d14cab"},
-    {url = "https://files.pythonhosted.org/packages/6a/cd/5ef249cd71029d869edb858171d108ea001c98baab7c1e88123d7a49c86b/ruff-0.0.272-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:1609b864a8d7ee75a8c07578bdea0a7db75a144404e75ef3162e0042bfdc100d"},
-    {url = "https://files.pythonhosted.org/packages/6e/41/8d0ceacc7e5be1f54f9c5cf22ad80541e8751ffa4b6870d801ad082257e7/ruff-0.0.272-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:677284430ac539bb23421a2b431b4ebc588097ef3ef918d0e0a8d8ed31fea216"},
-    {url = "https://files.pythonhosted.org/packages/6e/ff/6864326dc773a5467a06369cb1125391424b86478ed8f242bffb835b10a8/ruff-0.0.272-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:905ff8f3d6206ad56fcd70674453527b9011c8b0dc73ead27618426feff6908e"},
-    {url = "https://files.pythonhosted.org/packages/74/a8/c6a072ae54cb9144086b0437e9febc638e52d7c4e4520e197395cf6b1e7a/ruff-0.0.272-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:48eccf225615e106341a641f826b15224b8a4240b84269ead62f0afd6d7e2d95"},
-    {url = "https://files.pythonhosted.org/packages/91/81/5d65b3ed9a0e02f14275df6e2e1e1d95495af0a429256ab998a35d2de104/ruff-0.0.272-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:ae9b57546e118660175d45d264b87e9b4c19405c75b587b6e4d21e6a17bf4fdf"},
-    {url = "https://files.pythonhosted.org/packages/98/9c/932d41fe80ec408a8a618b61ee7f36a99d67b99b70de480f8ab1d2771af0/ruff-0.0.272-py3-none-win32.whl", hash = "sha256:dc406e5d756d932da95f3af082814d2467943631a587339ee65e5a4f4fbe83eb"},
-    {url = "https://files.pythonhosted.org/packages/98/b7/478cf23d492f07ca13b45b7efa2c43660e3a4a229623f3f196022631e387/ruff-0.0.272-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ee76b4f05fcfff37bd6ac209d1370520d509ea70b5a637bdf0a04d0c99e13dff"},
-    {url = "https://files.pythonhosted.org/packages/c5/74/25a315f9020f05e5f8508467d930bff61667514260ab03505397fb293cf0/ruff-0.0.272-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:9c4bfb75456a8e1efe14c52fcefb89cfb8f2a0d31ed8d804b82c6cf2dc29c42c"},
-    {url = "https://files.pythonhosted.org/packages/d6/ae/8018ccae4f6757d1b6c0e3b1c6ca5fbe2f0a9c83474b9abc468b76b2ba26/ruff-0.0.272-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:86bc788245361a8148ff98667da938a01e1606b28a45e50ac977b09d3ad2c538"},
-    {url = "https://files.pythonhosted.org/packages/e2/1a/c0e7f3b10550f53113bdb671b509171f54e7c3fbec99b7114561c99c5cc2/ruff-0.0.272-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:27b2ea68d2aa69fff1b20b67636b1e3e22a6a39e476c880da1282c3e4bf6ee5a"},
-    {url = "https://files.pythonhosted.org/packages/e3/f8/c8242e21cd82e0e2d6403e54d62d2dff66a6bf5f221455ba3496363de0a3/ruff-0.0.272-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bd2bbe337a3f84958f796c77820d55ac2db1e6753f39d1d1baed44e07f13f96d"},
+"ruff 0.0.274" = [
+    {url = "https://files.pythonhosted.org/packages/07/59/7b043efe280a7f6815c87fda4bf1e43e51c87b181f3b461bd761e29377f7/ruff-0.0.274-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:fa9ad8776cb92f2739b8eee316cde841d6012d0eafbf06bae09166203ddf9bb8"},
+    {url = "https://files.pythonhosted.org/packages/18/26/3ee1c9717fa206318be9eb892b8326ac415f1a57952aa996fd7b88435126/ruff-0.0.274-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:044084f039a679e557240fefcf521e057941b163014cf969ac6d04620861e04a"},
+    {url = "https://files.pythonhosted.org/packages/30/ad/9dc28c29b8fbb390f2f08c5e2e961c9b2adf2d71549f78ac4f310f392b30/ruff-0.0.274-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:dca36d651f88b4b24f17df5db54487057ce0ccd3599cbf38d237cf4d9f0d63c2"},
+    {url = "https://files.pythonhosted.org/packages/36/a2/7b226d7586607e3991646961b29a15d1f923fa8459f0015114c80394e82c/ruff-0.0.274-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:023cdc5e64b3f34244e12bd236ab412c6056061a2415d50fb862cab333b4ab7c"},
+    {url = "https://files.pythonhosted.org/packages/39/24/e60dfe0b610a13a716bb4fb574c6e4365c7404a16d8352b27edf6d6b1ee9/ruff-0.0.274-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:6d7069157a5674be8090c7d89fa69dbb2478f333a80b1312d20ade2a870cca3e"},
+    {url = "https://files.pythonhosted.org/packages/73/31/3cc256943d29025793279244fd6837240382edd3c585f3b562a62b66deb6/ruff-0.0.274.tar.gz", hash = "sha256:c7e5f9deffbd02d8054f90b565a1106faee64e16cedf50f3aa05c14b59ff8727"},
+    {url = "https://files.pythonhosted.org/packages/7b/d1/029f18d1ad0456c01e23ec40c99c817be7593ce345711ec02683ff8092bf/ruff-0.0.274-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:86d943107f20fec924f56dc4933cefb0efbc1ec8b729e0a1afabac598c5586ca"},
+    {url = "https://files.pythonhosted.org/packages/7f/60/f8d4966112555805366ec2df37e3653d4d80adbc1b00bf4254dbbd9e340d/ruff-0.0.274-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:587130943110e9536018ce139158e2962d46623f379a4486aabfd525e9714b0e"},
+    {url = "https://files.pythonhosted.org/packages/84/7c/21841a330cd8e162ccc848d99e84a3cb27416cd7eb983cc17b082a6469ec/ruff-0.0.274-py3-none-musllinux_1_2_i686.whl", hash = "sha256:b13e765b64487143f05e6ad6f624388b9ac5a6ff8657ff801091c9282de3ca52"},
+    {url = "https://files.pythonhosted.org/packages/b5/da/694e37da2604444f0c5a4dc5eb5cf23af02622d9b4638dc343997a84d3fd/ruff-0.0.274-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:34e71a06a4e27554ca2f1c2b1749a802e3e76cac41481cfc2cb86936c1e37d3c"},
+    {url = "https://files.pythonhosted.org/packages/b9/4b/25f1f00393db9a4d018039b7a39fca5164c6cb5b251caba7abd8ccd8f957/ruff-0.0.274-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6133fa856b230a0281197aeba3e89ce9595f9d8a7265113520ad259d416c9f4b"},
+    {url = "https://files.pythonhosted.org/packages/b9/d9/2dd3f535a211a73754c764212a52d7db70e9d55f9263a963b9b95e779dfe/ruff-0.0.274-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:461bda8c3a4c1591fd7a09960b86e2ffc9a59a1c42cf14d725077314c12b60b0"},
+    {url = "https://files.pythonhosted.org/packages/bd/7d/57ccbca1428cd4876bf68decfc465b2725ce5234da91fb4c4910443de0f5/ruff-0.0.274-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:5137f853fffa7352901038a1b5e36a97058380a554763e534aae9f6c0734fdab"},
+    {url = "https://files.pythonhosted.org/packages/c6/ec/fdd733bddd74cee9293cf235505f7e865d435306e24543ca590910f1260c/ruff-0.0.274-py3-none-win_amd64.whl", hash = "sha256:e80aa0c7e1347a96db846287695971925eb56760c019a7d66312fbca389a6800"},
+    {url = "https://files.pythonhosted.org/packages/cf/0b/bf76ae7566952fb0675537ea8730a567c416ba35cd23c95e70b3ea07139f/ruff-0.0.274-py3-none-win_arm64.whl", hash = "sha256:8b99ce776fc60fb938791f558b297e53ed634adeef1a7b84a33455924948c9af"},
+    {url = "https://files.pythonhosted.org/packages/e1/95/1debc53b970c97a991f15c01e6650e76b7e35c8cd4945b0a9a33ec2c53cc/ruff-0.0.274-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:39b80156ef57b33ab7bfc454b7c2678eaae07f43a7dcf2e7c058f72d87b49538"},
+    {url = "https://files.pythonhosted.org/packages/e6/4a/c09cde430f6aa48e98f0384d49e9612e4f22e2429f745e3e9eca30075f53/ruff-0.0.274-py3-none-win32.whl", hash = "sha256:09c87fa2c4f53bd63c1d8a35150683794b022f4f2fbd6ef2fe383ce21ab53fec"},
 ]
 "scalene 1.5.19" = [
     {url = "https://files.pythonhosted.org/packages/11/19/c973ecc43b18076df6c7efff7bec280d02d48d8245f46d94b7e90cf306f2/scalene-1.5.19-cp39-cp39-win_amd64.whl", hash = "sha256:d1fd5d83f3c022ddc46049f29823351b8dbdb8590f5803358fa6034784601f24"},
     {url = "https://files.pythonhosted.org/packages/19/54/d89426ab970f1cb3850b0374967ae22d831d0091efeb2c1d8e8d02ac2a19/scalene-1.5.19-cp39-cp39-macosx_11_7_universal2.whl", hash = "sha256:6c08f3bc0b6355db3c34f0e9aea1b291e64675bb832e19758ee751918787cac0"},
     {url = "https://files.pythonhosted.org/packages/49/11/5a2fa4567eee217609e0a627534f5fb60d0c1f768b43a93145a2ea24e39b/scalene-1.5.19-cp38-cp38-manylinux_2_24_x86_64.whl", hash = "sha256:f67f39321548c06de440319bdd70c41c14b6c50d4748226a101402995677cade"},
     {url = "https://files.pythonhosted.org/packages/5e/3c/b1f159a11f0949f3f27b18af1cc68ee301088a7337efc7d961684bdd3f46/scalene-1.5.19-cp37-cp37m-macosx_10_15_universal2.whl", hash = "sha256:58fb40d031081a55e813f292b2d85b64d7558a372832d8e456f7fe2113adf182"},
     {url = "https://files.pythonhosted.org/packages/65/c3/ebaf00eef807b8da6c5b0c4eb6627f0a67538a25ac7e3858347e15c55d22/scalene-1.5.19-cp38-cp38-win_amd64.whl", hash = "sha256:7a1d452ad4d32cf8adb8b86cae4e5b9c7bff866fff1c43618f9ad114b9ecac32"},
@@ -3311,17 +3311,17 @@
     {url = "https://files.pythonhosted.org/packages/f0/cc/cf416dff5bd88899a567fea556a5f68ab94cdf525ebe122e0bdba478f2c4/yarl-1.9.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:52a25809fcbecfc63ac9ba0c0fb586f90837f5425edfd1ec9f3372b119585e45"},
     {url = "https://files.pythonhosted.org/packages/f1/0c/c2e07b3a37c4363078a1c7d586b251eec191594a2d24d6e09dae33c1368f/yarl-1.9.2-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:1b1bba902cba32cdec51fca038fd53f8beee88b77efc373968d1ed021024cc04"},
     {url = "https://files.pythonhosted.org/packages/f2/b1/9a6eeba1a3f35188eac6b7b535f20c06df0f48e78705405d86a0407e75f1/yarl-1.9.2-cp38-cp38-win32.whl", hash = "sha256:f7a3d8146575e08c29ed1cd287068e6d02f1c7bdff8970db96683b9591b86ee7"},
     {url = "https://files.pythonhosted.org/packages/f2/ea/6fd350376ed2581d0cdb11018bad0215cf987817dba69ea9a4bf8adbac6e/yarl-1.9.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:8288d7cd28f8119b07dd49b7230d6b4562f9b61ee9a4ab02221060d21136be80"},
     {url = "https://files.pythonhosted.org/packages/fb/2d/060ab740f64ea6ea2088e375c3046839faaf4bbba2b65a5364668bd765e7/yarl-1.9.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59"},
     {url = "https://files.pythonhosted.org/packages/fe/7d/9d85f658b6f7c041ca3ba371d133040c4dc41eb922aef0a6ba917291d187/yarl-1.9.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb"},
 ]
-"yt-dlp 2023.3.4" = [
-    {url = "https://files.pythonhosted.org/packages/a7/df/498c57f641e9993376cf52489047158e6d660e8bab06b72c470ad5cce2bd/yt_dlp-2023.3.4-py2.py3-none-any.whl", hash = "sha256:40ca421407ce07c8fd700854fd978d58526ec6fff3468caa34ff1c7333b8dc34"},
-    {url = "https://files.pythonhosted.org/packages/e8/4a/1e01f24fcb49191626e2b17d00e13a093315d03a9da09fccb1c75913e420/yt-dlp-2023.3.4.tar.gz", hash = "sha256:265d5da97a76c15d7d9a4088a67b78acd5dcf6f8cfd8257c52f581ff996ff515"},
+"yt-dlp 2023.6.21" = [
+    {url = "https://files.pythonhosted.org/packages/36/9a/13eee74e6a621ab42d2b8c7fd7daf6e943af1a8269aa966718fae177a64b/yt-dlp-2023.6.21.tar.gz", hash = "sha256:56c35d1ad3ecfb828c3b89ffe07b235b354eddd82e1a31ddc3d16eb8c3e71e8e"},
+    {url = "https://files.pythonhosted.org/packages/45/27/02df242aba3ccb6b02457c4063113add4c7b06af46f1cd5bc75b9856656f/yt_dlp-2023.6.21-py2.py3-none-any.whl", hash = "sha256:e4117b1ee07878c7dade2a64e6102fb7840fa1e3f19365cca42ce291754f35cf"},
 ]
 "zeroconf 0.69.0" = [
     {url = "https://files.pythonhosted.org/packages/04/f9/b89ba913563eca7ad5cf80d066d14df68c8a1614731b07a5cc238c7680cb/zeroconf-0.69.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:9e2cfe4baa6540e21cbb74d820a1bf8f3258449bee92be1cba289033fe77f0c9"},
     {url = "https://files.pythonhosted.org/packages/0b/30/0d5cb2bf0a29e844748c039d7ceb13008a376e2af95c6b51f4a8754ed494/zeroconf-0.69.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:ff92c07ff69156cb496d001700afd06959c37b80731c78c5ce896f4f3aebfe21"},
     {url = "https://files.pythonhosted.org/packages/0b/31/516fd6b8512190e94896ece6c37f9be244611ea2c64877a3ea0227ef532d/zeroconf-0.69.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:1dea30128d618a46d489809a55a932a5797c353b5d9a3dc5ed63d5d5887a7e97"},
     {url = "https://files.pythonhosted.org/packages/0b/5a/03a16379942dd478099eddc92316e4b1be37928797fa12ed592353360482/zeroconf-0.69.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:0a7a34989a88eacd4948e8a04c5b9ed5757df8684a09fb85e8f3d374b57903e5"},
     {url = "https://files.pythonhosted.org/packages/15/72/34dbc01948cf279175f4d042405caefeb90e720cfcb9988b370ca8dee052/zeroconf-0.69.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d1d543bc558e526ae217848c508c737d74be678712ebd226fc3d8335762b807f"},
```

### Comparing `xklb-2.1.6/readme.py` & `xklb-2.1.7/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.1.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.1.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/.github/workflows/push.yaml` & `xklb-2.1.7/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/av.py` & `xklb-2.1.7/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/books.py` & `xklb-2.1.7/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/consts.py` & `xklb-2.1.7/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/db.py` & `xklb-2.1.7/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/dl_config.py` & `xklb-2.1.7/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/dl_extract.py` & `xklb-2.1.7/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/fs_extract.py` & `xklb-2.1.7/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/gdl_backend.py` & `xklb-2.1.7/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/gdl_extract.py` & `xklb-2.1.7/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/gui.py` & `xklb-2.1.7/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/history.py` & `xklb-2.1.7/xklb/history.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,9 +19,10 @@
         {
             "media_id": media_id,
             "time_played": time_played or consts.now(),
             "playhead": playhead,
             "done": mark_done,
         }
         for media_id in media_ids
+        if media_id
     ]
     args.db["history"].insert_all(utils.list_dict_filter_bool(rows), pk="id", alter=True)
```

### Comparing `xklb-2.1.6/xklb/hn_extract.py` & `xklb-2.1.7/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/lb.py` & `xklb-2.1.7/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/media.py` & `xklb-2.1.7/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/play_actions.py` & `xklb-2.1.7/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/player.py` & `xklb-2.1.7/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,17 +329,22 @@
         raise ValueError("Unrecognized action:", action)
 
 
 def override_sort(sort_expression: str) -> str:
     def year_month_sql(var):
         return f"cast(strftime('%Y%m', datetime({var}, 'unixepoch')) as int)"
 
+    def year_month_day_sql(var):
+        return f"cast(strftime('%Y%m%d', datetime({var}, 'unixepoch')) as int)"
+
     return (
         sort_expression.replace("month_created", year_month_sql("time_created"))
         .replace("month_modified", year_month_sql("time_modified"))
+        .replace("date_created", year_month_day_sql("time_created"))
+        .replace("date_modified", year_month_day_sql("time_modified"))
         .replace("random", "random()")
         .replace("priority", "ntile(1000) over (order by size) desc, duration")
     )
 
 
 def filter_args_sql(args, m_columns):
     return f"""
```

### Comparing `xklb-2.1.6/xklb/playlists.py` & `xklb-2.1.7/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/praw_extract.py` & `xklb-2.1.7/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/search.py` & `xklb-2.1.7/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/subtitle.py` & `xklb-2.1.7/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/tabs_actions.py` & `xklb-2.1.7/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/tabs_extract.py` & `xklb-2.1.7/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/tube_backend.py` & `xklb-2.1.7/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/tube_extract.py` & `xklb-2.1.7/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/usage.py` & `xklb-2.1.7/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/utils.py` & `xklb-2.1.7/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/bigdirs.py` & `xklb-2.1.7/xklb/scripts/bigdirs.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library bigdirs",
         usage=usage.bigdirs,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--sort-by")
+    parser.add_argument("--sort-by", "--sort", "-u")
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="4000")
     parser.add_argument("--depth", "-d", default=0, type=int, help="Depth of folders")
     parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
     parser.add_argument(
         "--folder-size",
         "--foldersize",
@@ -159,15 +159,21 @@
 def process_bigdirs(args, media) -> List[Dict]:
     folders = group_files_by_folder(args, media)
     if args.depth:
         folders = folder_depth(args, folders)
     if args.folder_size:
         args.folder_size = utils.parse_human_to_lambda(utils.human_to_bytes, args.folder_size)
         folders = [d for d in folders if args.folder_size(d["size"])]
-    return sorted(folders, key=sort_by(args))
+
+    reverse = False
+    if " desc" in args.sort_by:
+        args.sort_by = args.sort_by.replace(" desc", "")
+        reverse = True
+
+    return sorted(folders, key=sort_by(args), reverse=reverse)
 
 
 def bigdirs() -> None:
     args = parse_args()
     history.create(args)
 
     tbl = get_table(args)
```

### Comparing `xklb-2.1.6/xklb/scripts/block.py` & `xklb-2.1.7/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/christen.py` & `xklb-2.1.7/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/cluster_sort.py` & `xklb-2.1.7/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/copy_play_counts.py` & `xklb-2.1.7/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/dedupe.py` & `xklb-2.1.7/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/dedupe_db.py` & `xklb-2.1.7/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/download_status.py` & `xklb-2.1.7/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/history.py` & `xklb-2.1.7/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/merge_dbs.py` & `xklb-2.1.7/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/merge_online_local.py` & `xklb-2.1.7/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/move_list.py` & `xklb-2.1.7/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/optimize_db.py` & `xklb-2.1.7/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/playback_control.py` & `xklb-2.1.7/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/playlists.py` & `xklb-2.1.7/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/redownload.py` & `xklb-2.1.7/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/relmv.py` & `xklb-2.1.7/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/scatter.py` & `xklb-2.1.7/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/streaming_tab_loader.py` & `xklb-2.1.7/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/mining/data.py` & `xklb-2.1.7/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/mining/extract_links.py` & `xklb-2.1.7/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.1.7/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/mining/nouns.py` & `xklb-2.1.7/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/mining/pushshift.py` & `xklb-2.1.7/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.1.7/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/xklb/assets/kotobago.png` & `xklb-2.1.7/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/.gitignore` & `xklb-2.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/LICENSE` & `xklb-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/README.md` & `xklb-2.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.1.006)
+    xk media library subcommands (v2.1.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-2.1.6/pyproject.toml` & `xklb-2.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.6/PKG-INFO` & `xklb-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.1.6
+Version: 2.1.7
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.1.006)
+    xk media library subcommands (v2.1.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

