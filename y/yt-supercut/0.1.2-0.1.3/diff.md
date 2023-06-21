# Comparing `tmp/yt_supercut-0.1.2.tar.gz` & `tmp/yt_supercut-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_supercut-0.1.2.tar", max compression
+gzip compressed data, was "yt_supercut-0.1.3.tar", max compression
```

## Comparing `yt_supercut-0.1.2.tar` & `yt_supercut-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       14 2023-05-29 21:15:44.453273 yt_supercut-0.1.2/README.md
--rw-r--r--   0        0        0      683 2023-06-14 16:40:51.040996 yt_supercut-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5959 2023-06-02 19:36:34.711692 yt_supercut-0.1.2/yt_supercut/db.py
--rw-r--r--   0        0        0     3542 2023-06-05 16:10:34.390386 yt_supercut-0.1.2/yt_supercut/main.py
--rw-r--r--   0        0        0     3522 2023-06-14 16:38:36.753352 yt_supercut-0.1.2/yt_supercut/utils.py
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 yt_supercut-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-05-29 21:15:44.453273 yt_supercut-0.1.3/README.md
+-rw-r--r--   0        0        0      702 2023-06-21 20:18:44.447684 yt_supercut-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6072 2023-06-19 02:56:18.515490 yt_supercut-0.1.3/yt_supercut/db.py
+-rw-r--r--   0        0        0     3813 2023-06-21 19:47:48.838530 yt_supercut-0.1.3/yt_supercut/main.py
+-rw-r--r--   0        0        0     4206 2023-06-21 20:10:07.117721 yt_supercut-0.1.3/yt_supercut/utils.py
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 yt_supercut-0.1.3/PKG-INFO
```

### Comparing `yt_supercut-0.1.2/pyproject.toml` & `yt_supercut-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yt-supercut"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["redraw <redraw@sdf.org>"]
 readme = "README.md"
 packages = [{include = "yt_supercut"}]
 
 [tool.poetry.scripts]
 yt-supercut = "yt_supercut.main:cli"
@@ -15,14 +15,15 @@
 yt-dlp = "^2023.3.4"
 datasette = {version = "^0.64.3", extras = ["datasette"]}
 datasette-youtube-embed = {version = "^0.1", extras = ["datasette"]}
 tqdm = "^4.65.0"
 webvtt-py = "^0.4.6"
 tabulate = "^0.9.0"
 sqlite-utils = "^3.32.1"
+appdirs = "^1.4.4"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.13.2"
 ipdb = "^0.13.13"
 
 
 [build-system]
```

### Comparing `yt_supercut-0.1.2/yt_supercut/db.py` & `yt_supercut-0.1.3/yt_supercut/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,20 +184,26 @@
 
 def get_videos():
     db = get_db()
     for video in db["videos"].rows:
         yield video
 
 
+def get_video_languages():
+    db = get_db()
+    for video_language in db["video_languages"].rows:
+        yield video_language
+
+
 def filter_existing_video_ids(video_ids, lang):
     db = get_db()
     db.execute("CREATE TEMPORARY TABLE IF NOT EXISTS tmp (video_id TEXT NOT NULL PRIMARY KEY)")
     db["tmp"].insert_all([{"video_id": video_id} for video_id in video_ids])
     for row in db["tmp"].rows_where(
-        "video_id not in (select video_id from video_languages where lang = :lang or available = 0)",
+        "video_id not in (select video_id from video_languages where lang = :lang)",
         {"lang": lang},
     ):
         yield row["video_id"]
     db["tmp"].drop()
 
 
 def get_video(video_id):
```

### Comparing `yt_supercut-0.1.2/yt_supercut/main.py` & `yt_supercut-0.1.3/yt_supercut/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 from pathlib import Path
 import subprocess
-import typer
+from typing import List, Optional
 import threading
 import concurrent.futures
+
+import typer
 from tqdm import tqdm
 from tabulate import tabulate
 from . import db, utils
 
 cli = typer.Typer()
 lock = threading.Lock()
 
@@ -16,18 +18,19 @@
 
 
 @cli.command()
 def index(
     url: str,
     lang: str = "es",
     verbose: bool = False,
-    max_threads: int = None,
+    max_threads: Optional[int] = None,
+    cookies_from: Optional[str] = None,
 ):
     print(f"Fetching video urls from {url}...")
-    video_ids = list(utils.get_video_ids(url, verbose=verbose))
+    video_ids = list(utils.get_video_ids(url, cookies_from=cookies_from, lang=lang, verbose=verbose))
     new_ids = list(db.filter_existing_video_ids(video_ids, lang))
 
     # download and index subs in parallel
     with concurrent.futures.ThreadPoolExecutor(max_threads) as executor:
         tasks = (
             executor.submit(
                 utils.download_and_process_subtitles,
@@ -118,27 +121,30 @@
     db.delete_channel(uploader_id)
 
 
 @cli.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
     help="Run datasette, supports all datasette options",
 )
-def server(ctx: typer.Context):
+def server(ctx: typer.Context, port: str = "8001"):
     try:
         import datasette
     except ImportError:
         typer.echo("datasette not installed. Run `pip install yt-supercut[datasette]`")
         raise typer.Exit(1)
 
     args = [
         "datasette",
         db.DB_PATH,
         "--metadata",
         str(Path().parent / "metadata.json"),
+        "--port",
+        port,
         *ctx.args
     ] 
 
+    print(f"When server is ready, open http://localhost:{port}/youtube/subtitles_with_videos")
     subprocess.run(args)
 
 
 if __name__ == "__main__":
-    cli()
+    cli()
```

### Comparing `yt_supercut-0.1.2/PKG-INFO` & `yt_supercut-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: yt-supercut
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: redraw
 Author-email: redraw@sdf.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: datasette-youtube-embed[datasette] (>=0.1,<0.2)
 Requires-Dist: datasette[datasette] (>=0.64.3,<0.65.0)
 Requires-Dist: sqlite-utils (>=3.32.1,<4.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: webvtt-py (>=0.4.6,<0.5.0)
```

