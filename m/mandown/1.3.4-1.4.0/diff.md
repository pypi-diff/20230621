# Comparing `tmp/mandown-1.3.4.tar.gz` & `tmp/mandown-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mandown-1.3.4.tar", max compression
+gzip compressed data, was "mandown-1.4.0.tar", max compression
```

## Comparing `mandown-1.3.4.tar` & `mandown-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0    34520 2023-01-19 04:32:59.935926 mandown-1.3.4/LICENSE
--rw-r--r--   0        0        0     3819 2023-02-26 21:02:31.227352 mandown-1.3.4/README.md
--rw-r--r--   0        0        0      523 2023-04-27 21:56:31.915371 mandown-1.3.4/mandown/__init__.py
--rw-r--r--   0        0        0    11018 2023-04-09 22:54:34.442921 mandown-1.3.4/mandown/api.py
--rw-r--r--   0        0        0     1700 2022-12-31 01:43:12.048313 mandown-1.3.4/mandown/base.py
--rw-r--r--   0        0        0    15780 2023-04-09 22:50:30.475038 mandown-1.3.4/mandown/cli.py
--rw-r--r--   0        0        0     2564 2023-01-19 03:47:14.110630 mandown-1.3.4/mandown/comic.py
--rw-r--r--   0        0        0     5549 2023-04-09 23:00:40.166019 mandown-1.3.4/mandown/io.py
--rw-r--r--   0        0        0     5102 2023-01-29 00:07:27.899107 mandown-1.3.4/mandown/processor/__init__.py
--rw-r--r--   0        0        0     4109 2022-12-31 00:17:08.710330 mandown-1.3.4/mandown/processor/ops.py
--rw-r--r--   0        0        0     1603 2022-12-31 00:17:08.710330 mandown-1.3.4/mandown/processor/profiles.py
--rw-r--r--   0        0        0     1428 2023-04-09 22:52:14.729134 mandown-1.3.4/mandown/sources/__init__.py
--rw-r--r--   0        0        0     2017 2022-12-23 01:36:28.689150 mandown-1.3.4/mandown/sources/base_source.py
--rw-r--r--   0        0        0     4938 2023-01-29 00:08:10.853514 mandown-1.3.4/mandown/sources/source_mangadex.py
--rw-r--r--   0        0        0     2561 2022-10-06 18:48:03.141061 mandown-1.3.4/mandown/sources/source_mangakakalot.py
--rw-r--r--   0        0        0     2697 2023-03-16 22:50:42.471198 mandown-1.3.4/mandown/sources/source_manganato.py
--rw-r--r--   0        0        0     3744 2022-10-06 18:48:03.142061 mandown-1.3.4/mandown/sources/source_mangasee.py
--rw-r--r--   0        0        0     3617 2023-03-16 22:46:08.667522 mandown-1.3.4/mandown/sources/source_readcomiconline.py
--rw-r--r--   0        0        0     4116 2023-03-28 15:47:14.408606 mandown-1.3.4/mandown/sources/source_webtoons.py
--rw-r--r--   0        0        0     4597 2022-10-06 18:48:03.142061 mandown-1.3.4/mandown/ui/form.ui
--rw-r--r--   0        0        0     7214 2022-10-06 18:48:03.143061 mandown-1.3.4/mandown/ui/mainwin.py
--rw-r--r--   0        0        0       38 2022-10-06 18:48:03.143061 mandown-1.3.4/mandown/ui/mandown-qt.pyproject
--rw-r--r--   0        0        0     7049 2022-10-06 18:48:03.143061 mandown-1.3.4/mandown/ui/ui.py
--rw-r--r--   0        0        0     1406 2023-04-27 21:56:20.091790 mandown-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 mandown-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3845 2023-06-21 03:20:51.716586 mandown-1.4.0/README.md
+-rw-r--r--   0        0        0      523 2023-04-28 17:41:44.918635 mandown-1.4.0/mandown/__init__.py
+-rw-r--r--   0        0        0    11958 2023-06-21 02:16:52.907651 mandown-1.4.0/mandown/api.py
+-rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.4.0/mandown/base.py
+-rw-r--r--   0        0        0    16688 2023-06-20 22:27:01.443946 mandown-1.4.0/mandown/cli.py
+-rw-r--r--   0        0        0     2564 2023-04-28 17:41:44.917635 mandown-1.4.0/mandown/comic.py
+-rw-r--r--   0        0        0      682 2023-06-20 22:05:26.357720 mandown-1.4.0/mandown/convert_utils.py
+-rw-r--r--   0        0        0     5549 2023-04-28 17:41:44.918635 mandown-1.4.0/mandown/io.py
+-rw-r--r--   0        0        0     5102 2023-04-28 17:41:44.926635 mandown-1.4.0/mandown/processor/__init__.py
+-rw-r--r--   0        0        0     4109 2023-04-28 17:41:44.926635 mandown-1.4.0/mandown/processor/ops.py
+-rw-r--r--   0        0        0     1603 2023-04-28 17:41:44.926635 mandown-1.4.0/mandown/processor/profiles.py
+-rw-r--r--   0        0        0     1449 2023-06-21 02:53:38.485548 mandown-1.4.0/mandown/sources/__init__.py
+-rw-r--r--   0        0        0     2017 2023-04-28 17:41:44.919635 mandown-1.4.0/mandown/sources/base_source.py
+-rw-r--r--   0        0        0     4938 2023-04-28 17:41:44.919635 mandown-1.4.0/mandown/sources/source_mangadex.py
+-rw-r--r--   0        0        0     2569 2023-06-21 02:59:09.077067 mandown-1.4.0/mandown/sources/source_mangakakalot.py
+-rw-r--r--   0        0        0     2697 2023-04-28 17:41:44.920635 mandown-1.4.0/mandown/sources/source_manganato.py
+-rw-r--r--   0        0        0     3744 2023-04-28 17:41:44.920635 mandown-1.4.0/mandown/sources/source_mangasee.py
+-rw-r--r--   0        0        0     3051 2023-06-21 02:58:11.800715 mandown-1.4.0/mandown/sources/source_manhuaes.py
+-rw-r--r--   0        0        0     3599 2023-06-21 02:59:45.366868 mandown-1.4.0/mandown/sources/source_readcomiconline.py
+-rw-r--r--   0        0        0     4116 2023-04-28 17:41:44.920635 mandown-1.4.0/mandown/sources/source_webtoons.py
+-rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.4.0/mandown/ui/form.ui
+-rw-r--r--   0        0        0     7214 2023-04-28 17:41:44.928635 mandown-1.4.0/mandown/ui/mainwin.py
+-rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.4.0/mandown/ui/mandown-qt.pyproject
+-rw-r--r--   0        0        0     7049 2023-04-28 17:41:44.928635 mandown-1.4.0/mandown/ui/ui.py
+-rw-r--r--   0        0        0     1398 2023-06-21 03:26:10.118172 mandown-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 mandown-1.4.0/PKG-INFO
```

### Comparing `mandown-1.3.4/LICENSE` & `mandown-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/README.md` & `mandown-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,14 @@
   - Rotate or split double-page spreads
   - Trim borders
   - Resize images
 - Convert downloaded comics to CBZ, EPUB, or PDF
   - Convert any other CBZ, EPUB, or PDF comic to CBZ, EPUB, or PDF
 - [A library to easily do all of this from other Python scripts](#basic-library-usage)
 
-## Supported sites
-
-To request a new site, please file a [new issue](https://github.com/potatoeggy/mandown/issues/new?title=Source%20request:).
-
-- <https://mangasee123.com>
-- <https://manganato.com>
-- <https://webtoons.com>
-- <https://mangadex.org>
-- <https://mangakakalot.com>
-- <https://readcomiconline.li>
-
 ## Usage
 
 Run `mandown --help` or see the [docs](/docs/) for more information and examples.
 
 ```
 mandown get <URL>
 ```
@@ -46,15 +35,15 @@
 
 ```
 mandown get <URL> --convert epub --process rotate_double_pages
 ```
 
 To download only a certain range of chapters, append the `--start` and/or `--end` options.
 
-> **Note:** `--start` and `--end` are *inclusive*, i.e., using `--start 2 --end 3` will download chapters 2 and 3.
+> **Note:** `--start` and `--end` are _inclusive_, i.e., using `--start 2 --end 3` will download chapters 2 and 3.
 
 To convert an existing folder or comic file without downloading anything (like a stripped-down version of <https://github.com/ciromattia/kcc>), use the `convert` command.
 
 ```
 mandown convert <FORMAT> <PATH_TO_COMIC>
 ```
 
@@ -94,14 +83,27 @@
 
 ```
 git clone https://github.com/potatoeggy/mandown.git
 poetry install
 poetry build
 pip3 install dist/mandown*.whl
 ```
+
+## Supported sites
+
+To request a new site, please file a [new issue](https://github.com/potatoeggy/mandown/issues/new?title=Source%20request:).
+
+- <https://mangasee123.com>
+- <https://manganato.com>
+- <https://webtoons.com>
+- <https://mangadex.org>
+- <https://mangakakalot.com>
+- <https://manhuaes.com>
+- <https://readcomiconline.li>
+
 ## Basic library usage
 
 See the [docs](/docs/) for more information and examples.
 
 To just download the images:
 
 ```python
```

### Comparing `mandown-1.3.4/mandown/__init__.py` & `mandown-1.4.0/mandown/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/api.py` & `mandown-1.4.0/mandown/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 # pylint: disable=invalid-name
 
 import shutil
-from enum import Enum
 from pathlib import Path
 from typing import Iterator
 
 import comicon
 
 from . import io, sources
 from .comic import BaseComic
+from .convert_utils import ConvertFormats, convert_one
 from .processor import ProcessConfig, ProcessOps, Processor
 
 
-class ConvertFormats(str, Enum):
-    """
-    The formats that mandown can convert to. This is used for the `--format` option.
-    """
-
-    # for typing purposes
-    CBZ = "cbz"
-    EPUB = "epub"
-    PDF = "pdf"
-    NONE = "none"
-
-
 def query(url: str) -> BaseComic:
     """
     Attempt to query for a comic given a URL.
     :param `url`: An internet URL to search for
     :raises `ValueError` if the source is not found.
     """
     adapter = sources.get_class_for(url)(url)
@@ -93,24 +81,27 @@
 
 
 def convert_progress(
     comic_path: Path | str,
     to: ConvertFormats,
     dest_folder: Path | str | None = None,
     remove_after: bool = False,
+    split_by_chapters: bool = False,
 ) -> Iterator[str | int]:
     """
     Convert the comic located at `folder_path` to `convert_to`
     and put it in `dest_folder` (defaults to workdir).
 
     :param `comic_path`: The path to the comic to convert (may be in Mandown
     folder form or any of the `mandown.ConvertFormats` such as EPUB)
     :param `convert_to`: The format to convert to
     :param `dest_folder`: A folder to put the converted comic in
     :param `remove_after`: If `True`, delete the original file/folder after conversion
+    :param `split_by_chapters`: Only applies to Mandown-created comics. If `True`,
+    output a comic file per chapter. Existing comic files will not be overwritten.
 
     :returns An `Iterator` representing a progress bar. The first iteration returns
     the remaining number of iterations. If converting between file formats, an
     iteration after the first number of iterations ends will return the remaining
     number of the second number of iterations.
     """
     comic_path = Path(comic_path)
@@ -123,36 +114,60 @@
     if comic_path.is_dir():
         # it's a mandown comic, convert it to CIR
         comic = load(comic_path)
 
         # find cover
         cover: str | None = None
         for item in comic_path.iterdir():
-            if str(item).startswith("cover"):
+            if item.name.startswith("cover"):
                 cover = item.name
                 break
 
-        comicon_comic = comicon.Comic(
-            comicon.Metadata(
-                title=comic.metadata.title,
-                authors=comic.metadata.authors,
-                description=comic.metadata.description,
-                genres=comic.metadata.genres,
-                cover_path_rel=cover,
-            ),
-            [comicon.Chapter(chap.title, chap.slug) for chap in comic.chapters],
-        )
+        if split_by_chapters:
+            comicon_comics = [
+                comicon.Comic(
+                    comicon.Metadata(
+                        title=f"{comic.metadata.title} - {chap.title}",
+                        authors=comic.metadata.authors,
+                        description=comic.metadata.description,
+                        genres=comic.metadata.genres,
+                        cover_path_rel=cover,
+                    ),
+                    [comicon.Chapter(chap.title, chap.slug)],
+                )
+                for chap in comic.chapters
+            ]
 
-        # save comicon.json
-        (comic_path / comicon.cirtools.IR_DATA_FILE).write_text(comicon_comic.to_json())
+            yield len(comicon_comics)
+            existing_filenames = {
+                file.name for file in dest_folder.iterdir() if file.is_file()
+            }
+            for comicomic in comicon_comics:
+                yield comicomic.metadata.title
+
+                # do not overwrite existing cache
+                if f"{comicomic.metadata.title}.{to.value}" in existing_filenames:
+                    continue
+                for _ in convert_one(comicomic, comic_path, to, dest_folder):
+                    ...
+
+        else:
+            comicon_comic = comicon.Comic(
+                comicon.Metadata(
+                    title=comic.metadata.title,
+                    authors=comic.metadata.authors,
+                    description=comic.metadata.description,
+                    genres=comic.metadata.genres,
+                    cover_path_rel=cover,
+                ),
+                [comicon.Chapter(chap.title, chap.slug) for chap in comic.chapters],
+            )
+
+            yield from convert_one(comicon_comic, comic_path, to, dest_folder)
 
-        # now we have a properly formed CIR
-        yield from comicon.outputs.create_comic_progress(
-            comic_path, dest_folder / f"{comic.metadata.title}.{to.value}"
-        )
     else:
         # it's a file, no conversion needed, let comicon do its inferencing
         yield from comicon.convert_progress(
             comic_path, dest_folder / f"{comic_path.stem}.{to.value}"
         )
 
     if remove_after:
```

### Comparing `mandown-1.3.4/mandown/base.py` & `mandown-1.4.0/mandown/base.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/cli.py` & `mandown-1.4.0/mandown/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,52 +151,58 @@
 
 
 def cli_convert(
     comic_path: Path,
     target_format: ConvertFormats,
     dest_folder: Path = Path.cwd(),
     remove_after: bool = False,
+    split_by_chapters: bool = False,
 ) -> None:
     iterator = api.convert_progress(
-        comic_path, target_format, dest_folder, remove_after
+        comic_path, target_format, dest_folder, remove_after, split_by_chapters
     )
 
     is_single_conversion = comic_path.is_dir()
 
     len_first_conv = cast(int, next(iterator))
     len_second_conv = -1
 
     first_convert_message = (
-        f"Packing {target_format.value}"
+        f"Packing {target_format.value}(s)"
         if is_single_conversion
         else "Pre-converting comic"
     )
 
     with typer.progressbar(
         iterator,
         length=len_first_conv,
         label=first_convert_message,
     ) as progress:
         for res in progress:
             if isinstance(res, int):
                 len_second_conv = res
                 break
+            if split_by_chapters:
+                progress.label = res
 
     if not is_single_conversion:
         # it *should* be guaranteed len_second_conv exists
         with typer.progressbar(
             iterator,
             length=len_second_conv,
             label=f"Packing {target_format.value}",
         ) as progress:
             for _ in progress:
                 ...
 
-    dest_file = dest_folder / f"{comic_path.stem}.{target_format.value}"
-    typer.secho(f"Successfully converted to {dest_file}", fg=typer.colors.GREEN)
+    if not split_by_chapters:
+        dest_file = dest_folder / f"{comic_path.stem}.{target_format.value}"
+        typer.secho(f"Successfully converted to {dest_file}", fg=typer.colors.GREEN)
+    else:
+        typer.secho(f"Successfully converted to {dest_folder}", fg=typer.colors.GREEN)
 
 
 def cli_process(
     comic_path: Path, options: list[ProcessOps], config: ProcessConfig
 ) -> None:
     if ProcessOps.NO_POSTPROCESSING in options:
         return
@@ -238,26 +244,33 @@
     ),
     remove_after: bool = typer.Option(
         False,
         "--remove-after",
         "-r",
         help="Remove the the original folder after conversion",
     ),
+    split_by_chapters: bool = typer.Option(
+        False,
+        "--split-by-chapters",
+        "-b",
+        help="Instead of returning one large comic file, create one comic"
+        "file for each chapter (applies only to Mandown-created comic folders)",
+    ),
 ) -> None:
     """
     Convert a comic OR comic folder into CBZ/EPUB/PDF.
 
     eg. To convert to CBZ:
     mandown convert cbz /path/to/comic/folder
 
     eg. To convert an existing PDF comic to EPUB:
     mandown convert epub /path/to/comic.pdf
     """
     typer.echo(f"Converting to {convert_to}...")
-    cli_convert(folder_path, convert_to, dest, remove_after)
+    cli_convert(folder_path, convert_to, dest, remove_after, split_by_chapters)
 
 
 @app.command(no_args_is_help=True)
 def process(
     options: list[ProcessOps],
     folder_path: Path = typer.Argument(Path.cwd()),
     target_size: Optional[tuple[int, int]] = typer.Option(
@@ -350,14 +363,21 @@
     ),
     remove_after: bool = typer.Option(
         False,
         "--remove-after",
         "-r",
         help="IF CONVERTING: Remove the downloaded folder after converting",
     ),
+    split_by_chapters: bool = typer.Option(
+        False,
+        "--split-by-chapters",
+        "-b",
+        help="Instead of returning one large comic file, create one comic"
+        "file for each chapter (applies only to Mandown-created comic folders)",
+    ),
 ) -> None:
     """
     Download from a URL chapters start_chapter to end_chapter.
     Defaults to the first chapter and last chapter, respectively
     in the working directory.
 
     eg. To download all chapters of a comic to the current directory:
@@ -425,15 +445,21 @@
             )
             raise typer.Exit(1) from err
 
         cli_process(dest / comic.metadata.title, processing_options, config)
 
     # convert
     if convert_to != ConvertFormats.NONE:
-        cli_convert(dest / comic.metadata.title, convert_to, dest, remove_after)
+        cli_convert(
+            dest / comic.metadata.title,
+            convert_to,
+            dest,
+            remove_after,
+            split_by_chapters,
+        )
 
 
 @app.command(name="init-metadata")
 def init_metadata(
     path: Optional[Path] = typer.Argument(None, help="The folder to initialise"),
     source_url: Optional[str] = typer.Argument(
         None, help="The url to get metadata from"
```

### Comparing `mandown-1.3.4/mandown/comic.py` & `mandown-1.4.0/mandown/comic.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/io.py` & `mandown-1.4.0/mandown/io.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/processor/__init__.py` & `mandown-1.4.0/mandown/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/processor/ops.py` & `mandown-1.4.0/mandown/processor/ops.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/processor/profiles.py` & `mandown-1.4.0/mandown/processor/profiles.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/sources/__init__.py` & `mandown-1.4.0/mandown/sources/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import types
 
 from . import (
     source_mangadex,
     source_mangakakalot,
     source_manganato,
     source_mangasee,
+    source_manhuaes,
     source_readcomiconline,
     source_webtoons,
 )
 from .base_source import BaseSource
 
 __class_list: list[type[BaseSource]] = []
```

### Comparing `mandown-1.3.4/mandown/sources/base_source.py` & `mandown-1.4.0/mandown/sources/base_source.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/sources/source_mangadex.py` & `mandown-1.4.0/mandown/sources/source_mangadex.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/sources/source_mangakakalot.py` & `mandown-1.4.0/mandown/sources/source_mangakakalot.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             BaseChapter(c.next_element, c["href"])
             for c in soup.select(".row > span > a")
         ]
         chapters.reverse()
         return chapters
 
     def fetch_chapter_image_list(self, chapter: BaseChapter) -> list[str]:
-        soup = BeautifulSoup(requests.get(chapter.url).text)
+        soup = BeautifulSoup(requests.get(chapter.url).text, "lxml")
         images = []
         for i in soup.select(".container-chapter-reader > img"):
             images.append(i["src"])
         return images
 
     def _get_scripts(self) -> str:
         if self._scripts:
```

### Comparing `mandown-1.3.4/mandown/sources/source_manganato.py` & `mandown-1.4.0/mandown/sources/source_manganato.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/sources/source_mangasee.py` & `mandown-1.4.0/mandown/sources/source_mangasee.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/sources/source_readcomiconline.py` & `mandown-1.4.0/mandown/sources/source_readcomiconline.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self, url: str) -> None:
         super().__init__(url)
         self.id = self.url_to_id(url)
 
     def fetch_metadata(self) -> BaseMetadata:
         soup = BeautifulSoup(
             requests.get(f"https://readcomiconline.li/Comic/{self.id}").text,
-            features="lxml",
+            "lxml",
         )
 
         title = str(soup.select_one("h3").text)
         author = [
             str(
                 # this site uses "Various" if there's more than one author
                 soup.select_one("a[href^='/Writer']").text
@@ -46,15 +46,15 @@
         cover = self.domains[0] + str(soup.find("link")["href"])
 
         return BaseMetadata(title, author, self.url, genres, description, cover)
 
     def fetch_chapter_list(self) -> list[BaseChapter]:
         soup = BeautifulSoup(
             requests.get(f"https://readcomiconline.li/Comic/{self.id}").text,
-            features="lxml",
+            "lxml",
         )
 
         chapters: list[BaseChapter] = []
         for e in soup.select("ul.list > li > a"):
             chapters.append(
                 BaseChapter(next(e.children).text, self.domains[0] + e["href"])
             )
```

### Comparing `mandown-1.3.4/mandown/sources/source_webtoons.py` & `mandown-1.4.0/mandown/sources/source_webtoons.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/ui/form.ui` & `mandown-1.4.0/mandown/ui/form.ui`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/ui/mainwin.py` & `mandown-1.4.0/mandown/ui/mainwin.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/mandown/ui/ui.py` & `mandown-1.4.0/mandown/ui/ui.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.4/pyproject.toml` & `mandown-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mandown"
-version = "1.3.4"
+version = "1.4.0"
 description = "Comic/manga/webtoon downloader and CBZ/EPUB/PDF converter"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/potatoeggy/mandown"
 documentation = "https://github.com/potatoeggy/mandown"
 keywords = ["manga", "comic", "downloader", "download", "webtoons", "webtoon"]
@@ -12,37 +12,36 @@
 [tool.poetry.scripts]
 mandown = "mandown.cli:main"
 mandown-gui = "mandown.ui.ui:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 typer = "^0.7.0"
-feedparser = "^6.0.8"
-beautifulsoup4 = "^4.10.0"
-requests = "^2.27.0"
-lxml = "^4.7.1"
-Pillow = "^9.0.1"
-python-slugify = "^6.1.2"
+feedparser = "^6.0.10"
+beautifulsoup4 = "^4.12.2"
+requests = "^2.31.0"
+lxml = "^4.9.2"
+Pillow = "^9.5.0"
+python-slugify = "^8.0.1"
 PySide6 = {version = "^6.4.0", optional = true}
 natsort = "^8.1.0"
-filetype = "^1.1.0"
-comicon = "^0.2.3"
+filetype = "^1.2.0"
+comicon = "^0.2.4"
 
-[tool.poetry.dev-dependencies]
-types-requests = "^2.26.3"
-types-lxml = "^2022.4.10"
-pytest = "^7.2.0"
+[tool.poetry.group.dev.dependencies]
+types-requests = "^2.31.0.1"
+types-lxml = "^2023.3.28"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.extras]
 gui = ["PySide6"]
 
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = ["B", "C", "E", "F", "W"]
 ignore = ["B905"]
```

### Comparing `mandown-1.3.4/PKG-INFO` & `mandown-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: mandown
-Version: 1.3.4
+Version: 1.4.0
 Summary: Comic/manga/webtoon downloader and CBZ/EPUB/PDF converter
 Home-page: https://github.com/potatoeggy/mandown
 License: AGPL-3.0-only
 Keywords: manga,comic,downloader,download,webtoons,webtoon
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
-Requires-Dist: Pillow (>=9.0.1,<10.0.0)
+Requires-Dist: Pillow (>=9.5.0,<10.0.0)
 Requires-Dist: PySide6 (>=6.4.0,<7.0.0) ; extra == "gui"
-Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
-Requires-Dist: comicon (>=0.2.3,<0.3.0)
-Requires-Dist: feedparser (>=6.0.8,<7.0.0)
-Requires-Dist: filetype (>=1.1.0,<2.0.0)
-Requires-Dist: lxml (>=4.7.1,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: comicon (>=0.2.4,<0.3.0)
+Requires-Dist: feedparser (>=6.0.10,<7.0.0)
+Requires-Dist: filetype (>=1.2.0,<2.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: natsort (>=8.1.0,<9.0.0)
-Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
-Requires-Dist: requests (>=2.27.0,<3.0.0)
+Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://github.com/potatoeggy/mandown
 Project-URL: Repository, https://github.com/potatoeggy/mandown
 Description-Content-Type: text/markdown
 
 # mandown
 
@@ -49,25 +49,14 @@
   - Rotate or split double-page spreads
   - Trim borders
   - Resize images
 - Convert downloaded comics to CBZ, EPUB, or PDF
   - Convert any other CBZ, EPUB, or PDF comic to CBZ, EPUB, or PDF
 - [A library to easily do all of this from other Python scripts](#basic-library-usage)
 
-## Supported sites
-
-To request a new site, please file a [new issue](https://github.com/potatoeggy/mandown/issues/new?title=Source%20request:).
-
-- <https://mangasee123.com>
-- <https://manganato.com>
-- <https://webtoons.com>
-- <https://mangadex.org>
-- <https://mangakakalot.com>
-- <https://readcomiconline.li>
-
 ## Usage
 
 Run `mandown --help` or see the [docs](/docs/) for more information and examples.
 
 ```
 mandown get <URL>
 ```
@@ -76,15 +65,15 @@
 
 ```
 mandown get <URL> --convert epub --process rotate_double_pages
 ```
 
 To download only a certain range of chapters, append the `--start` and/or `--end` options.
 
-> **Note:** `--start` and `--end` are *inclusive*, i.e., using `--start 2 --end 3` will download chapters 2 and 3.
+> **Note:** `--start` and `--end` are _inclusive_, i.e., using `--start 2 --end 3` will download chapters 2 and 3.
 
 To convert an existing folder or comic file without downloading anything (like a stripped-down version of <https://github.com/ciromattia/kcc>), use the `convert` command.
 
 ```
 mandown convert <FORMAT> <PATH_TO_COMIC>
 ```
 
@@ -124,14 +113,27 @@
 
 ```
 git clone https://github.com/potatoeggy/mandown.git
 poetry install
 poetry build
 pip3 install dist/mandown*.whl
 ```
+
+## Supported sites
+
+To request a new site, please file a [new issue](https://github.com/potatoeggy/mandown/issues/new?title=Source%20request:).
+
+- <https://mangasee123.com>
+- <https://manganato.com>
+- <https://webtoons.com>
+- <https://mangadex.org>
+- <https://mangakakalot.com>
+- <https://manhuaes.com>
+- <https://readcomiconline.li>
+
 ## Basic library usage
 
 See the [docs](/docs/) for more information and examples.
 
 To just download the images:
 
 ```python
```

