# Comparing `tmp/pretext-1.6.1.dev20230620.tar.gz` & `tmp/pretext-1.6.1.dev20230621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230620.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230621.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230620.tar` & `pretext-1.6.1.dev20230621.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-20 06:19:34.436590 pretext-1.6.1.dev20230620/LICENSE
--rw-r--r--   0        0        0     9757 2023-06-20 06:19:34.436590 pretext-1.6.1.dev20230620/README.md
--rw-r--r--   0        0        0     1901 2023-06-20 06:20:15.196987 pretext-1.6.1.dev20230620/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/__main__.py
--rw-r--r--   0        0        0     8170 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/build.py
--rw-r--r--   0        0        0    25351 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-20 06:20:20.401038 pretext-1.6.1.dev20230620/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/core/resources.py
--rw-r--r--   0        0        0  1035425 2023-06-20 06:20:20.397037 pretext-1.6.1.dev20230620/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/generate.py
--rw-r--r--   0        0        0    27475 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/project.py
--rw-r--r--   0        0        0      516 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-20 06:20:20.477038 pretext-1.6.1.dev20230620/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-20 06:20:20.477038 pretext-1.6.1.dev20230620/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160064 2023-06-20 06:20:20.473038 pretext-1.6.1.dev20230620/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7570 2023-06-20 06:20:20.445038 pretext-1.6.1.dev20230620/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173263 2023-06-20 06:20:20.465038 pretext-1.6.1.dev20230620/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-06-20 06:20:20.477038 pretext-1.6.1.dev20230620/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4611 2023-06-20 06:20:20.445038 pretext-1.6.1.dev20230620/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-20 06:20:20.477038 pretext-1.6.1.dev20230620/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-20 06:20:20.477038 pretext-1.6.1.dev20230620/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8346 2023-06-20 06:20:20.477038 pretext-1.6.1.dev20230620/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18416 2023-06-20 06:19:34.440590 pretext-1.6.1.dev20230620/pretext/utils.py
--rw-r--r--   0        0        0     1143 2023-06-20 06:20:15.196987 pretext-1.6.1.dev20230620/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230620/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/LICENSE
+-rw-r--r--   0        0        0     9757 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/README.md
+-rw-r--r--   0        0        0     1909 2023-06-21 06:19:56.017106 pretext-1.6.1.dev20230621/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/build.py
+-rw-r--r--   0        0        0    25561 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-06-21 06:20:01.109121 pretext-1.6.1.dev20230621/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/core/resources.py
+-rw-r--r--   0        0        0  1035425 2023-06-21 06:20:01.109121 pretext-1.6.1.dev20230621/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16766 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/generate.py
+-rw-r--r--   0        0        0    31778 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/project.py
+-rw-r--r--   0        0        0      555 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-21 06:20:01.177121 pretext-1.6.1.dev20230621/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-21 06:20:01.177121 pretext-1.6.1.dev20230621/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160110 2023-06-21 06:20:01.173121 pretext-1.6.1.dev20230621/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7616 2023-06-21 06:20:01.145121 pretext-1.6.1.dev20230621/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173309 2023-06-21 06:20:01.165121 pretext-1.6.1.dev20230621/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2192 2023-06-21 06:20:01.177121 pretext-1.6.1.dev20230621/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4657 2023-06-21 06:20:01.149121 pretext-1.6.1.dev20230621/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-21 06:20:01.177121 pretext-1.6.1.dev20230621/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-21 06:20:01.177121 pretext-1.6.1.dev20230621/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8392 2023-06-21 06:20:01.177121 pretext-1.6.1.dev20230621/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    19529 2023-06-21 06:19:26.334217 pretext-1.6.1.dev20230621/pretext/utils.py
+-rw-r--r--   0        0        0     3093 2023-06-21 06:19:56.021106 pretext-1.6.1.dev20230621/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230621/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230620/LICENSE` & `pretext-1.6.1.dev20230621/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230620/README.md` & `pretext-1.6.1.dev20230621/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230620/pretext/__init__.py` & `pretext-1.6.1.dev20230621/pretext/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "interactive",
     "youtube",
     "codelens",
     "datafile",
 ]
 
 
-def activate():
+def activate() -> None:
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
     to help anyone who might have upgraded from the original package.
     """
     raise RuntimeError(
```

### Comparing `pretext-1.6.1.dev20230620/pretext/build.py` & `pretext-1.6.1.dev20230621/pretext/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 import os
 from pathlib import Path
 import sys
-from typing import Optional
+from typing import Dict, Optional
 
 from . import utils, core, codechat
 
 # Get access to logger
 log = logging.getLogger("ptxlogger")
 
 
 def html(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
-    stringparams,
+    stringparams: Dict[str, str],
     custom_xsl: Optional[Path],
-    xmlid_root,
-    zipped=False,
-):
+    xmlid_root: Optional[str],
+    zipped: bool = False,
+) -> None:
     os.makedirs(output, exist_ok=True)
     log.info(f"\nNow building HTML into {output}\n")
     if xmlid_root is not None:
         log.info(f"Only building @xml:id `{xmlid_root}`\n")
     if zipped:
         file_format = "zip"
     else:
@@ -36,31 +36,31 @@
                 stringparams,
                 xmlid_root,
                 file_format,
                 custom_xsl and custom_xsl.as_posix(),  # pass None or posix string
                 None,
                 output.as_posix(),
             )
-            codechat.map_path_to_xml_id(
-                ptxfile, utils.project_path(ptxfile), output.as_posix()
-            )
+            pp = utils.project_path(ptxfile)
+            assert pp is not None, f"Invalid project path to {ptxfile}."
+            codechat.map_path_to_xml_id(ptxfile, pp, output.as_posix())
         except Exception as e:
             log.critical(e)
             log.debug("Exception info:\n##################\n", exc_info=True)
             log.info("##################")
             sys.exit("Failed to build html.  Exiting...")
 
 
 def latex(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
-    stringparams,
+    stringparams: Dict[str, str],
     custom_xsl: Optional[Path],
-):
+) -> None:
     os.makedirs(output, exist_ok=True)
     log.info(f"\nNow building LaTeX into {output}\n")
     # ensure working directory is preserved
     with utils.working_directory(Path()):
         try:
             core.latex(
                 ptxfile,
@@ -77,18 +77,18 @@
             sys.exit("Failed to build latex.  Exiting...")
 
 
 def pdf(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
-    stringparams,
+    stringparams: Dict[str, str],
     custom_xsl: Optional[Path],
     pdf_method: str,
-):
+) -> None:
     os.makedirs(output, exist_ok=True)
     log.info(f"\nNow building LaTeX into {output}\n")
     # ensure working directory is preserved
     with utils.working_directory(Path()):
         try:
             core.pdf(
                 ptxfile,
@@ -106,18 +106,18 @@
             sys.exit("Failed to build pdf.  Exiting...")
 
 
 def custom(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
-    stringparams,
+    stringparams: Dict[str, str],
     custom_xsl: Path,
     output_filename: Optional[str] = None,
-):
+) -> None:
     os.makedirs(output, exist_ok=True)
     if output_filename is not None:
         output_filepath = output / output_filename
         output_dir = None
         log.info(f"\nNow building with custom {custom_xsl} into {output_filepath}\n")
     else:
         output_filepath = None
@@ -137,25 +137,27 @@
             log.critical(e)
             log.debug("Exception info:\n##################\n", exc_info=True)
             log.info("##################")
             sys.exit("Failed custom build.  Exiting...")
 
 
 # build (non Kindle) ePub:
-def epub(ptxfile, pub_file: Path, output: Path, stringparams):
+def epub(
+    ptxfile: Path, pub_file: Path, output: Path, stringparams: Dict[str, str]
+) -> None:
     os.makedirs(output, exist_ok=True)
     try:
         utils.npm_install()
     except Exception as e:
         log.debug(e)
         sys.exit(
             "Unable to build epub because node packages are not installed.  Exiting..."
         )
     log.info(f"\nNow building ePub into {output}\n")
-    with utils.working_directory("."):
+    with utils.working_directory(Path()):
         try:
             core.epub(
                 ptxfile,
                 pub_file.as_posix(),
                 out_file=None,  # will be derived from source
                 dest_dir=output.as_posix(),
                 math_format="svg",
@@ -165,25 +167,27 @@
             log.critical(e)
             log.debug("Exception info:\n##################\n", exc_info=True)
             log.info("##################")
             sys.exit("Failed to build epub.  Exiting...")
 
 
 # build Kindle ePub:
-def kindle(ptxfile, pub_file: Path, output: Path, stringparams):
+def kindle(
+    ptxfile: Path, pub_file: Path, output: Path, stringparams: Dict[str, str]
+) -> None:
     os.makedirs(output, exist_ok=True)
     try:
         utils.npm_install()
     except Exception as e:
         log.critical(e)
         sys.exit(
             "Unable to build Kindle ePub because node packages are not installed.  Exiting..."
         )
     log.info(f"\nNow building Kindle ePub into {output}\n")
-    with utils.working_directory("."):
+    with utils.working_directory(Path()):
         try:
             core.epub(
                 ptxfile,
                 pub_file.as_posix(),
                 out_file=None,  # will be derived from source
                 dest_dir=output.as_posix(),
                 math_format="kindle",
@@ -193,28 +197,34 @@
             log.critical(e)
             log.debug("Exception info:\n##################\n", exc_info=True)
             log.info("##################")
             sys.exit("Failed to build kindle ebook.  Exiting...")
 
 
 # build Braille:
-def braille(ptxfile, pub_file: Path, output: Path, stringparams, page_format="emboss"):
+def braille(
+    ptxfile: Path,
+    pub_file: Path,
+    output: Path,
+    stringparams: Dict[str, str],
+    page_format: str = "emboss",
+) -> None:
     os.makedirs(output, exist_ok=True)
     log.warning(
         "Braille output is still experimental, and requires additional libraries from liblouis (specifically the file2brl software)."
     )
     try:
         utils.npm_install()
     except Exception as e:
         log.debug(e)
         sys.exit(
             "Unable to build braille because node packages could not be installed.  Exiting..."
         )
     log.info(f"\nNow building braille into {output}\n")
-    with utils.working_directory("."):
+    with utils.working_directory(Path()):
         try:
             core.braille(
                 xml_source=ptxfile,
                 pub_file=pub_file.as_posix(),
                 out_file=None,  # will be derived from source
                 dest_dir=output.as_posix(),
                 page_format=page_format,  # could be "eboss" or "electronic"
@@ -228,17 +238,17 @@
 
 
 # Build WeBWorK sets (for archive)
 def webwork_sets(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
-    stringparams,
-    zipped=False,
-):
+    stringparams: Dict[str, str],
+    zipped: bool = False,
+) -> None:
     os.makedirs(output, exist_ok=True)
     log.info(f"\nNow building WeBWorK Sets into {output}\n")
     # ensure working directory is preserved
     with utils.working_directory(Path()):
         try:
             core.webwork_sets(
                 xml_source=ptxfile,
```

### Comparing `pretext-1.6.1.dev20230620/pretext/cli.py` & `pretext-1.6.1.dev20230621/pretext/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import os
 import zipfile
 import requests
 import io
 import tempfile
 import platform
 from pathlib import Path
-import typing as t
 import atexit
 import subprocess
+from typing import List, Optional, Tuple
 from .config import xml_overlay
 
 from . import (
     utils,
     templates,
     core,
     VERSION,
@@ -58,43 +58,43 @@
 @click.version_option(VERSION, message=VERSION)
 @click.option(
     "-t",
     "--targets",
     is_flag=True,
     help='Display list of build/view "targets" available in the project manifest.',
 )
-def main(ctx, targets):
+def main(ctx: click.Context, targets: bool) -> None:
     """
     Command line tools for quickly creating, authoring, and building PreTeXt projects.
 
     PreTeXt Guide for authors and publishers:
 
     - https://pretextbook.org/documentation.html
 
     PreTeXt CLI README for developers:
 
     - https://github.com/PreTeXtBook/pretext-cli/
 
     Use the `--help` option on any CLI command to learn more, for example,
     `pretext build --help`.
     """
-    if utils.project_path() is not None:
+    if (pp := utils.project_path()) is not None:
         if targets:
             Project().print_target_names()
             return
         # create file handler which logs even debug messages
-        fh = logging.FileHandler(utils.project_path() / "cli.log", mode="w")
+        fh = logging.FileHandler(pp / "cli.log", mode="w")
         fh.setLevel(logging.DEBUG)
         file_log_format = logging.Formatter("{levelname:<8}: {message}", style="{")
         fh.setFormatter(file_log_format)
         log.addHandler(fh)
         # output info
         log.info(f"PreTeXt project found in `{utils.project_path()}`.")
         # permanently change working directory for rest of process
-        os.chdir(utils.project_path())
+        os.chdir(pp)
         if utils.requirements_version() is None:
             log.warning(
                 "Project's CLI version could not be detected from `requirements.txt`."
             )
             log.warning("Try `pretext init --refresh` to produce a compatible file.")
         elif utils.requirements_version() != VERSION:
             log.warning(f"Using CLI version {VERSION} but project's `requirements.txt`")
@@ -115,15 +115,15 @@
 
 
 # pretext support
 @main.command(
     short_help="Use when communicating with PreTeXt support.",
     context_settings=CONTEXT_SETTINGS,
 )
-def support():
+def support() -> None:
     """
     Outputs useful information about your installation needed by
     PreTeXt volunteers when requesting help on the pretext-support
     Google Group.
     """
     log.info("")
     log.info("Please share the following information when posting to the")
@@ -156,20 +156,22 @@
 
 # pretext devscript
 @main.command(
     short_help="Alias for the developer pretext/pretext script.",
     context_settings={"help_option_names": [], "ignore_unknown_options": True},
 )
 @click.argument("args", nargs=-1)
-def devscript(args):
+def devscript(args: List[str]) -> None:
     """
     Aliases the core pretext script.
     """
     PY_CMD = sys.executable
-    subprocess.run([PY_CMD, core.resources.path("pretext", "pretext")] + list(args))
+    subprocess.run(
+        [PY_CMD, str(core.resources.path("pretext", "pretext"))] + list(args)
+    )
 
 
 # pretext new
 @main.command(
     short_help="Generates the necessary files for a new PreTeXt project.",
     context_settings=CONTEXT_SETTINGS,
 )
@@ -187,15 +189,15 @@
 )
 @click.option(
     "-u",
     "--url-template",
     type=click.STRING,
     help="Download a zipped template from its URL.",
 )
-def new(template, directory, url_template):
+def new(template: str, directory: Path, url_template: str) -> None:
     """
     Generates the necessary files for a new PreTeXt project.
     Supports `pretext new book` (default) and `pretext new article`,
     or generating from URL with `pretext new --url-template [URL]`.
     """
     directory_fullpath = Path(directory).resolve()
     if utils.project_path(directory_fullpath) is not None:
@@ -245,15 +247,15 @@
 )
 @click.option(
     "-r",
     "--refresh",
     is_flag=True,
     help="Refresh initialization of project even if project.ptx exists.",
 )
-def init(refresh):
+def init(refresh: bool) -> None:
     """
     Generates the project manifest for a PreTeXt project in the current directory. This feature
     is mainly intended for updating existing projects to use this CLI.
 
     If --refresh is used, files will be generated even if the project has already been initialized.
     Existing files won't be overwritten; a copy of the fresh initialized file will be created
     with a timestamp in its filename for comparison.
@@ -269,15 +271,15 @@
         "project.ptx": "project.ptx",
         "publication.ptx": "publication/publication.ptx",
         ".gitignore": ".gitignore",
         "devcontainer.json": ".devcontainer/devcontainer.json",
     }
     for resource in resource_to_dest:
         with templates.resource_path(resource) as resource_path:
-            project_resource_path = Path(resource_to_dest.get(resource)).resolve()
+            project_resource_path = Path(resource_to_dest[resource]).resolve()
             if project_resource_path.exists():
                 new_resource_name = (
                     project_resource_path.stem
                     + "-"
                     + timestamp
                     + project_resource_path.suffix
                 )
@@ -307,15 +309,15 @@
     log.info(
         "Edit your <target/>s to point to the location of your PreTeXt source files."
     )
 
 
 # pretext build
 @main.command(short_help="Build specified target", context_settings=CONTEXT_SETTINGS)
-@click.argument("target", required=False)
+@click.argument("target_name", required=False, metavar="target")
 @click.option(
     "--clean",
     is_flag=True,
     help="Destroy output's target directory before build to clean up previously built files",
 )
 @click.option(
     "-g",
@@ -340,21 +342,21 @@
     "-p",
     "--project-ptx-override",
     type=(str, str),
     multiple=True,
     help=xml_overlay.USAGE_DESCRIPTION.format("-p"),
 )
 def build(
-    target,
-    clean,
-    generate,
-    no_generate,
-    xmlid: t.Optional[str],
-    project_ptx_override: t.Tuple[str, str],
-):
+    target_name: str,
+    clean: bool,
+    generate: str,
+    no_generate: bool,
+    xmlid: Optional[str],
+    project_ptx_override: Tuple[Tuple[str, str], ...],
+) -> None:
     """
     Build [TARGET] according to settings specified by project.ptx.
 
     If using elements that require separate generation of assets (e.g., webwork, latex-image, etc.) then these will be generated automatically if their source has changed since the last build.  You can suppress this with the `--no-generate` flag, or force a regeneration with the `--generate` flag.
 
     Certain builds may require installations not included with the CLI, or internet
     access to external servers. Command-line paths
@@ -365,15 +367,14 @@
     # Add xmlid value to project_ptx_override (a tuple of tuples)
     if xmlid:
         project_ptx_override += (("targets.target.xmlid-root", xmlid),)
     overlay = xml_overlay.ShadowXmlDocument()
     for path, value in project_ptx_override:
         overlay.upsert_node_or_attribute(path, value)
 
-    target_name = target
     if utils.no_project(task="build"):
         return
     project = Project()
     if len(project_ptx_override) > 0:
         messages = project.apply_overlay(overlay)
         for message in messages:
             log.info("project.ptx overlay " + message)
@@ -449,14 +450,15 @@
 )
 @click.argument(
     "assets", default="ALL", type=click.Choice(ASSETS, case_sensitive=False)
 )
 @click.option(
     "-t",
     "--target",
+    "target_name",
     type=click.STRING,
     help="Name of target to generate assets for (if not specified, first target from manifest is used).",
 )
 @click.option(
     "-x", "--xmlid", type=click.STRING, help="xml:id of element to be generated."
 )
 @click.option(
@@ -470,19 +472,19 @@
     "--project-ptx-override",
     type=(str, str),
     multiple=True,
     help=xml_overlay.USAGE_DESCRIPTION.format("-p"),
 )
 def generate(
     assets: str,
-    target: t.Optional[str],
+    target_name: Optional[str],
     all_formats: bool,
-    xmlid: t.Optional[str],
-    project_ptx_override: t.Tuple[str, str],
-):
+    xmlid: Optional[str],
+    project_ptx_override: Tuple[Tuple[str, str], ...],
+) -> None:
     """
     Generate specified (or all) assets for the default target (first target in "project.ptx"). Asset "generation" is typically
     slower and performed less frequently than "building" a project, but is
     required for many PreTeXt features such as webwork and latex-image.
 
     Certain assets may require installations not included with the CLI, or internet
     access to external servers. Command-line paths
@@ -497,24 +499,23 @@
         overlay.upsert_node_or_attribute(path, value)
 
     project = Project()
     if len(project_ptx_override) > 0:
         messages = project.apply_overlay(overlay)
         for message in messages:
             log.info("project.ptx overlay " + message)
-    target_name = target
     target = project.target(name=target_name)
-    if target_name is None:
-        log.info(
-            f"Since no target was specified with the -t flag, we will generate assets for the first target in the manifest ({target.name()})."
-        )
     if target is None:
         utils.show_target_hints(target_name, project, task="generating assets for")
         log.critical("Exiting without generating any assets.")
         return
+    if target_name is None:
+        log.info(
+            f"Since no target was specified with the -t flag, we will generate assets for the first target in the manifest ({target.name()})."
+        )
     if all_formats and assets == "ALL":
         log.info(
             f'Generating all assets in all asset formats for the target "{target.name()}".'
         )
         project.generate(target.name(), all_formats=True, xmlid=xmlid)
     elif all_formats:
         log.info(
@@ -538,15 +539,15 @@
 # pretext view
 
 
 @main.command(
     short_help="Preview specified target based on its format.",
     context_settings=CONTEXT_SETTINGS,
 )
-@click.argument("target", required=False)
+@click.argument("target_name", metavar="target", required=False)
 @click.option(
     "-a",
     "--access",
     type=click.Choice(["public", "private"], case_sensitive=False),
     default="private",
     show_default=True,
     help="""
@@ -607,54 +608,53 @@
 )
 @click.option(
     "--no-launch",
     is_flag=True,
     help="By default, pretext view tries to launch the default application to view the specified target.  Setting this suppresses this behavior.",
 )
 def view(
-    target: str,
+    target_name: str,
     access: str,
-    port: t.Optional[int],
-    directory: str,
+    port: Optional[int],
+    directory: Optional[str],
     watch: bool,
     build: bool,
-    generate: t.Optional[str],
+    generate: Optional[str],
     no_launch: bool,
-):
+) -> None:
     """
     Starts a local server to preview built PreTeXt documents in your browser.
     TARGET is the name of the <target/> defined in `project.ptx`.
     """
     if directory is not None:
         if utils.cocalc_project_id() is not None:
             try:
-                subdir = directory.relative_to(Path.home())
+                subdir = Path(directory).relative_to(Path.home())
             except ValueError:
-                subdir = ""
+                subdir = Path()
             log.info("Directory can be previewed at the following link at any time:")
             log.info(f"    https://cocalc.com/{utils.cocalc_project_id()}/raw/{subdir}")
             return
         port = port or 8000
         utils.run_server(Path(directory), access, port, no_launch=no_launch)
         return
     if utils.no_project(task="view the output for"):
         return
-    target_name = target
     project = Project()
     target = project.target(name=target_name)
     if target is None:
         utils.show_target_hints(target_name, project, task="view")
         log.critical("Exiting.")
         return
     # Easter egg to spin up a local server at a specified directory:
     if utils.cocalc_project_id() is not None:
         try:
             subdir = target.output_dir().relative_to(Path.home())
         except ValueError:
-            subdir = ""
+            subdir = Path()
         log.info("Built project can be previewed at the following link at any time:")
         log.info(f"    https://cocalc.com/{utils.cocalc_project_id()}/raw/{subdir}")
         return
     port = port or target.port()
     if generate == "ALL":
         log.info("Generating all assets in default formats.")
         project.generate(target_name)
@@ -668,27 +668,26 @@
 
 
 # pretext deploy
 @main.command(
     short_help="Deploys Git-managed project to GitHub Pages.",
     context_settings=CONTEXT_SETTINGS,
 )
-@click.argument("target", required=False)
+@click.argument("target_name", metavar="target", required=False)
 @click.option("-u", "--update_source", is_flag=True, required=False)
-def deploy(target, update_source):
+def deploy(target_name: str, update_source: bool) -> None:
     """
     Automatically deploys most recent build of [TARGET] to GitHub Pages,
     making it available to the general public.
     Requires that your project is under Git version control
     properly configured with GitHub and GitHub Pages. Deployed
     files will live in `docs` subdirectory of project.
     """
     if utils.no_project(task="deploy"):
         return
-    target_name = target
     project = Project()
     target = project.target(name=target_name)
     if target is None or target.format() != "html":
         log.critical("Target could not be found in project.ptx manifest.")
         # only list targets with html format.
         log.critical(
             f"Possible html targets to deploy are: {project.target_names('html')}"
```

### Comparing `pretext-1.6.1.dev20230620/pretext/codechat.py` & `pretext-1.6.1.dev20230621/pretext/codechat.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # <http://www.python.org/dev/peps/pep-0008/#imports>`_.
 #
 # Standard library
 # ----------------
 import collections  # defaultdict
 import glob  # glob
 import json  # dumps
-import pathlib  # Path
+from pathlib import Path
 import sys  # platform
 import urllib.parse  # urlparse
 import urllib.request  # pathname2url
 
 # Third-party imports
 # -------------------
 # We assume a previous call to ``xsltproc`` has already verified that lxml is installed.
@@ -43,54 +43,56 @@
 #       # A list of XML IDs in this source file which produce HTML files.
 #       List[str]
 #   ]
 #
 # This allows a single source file to produce multiple HTML files, as well as supporting a one-to-one relationship. The list captures the order of appearance of the XML IDs in the tree -- element 0 is the first XML ID, etc.
 def map_path_to_xml_id(
     # A path to the root XML file in the pretext book being processed.
-    xml: str,
+    xml: Path,
     # A path to the project directory, which (should) contain ``codechat_config.yaml``.
-    project_path: pathlib.Path,
+    project_path: Path,
     # A path to the destination or output directory. The resulting JSON file will be stored there.
     dest_dir: str,
 ) -> None:
     # Make insertions easy by specifying that newly-created entries in ``path_to_xml_id`` contain an empty list.
     path_to_xml_id = collections.defaultdict(list)
 
     # Normalize path separators to current OS.
-    xml = str(pathlib.Path(xml).resolve())
+    _xml = str(xml.resolve())
 
     # This follows the `Python recommendations <https://docs.python.org/3/library/sys.html#sys.platform>`_.
     is_win = sys.platform == "win32"
 
     # Look at all HTML files in the output directory. Store only their stem, since this is what an XML ID specifies. Note that all output files will have the same path prefix (the ``dest_dir`` and the same suffix (``.html``); the stem is the only unique part.
     html_files = set(
-        pathlib.Path(html_file).stem for html_file in glob.glob(dest_dir + "/*.html")
+        Path(html_file).stem for html_file in glob.glob(dest_dir + "/*.html")
     )
 
     # lxml turns ``xml:id`` into the string below.
     xml_ns = "{http://www.w3.org/XML/1998/namespace}"
     xml_base_attrib = f"{xml_ns}base"
     xml_id_attrib = f"{xml_ns}id"
 
     # Define a loader which sets the ``xml:base`` of an xincluded element. While lxml `evidently used to do this in 2013 <https://stackoverflow.com/a/18158472/16038919>`_, a change eliminated this ability per some `dicussion <https://mail.gnome.org/archives/xml/2014-April/msg00015.html>`_, which included a rejected patch fixing this problem. `Current source <https://github.com/GNOME/libxml2/blob/master/xinclude.c#L1689>`_ lacks this patch.
-    def my_loader(href, parse, encoding=None, parser=None):
+    #
+    # Since there's few docs on this function, ignore the lack of types.
+    def my_loader(href, parse, encoding=None, parser=None):  # type: ignore
         ret = lxml.ElementInclude._lxml_default_loader(href, parse, encoding, parser)
         # The return value may not be an element.
         if isinstance(ret, ET._Element):
             ret.attrib[xml_base_attrib] = href
         return ret
 
     # Load the XML, performing xincludes using this loader.
     huge_parser = ET.XMLParser(huge_tree=True)
-    src_tree = ET.parse(xml, parser=huge_parser)
+    src_tree = ET.parse(_xml, parser=huge_parser)
     lxml.ElementInclude.include(src_tree, loader=my_loader)
 
-    # Walk though every element with an xml ID.
-    for elem in src_tree.iterfind(f"//*[@{xml_id_attrib}]"):
+    # Walk though every element with an xml ID. Note: the type stubs don't have the ``iterfind`` method, hence the ignore in the next line.
+    for elem in src_tree.iterfind(f"//*[@{xml_id_attrib}]"):  # type: ignore
         # Consider only elemets whose ID produced an HTML file. TODO: use a walrus operator after Python 3.7 is EOL.
         xml_id = elem.get(xml_id_attrib)
         if xml_id in html_files:
             # Store this discovered mapping between ID and output file.
             #
             # The `elem.base <https://lxml.de/api/lxml.etree._Element-class.html#base>`_ gives the URL of this file (which is correct due to the custom loader). Extract the path.
             up = urllib.parse.urlparse(elem.base)
@@ -99,15 +101,15 @@
             path = up.path
             # On Windows, this produces ``path == "/C:/path/to/file.ptx"``. Remove the slash.
             if is_win:
                 path = path[1:]
             # Decode the URL-encoded filename.
             path = urllib.parse.unquote(path)
             # Use ``resolve()`` to standardize capitalization on Windows.
-            stdpath = pathlib.Path(path).resolve()
+            stdpath = Path(path).resolve()
             # Make this path relative to the project directory, to avoid writing potentially confidential information (username / local filesystem paths) to the mapping file, which might be published to the web.
             relpath = stdpath.relative_to(project_path)
             # Add this XML ID to others for this path.
             path_to_xml_id[str(relpath)].append(xml_id)
 
     # Save the result as a JSON file in the ``dest_dir``.
-    (pathlib.Path(dest_dir) / ".mapping.json").write_text(json.dumps(path_to_xml_id))
+    (Path(dest_dir) / ".mapping.json").write_text(json.dumps(path_to_xml_id))
```

### Comparing `pretext-1.6.1.dev20230620/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230621/pretext/config/xml_overlay.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,24 +24,35 @@
     value: t.Union[str, None]
     attributes: t.List[t.Tuple[str, str]]
 
 
 class XmlOverlayType(click.ParamType):
     name = "xml_overlay"
 
-    def convert(self, value, param, ctx):
-        print("got", value, param, ctx.args, ctx.obj)
+    def convert(
+        self,
+        value: t.Any,
+        param: t.Optional[click.Parameter],
+        ctx: t.Optional[click.Context],
+    ) -> t.Any:
+        print(
+            "got",
+            value,
+            param,
+            None if ctx is None else ctx.args,
+            None if ctx is None else ctx.obj,
+        )
         return value
 
 
 class ShadowXmlDocument:
-    def __init__(self):
+    def __init__(self) -> None:
         self._nodes_dict: t.Dict[str, ShadowXmlNodeType] = {}
 
-    def upsert_node_or_attribute(self, path: str, value: t.Union[str, None]):
+    def upsert_node_or_attribute(self, path: str, value: str) -> "ShadowXmlDocument":
         """
         Upserts a node into the shadow document.
 
         @path - A string representing the path of the node/attribute. For example, `a.b.c` would be nested `<a><b><c>...` nodes.
                 `a.b@c` would be an attribute named `c` on the `b` node. E.g. `<a><b c="...">...`
         @value - The (string) value of the node/attribute.
         """
@@ -64,29 +75,29 @@
             node = self._nodes_dict.get(
                 path, {"name": None, "value": None, "attributes": []}
             )
             node["value"] = value
             self._nodes_dict[path] = node
         return self
 
-    def overlay_tree(self, root: ET.Element = ET.Element("root")) -> t.List[str]:
+    def overlay_tree(self, root: ET._Element = ET.Element("root")) -> t.List[str]:
         """
         Overlay `root` with the current ShadowXmlDocument's nodes and attributes.
         A list of string messages are returned about what elements were changed.
 
         This function mutates `root`.
         """
 
         ret: t.List[str] = []
 
         def upsert_node(
             path: t.List[str],
-            current: ET.Element = root,
+            current: ET._Element = root,
             current_path: t.List[str] = [],
-        ) -> t.List[ET.Element]:
+        ) -> t.List[ET._Element]:
             if len(path) == 0:
                 return [current]
             needed_tag = path[0]
             path = path[1:]
             current_path = [*current_path, needed_tag]
 
             # Find all matching tags. If none are found, we create one.
```

### Comparing `pretext-1.6.1.dev20230620/pretext/core/pretext.py` & `pretext-1.6.1.dev20230621/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230620/pretext/core/resources.py` & `pretext-1.6.1.dev20230621/pretext/core/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 import zipfile
 import importlib.resources
 from .. import CORE_COMMIT
 
 
-def path(*args) -> Path:
+def path(*args: str) -> Path:
     # Checks that the local static path ~/.ptx/ contains the static files needed for core, and installs them if they are missing (or if the version is different from the installed version of pretext).  Then returns the absolute path to the static files (appending arguments)
     local_base_path = Path.home() / ".ptx"
     local_commit_file = Path(local_base_path) / ".commit"
     if not Path.is_file(local_commit_file):
         print("Static pretext files do not appear to be installed.  Installing now.")
         install(local_base_path)
     # check that the static core_commit matches current core_commit
@@ -16,15 +16,15 @@
         static_commit = f.readline().strip()
     if static_commit != CORE_COMMIT:
         print("Static pretext files are out of date.  Installing them now.")
         install(local_base_path)
     return local_base_path.joinpath(*args)
 
 
-def install(local_base_path):
+def install(local_base_path: Path) -> None:
     with importlib.resources.path("pretext.core", "resources.zip") as static_zip:
         with zipfile.ZipFile(static_zip, "r") as zip:
             zip.extractall(local_base_path)
     # Write the current commit to local file
     with open(local_base_path / ".commit", "w") as f:
         f.write(CORE_COMMIT)
     print(
```

### Comparing `pretext-1.6.1.dev20230620/pretext/core/resources.zip` & `pretext-1.6.1.dev20230621/pretext/core/resources.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,143 +1,143 @@
 Zip file size: 1035425 bytes, number of entries: 141
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 xsl/
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-20 06:20 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-20 06:20 css/colors_green_plum.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-20 06:20 css/setcolors.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-20 06:20 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-20 06:20 css/mathbook-3.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-20 06:20 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-20 06:20 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-20 06:20 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-20 06:20 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-20 06:20 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-20 06:20 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-20 06:20 css/README.md
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-20 06:20 css/colors_red_blue.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-20 06:20 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-20 06:20 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-20 06:20 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-20 06:20 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-20 06:20 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-20 06:20 css/pretext_add_on.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-20 06:20 css/update_css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-20 06:20 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-20 06:20 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-20 06:20 css/style_default.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-20 06:20 css/mathbook-content.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-20 06:20 css/kindle.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-20 06:20 css/style_soundwriting.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-20 06:20 css/pretext.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-20 06:20 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-20 06:20 css/colors_martiansands.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-20 06:20 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx   109017 b- defN 23-Jun-20 06:20 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-20 06:20 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-20 06:20 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jun-20 06:20 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-20 06:20 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-20 06:20 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx   231248 b- defN 23-Jun-20 06:20 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   612399 b- defN 23-Jun-20 06:20 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-20 06:20 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-20 06:20 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-20 06:20 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-20 06:20 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-20 06:20 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-20 06:20 xsl/README.md
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-20 06:20 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-20 06:20 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-20 06:20 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-20 06:20 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-20 06:20 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-20 06:20 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-20 06:20 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-20 06:20 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-20 06:20 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-20 06:20 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-20 06:20 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-20 06:20 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-20 06:20 xsl/entities.ent
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-20 06:20 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-20 06:20 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-20 06:20 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-20 06:20 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-20 06:20 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-20 06:20 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-20 06:20 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-20 06:20 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-20 06:20 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-20 06:20 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-20 06:20 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-20 06:20 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-20 06:20 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-20 06:20 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-20 06:20 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-20 06:20 xsl/utilities/README.md
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-20 06:20 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-20 06:20 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-20 06:20 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-20 06:20 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-20 06:20 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-20 06:20 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-20 06:20 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-20 06:20 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-20 06:20 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-20 06:20 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-Jun-20 06:20 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-20 06:20 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-Jun-20 06:20 xsl/localizations/README.md
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-20 06:20 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-20 06:20 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-Jun-20 06:20 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-20 06:20 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-20 06:20 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-20 06:20 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-20 06:20 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-20 06:20 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-20 06:20 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-20 06:20 xsl/localizations/en-US.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 xsl/support/play-button/
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-20 06:20 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-20 06:20 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-20 06:20 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-20 06:20 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-20 06:20 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-20 06:20 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-20 06:20 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-20 06:20 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-20 06:20 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-20 06:20 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 06:20 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-20 06:20 pretext/module-test.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-20 06:20 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-20 06:20 pretext/README.md
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-20 06:20 pretext/pretext
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-20 06:20 pretext/pretext.py
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-20 06:20 pretext/braille_format.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-20 06:20 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-20 06:20 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-20 06:20 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-20 06:20 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-20 06:20 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 06:20 script/mjsre/update-sre
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-20 06:20 schema/pretext.xsd
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-20 06:20 schema/pretext.rng
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-20 06:20 schema/pretext.xml
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-20 06:20 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-20 06:20 schema/pretext.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-20 06:20 schema/README.md
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-20 06:20 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-20 06:20 schema/xml.xsd
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-20 06:20 schema/build.sh
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-20 06:20 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-20 06:20 schema/pretext-dev.rng
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 xsl/
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-21 06:20 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-21 06:20 css/colors_green_plum.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-21 06:20 css/setcolors.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-21 06:20 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-21 06:20 css/mathbook-3.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-21 06:20 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-21 06:20 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-21 06:20 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-21 06:20 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-21 06:20 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-21 06:20 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-21 06:20 css/README.md
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-21 06:20 css/colors_red_blue.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-21 06:20 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-21 06:20 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-21 06:20 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-21 06:20 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-21 06:20 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-21 06:20 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-21 06:20 css/update_css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-21 06:20 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-21 06:20 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-21 06:20 css/style_default.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-21 06:20 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-21 06:20 css/kindle.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-21 06:20 css/style_soundwriting.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-21 06:20 css/pretext.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-21 06:20 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-21 06:20 css/colors_martiansands.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-21 06:20 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   109017 b- defN 23-Jun-21 06:20 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-21 06:20 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-21 06:20 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jun-21 06:20 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-21 06:20 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-21 06:20 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   231248 b- defN 23-Jun-21 06:20 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   612399 b- defN 23-Jun-21 06:20 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-21 06:20 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-21 06:20 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-21 06:20 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-21 06:20 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-21 06:20 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-21 06:20 xsl/README.md
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-21 06:20 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-21 06:20 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-21 06:20 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-21 06:20 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-21 06:20 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-21 06:20 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-21 06:20 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-21 06:20 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-21 06:20 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-21 06:20 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-21 06:20 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-21 06:20 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-21 06:20 xsl/entities.ent
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-21 06:20 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-21 06:20 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-21 06:20 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-21 06:20 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-21 06:20 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-21 06:20 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-21 06:20 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-21 06:20 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-21 06:20 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-21 06:20 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-21 06:20 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-21 06:20 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-21 06:20 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-21 06:20 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-21 06:20 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-21 06:20 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-21 06:20 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-21 06:20 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-21 06:20 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-21 06:20 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-21 06:20 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-21 06:20 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-21 06:20 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-21 06:20 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-21 06:20 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-21 06:20 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-Jun-21 06:20 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-21 06:20 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jun-21 06:20 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-21 06:20 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-21 06:20 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-Jun-21 06:20 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-21 06:20 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-21 06:20 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-21 06:20 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-21 06:20 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-21 06:20 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-21 06:20 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-21 06:20 xsl/localizations/en-US.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-21 06:20 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-21 06:20 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-21 06:20 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-21 06:20 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-21 06:20 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-21 06:20 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-21 06:20 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-21 06:20 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-21 06:20 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-21 06:20 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 06:20 pretext/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-21 06:20 pretext/module-test.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-21 06:20 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-21 06:20 pretext/README.md
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-21 06:20 pretext/pretext
+-rw-r--r--  2.0 unx   172432 b- defN 23-Jun-21 06:20 pretext/pretext.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-21 06:20 pretext/braille_format.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-21 06:20 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-21 06:20 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-21 06:20 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-21 06:20 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-21 06:20 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 06:20 script/mjsre/update-sre
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-21 06:20 schema/pretext.xsd
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-21 06:20 schema/pretext.rng
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-21 06:20 schema/pretext.xml
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-21 06:20 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-21 06:20 schema/pretext.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-21 06:20 schema/README.md
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-21 06:20 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-21 06:20 schema/xml.xsd
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-21 06:20 schema/build.sh
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-21 06:20 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-21 06:20 schema/pretext-dev.rng
 141 files, 4814466 bytes uncompressed, 1017983 bytes compressed:  78.9%
```

### Comparing `pretext-1.6.1.dev20230620/pretext/generate.py` & `pretext-1.6.1.dev20230621/pretext/generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 from lxml import etree as ET
 import os
 import logging
 from . import utils, core
 from pathlib import Path
+from typing import Dict, List, Optional
 
 # Get access to logger
 log = logging.getLogger("ptxlogger")
 
 # generate latex-image assets
 
 
 def latex_image(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
-    params,
-    target_format,
-    xmlid_root,
-    pdf_method,
-    all_formats=False,
-):
+    params: Dict[str, str],
+    target_format: str,
+    xmlid_root: Optional[str],
+    pdf_method: str,
+    all_formats: bool = False,
+) -> None:
     # Dictionary of formats for images based on target
     formats = {
-        "pdf": None,
-        "latex": None,
+        "pdf": [],
+        "latex": [],
         "html": ["svg"],
         "epub": ["svg"],
         "kindle": ["png"],
     }
     # set overwrite formats to all when appropriate
     if all_formats:
-        formats[target_format] = {key: ["all"] for key in formats[target_format]}
+        formats[target_format] = ["all"]
     # We assume passed paths are absolute.
     # set images directory
     # parse source so we can check for latex-image.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
     if (
-        len(source_xml.xpath("/pretext/*[not(docinfo)]//latex-image")) > 0
+        isinstance(
+            li := source_xml.xpath("/pretext/*[not(docinfo)]//latex-image"), List
+        )
+        and len(li) > 0
         and formats[target_format] is not None
     ):
         image_output = (output / "latex-image").resolve()
         os.makedirs(image_output, exist_ok=True)
         log.info("Now generating latex-images\n\n")
         # Check for external requirements
         utils.check_asset_execs("latex-image", formats[target_format])
@@ -74,38 +78,39 @@
 # generate sageplot assets
 
 
 def sageplot(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
-    params,
-    target_format,
-    xmlid_root,
-    all_formats=False,
-):
+    params: Dict[str, str],
+    target_format: str,
+    xmlid_root: Optional[str],
+    all_formats: bool = False,
+) -> None:
     # Dictionary of formats for images based on target
     formats = {
         "pdf": ["pdf", "png"],
         "latex": ["pdf", "png"],
         "html": ["html", "svg"],
         "epub": ["svg"],
         "kindle": ["png"],
     }
     # set overwrite formats to all when appropriate
     if all_formats:
-        formats[target_format] = {key: ["all"] for key in formats[target_format]}
+        formats[target_format] = ["all"]
     # We assume passed paths are absolute.
     # set images directory
     # parse source so we can check for sageplot.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
     if (
-        len(source_xml.xpath("/pretext/*[not(docinfo)]//sageplot")) > 0
+        isinstance(li := source_xml.xpath("/pretext/*[not(docinfo)]//sageplot"), List)
+        and len(li) > 0
         and formats[target_format] is not None
     ):
         image_output = (output / "sageplot").resolve()
         os.makedirs(image_output, exist_ok=True)
         log.info("Now generating sageplot images\n\n")
         # Check for external requirements
         utils.check_asset_execs("sageplot", formats[target_format])
@@ -135,19 +140,19 @@
 # generate asymptote assets
 
 
 def asymptote(
     ptxfile: Path,
     pub_file: Path,
     output: Path,
-    params,
-    target_format,
-    xmlid_root,
-    all_formats=False,
-):
+    params: Dict[str, str],
+    target_format: str,
+    xmlid_root: Optional[str],
+    all_formats: bool = False,
+) -> None:
     # Dictionary of formats for images based on target
     formats = {
         "pdf": ["pdf"],
         "latex": ["pdf"],
         "html": ["html"],
         "epub": ["svg"],
         "kindle": ["png"],
@@ -157,15 +162,16 @@
         formats[target_format] = {key: ["all"] for key in formats[target_format]}
     # We assume passed paths are absolute.
     # parse source so we can check for asymptote.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
     if (
-        len(source_xml.xpath("/pretext/*[not(docinfo)]//asymptote")) > 0
+        isinstance(li := source_xml.xpath("/pretext/*[not(docinfo)]//asymptote"), List)
+        and len(li) > 0
         and formats[target_format] is not None
     ):
         image_output = (output / "asymptote").resolve()
         os.makedirs(image_output, exist_ok=True)
         log.info("Now generating asymptote images\n\n")
         with utils.working_directory(Path()):
             try:
@@ -190,21 +196,32 @@
     else:
         log.info("Note: No asymptote elements found.")
 
 
 # generate interactive preview assets
 
 
-def interactive(ptxfile: Path, pub_file: Path, output: Path, params, xmlid_root):
+def interactive(
+    ptxfile: Path,
+    pub_file: Path,
+    output: Path,
+    params: Dict[str, str],
+    xmlid_root: Optional[str],
+) -> None:
     # We assume passed paths are absolute.
     # parse source so we can check for interactives.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
-    if len(source_xml.xpath("/pretext/*[not(docinfo)]//interactive")) > 0:
+    if (
+        isinstance(
+            li := source_xml.xpath("/pretext/*[not(docinfo)]//interactive"), List
+        )
+        and len(li) > 0
+    ):
         # First verify that playwright has dependencies installed:
         utils.playwright_install()
         image_output = (output / "preview").resolve()
         os.makedirs(image_output, exist_ok=True)
         log.info("Now generating preview images for interactives\n\n")
         with utils.working_directory(Path()):
             try:
@@ -226,21 +243,32 @@
     else:
         log.info("Note: No interactive elements found.")
 
 
 # generate youtube thumbnail assets
 
 
-def youtube(ptxfile: Path, pub_file: Path, output: Path, params, xmlid_root):
+def youtube(
+    ptxfile: Path,
+    pub_file: Path,
+    output: Path,
+    params: Dict[str, str],
+    xmlid_root: Optional[str],
+) -> None:
     # We assume passed paths are absolute.
     # parse source so we can check for videos.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
-    if len(source_xml.xpath("/pretext/*[not(docinfo)]//video[@youtube]")) > 0:
+    if (
+        isinstance(
+            li := source_xml.xpath("/pretext/*[not(docinfo)]//video[@youtube]"), List
+        )
+        and len(li) > 0
+    ):
         image_output = (output / "youtube").resolve()
         os.makedirs(image_output, exist_ok=True)
         log.info("Now generating youtube previews\n\n")
         with utils.working_directory(Path()):
             try:
                 core.youtube_thumbnail(
                     xml_source=ptxfile,
@@ -260,21 +288,27 @@
     else:
         log.info("Note: No video@youtube elements found.")
 
 
 # generate webwork assets
 
 
-def webwork(ptxfile: Path, pub_file: Path, output: Path, params, xmlid_root=None):
+def webwork(
+    ptxfile: Path,
+    pub_file: Path,
+    output: Path,
+    params: Dict[str, str],
+    xmlid_root: Optional[str] = None,
+) -> None:
     # We assume passed paths are absolute.
     # parse source so we can check for webwork.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
-    if len(source_xml.xpath("//webwork[node()|@*]")) > 0:
+    if isinstance(li := source_xml.xpath("//webwork[node()|@*]"), List) and len(li) > 0:
         ww_output = (output / "webwork").resolve()
         os.makedirs(ww_output, exist_ok=True)
         log.info("Now generating webwork representation\n\n")
         with utils.working_directory(Path()):
             try:
                 core.webwork_to_xml(
                     xml_source=ptxfile,
@@ -296,21 +330,30 @@
     else:
         log.info("Note: No webwork elements found.")
 
 
 # generate codelens trace assets
 
 
-def codelens(ptxfile: Path, pub_file: Path, output: Path, params, xmlid_root):
+def codelens(
+    ptxfile: Path,
+    pub_file: Path,
+    output: Path,
+    params: Dict[str, str],
+    xmlid_root: Optional[str],
+) -> None:
     # We assume passed paths are absolute.
     # parse source so we can check for webwork.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
-    if len(source_xml.xpath("//program[@interactive = 'codelens']")) > 0:
+    if (
+        isinstance(li := source_xml.xpath("//program[@interactive = 'codelens']"), List)
+        and len(li) > 0
+    ):
         trace_output = (output / "trace").resolve()
         os.makedirs(trace_output, exist_ok=True)
         log.info("Now generating codelens trace\n\n")
         with utils.working_directory(Path()):
             try:
                 core.tracer(
                     xml_source=ptxfile,
@@ -328,23 +371,34 @@
     else:
         log.info("Note: No program elements using codelens found.")
 
 
 # generate qr code assets
 
 
-def qrcodes(ptxfile: Path, pub_file: Path, output: Path, params, xmlid_root):
+def qrcodes(
+    ptxfile: Path,
+    pub_file: Path,
+    output: Path,
+    params: Dict[str, str],
+    xmlid_root: Optional[str],
+) -> None:
     # We assume passed paths are absolute.
     # parse source so we can check for videos.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
     if (
-        len(source_xml.xpath("/pretext/*[not(docinfo)]//video")) > 0
-        or len(source_xml.xpath("/pretext/*[not(docinfo)]//interactive")) > 0
+        isinstance(li1 := source_xml.xpath("/pretext/*[not(docinfo)]//video"), List)
+        and len(li1) > 0
+    ) or (
+        isinstance(
+            li2 := source_xml.xpath("/pretext/*[not(docinfo)]//interactive"), List
+        )
+        and len(li2) > 0
     ):
         image_output = (output / "qrcode").resolve()
         os.makedirs(image_output, exist_ok=True)
         log.info("Now generating QR codes for videos and/or interactives\n\n")
         with utils.working_directory(Path()):
             try:
                 core.qrcode(
@@ -361,15 +415,15 @@
                 log.error(
                     "Failed to generate some QR codes for some videos or interactives. Check your source and partial output to diagnose the issue."
                 )
                 log.warning("Continuing...")
         # No else clause needed, since this isn't called specifically.
 
 
-def play_button(output: Path):
+def play_button(output: Path) -> None:
     # Currently we do not parse source to look for videos, as this can run regardless of the source.
     image_output = (output / "play-button").resolve()
     os.makedirs(image_output, exist_ok=True)
     log.info("Now copying play-button image for videos\n\n")
     with utils.working_directory(Path()):
         try:
             core.play_button(dest_dir=image_output.as_posix())
@@ -381,21 +435,30 @@
                 "Failed to copy play-button image for videos. Please report this on pretext-support."
             )
             log.warning("Continuing...")
     # No else clause needed, since this isn't called specifically.
 
 
 # generate datafile assets
-def datafiles(ptxfile: Path, pub_file: Path, output: Path, params, xmlid_root):
+def datafiles(
+    ptxfile: Path,
+    pub_file: Path,
+    output: Path,
+    params: Dict[str, str],
+    xmlid_root: Optional[str],
+) -> None:
     # We assume passed paths are absolute.
     # parse source so we can check for datafile elements.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
-    if len(source_xml.xpath("/pretext/*[not(docinfo)]//datafile")) > 0:
+    if (
+        isinstance(li := source_xml.xpath("/pretext/*[not(docinfo)]//datafile"), List)
+        and len(li) > 0
+    ):
         datafile_output = (output / "datafile").resolve()
         os.makedirs(datafile_output, exist_ok=True)
         log.info("Now generating base64 versions of datafiles\n\n")
         with utils.working_directory(Path()):
             try:
                 core.datafiles_to_xml(
                     xml_source=ptxfile,
```

### Comparing `pretext-1.6.1.dev20230620/pretext/project.py` & `pretext-1.6.1.dev20230621/pretext/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,277 +1,344 @@
 import pickle
 from lxml import etree as ET
-from lxml.etree import Element
+from lxml.etree import _Element
 import os
 import shutil
 import logging
 import tempfile
 from . import utils, generate, core
 from . import build as builder
 from . import ASSETS
 from pathlib import Path
 import sys
 from .config.xml_overlay import ShadowXmlDocument
-import typing as t
+from typing import Dict, List, Optional, Tuple
 import hashlib
 
 log = logging.getLogger("ptxlogger")
 
+asset_table_type = Dict[Tuple[str, str], bytes]
+
 
 class Target:
-    def __init__(self, xml_element, project_path):
+    def __init__(self, xml_element: _Element, project_path: Path):
         # construction is done!
         self.__xml_element = xml_element
         self.__project_path = Path(project_path).resolve()
         # ensure assets directories exist as assumed by core PreTeXt
-        if self.external_dir() is not None:
-            os.makedirs(self.external_dir(), exist_ok=True)
-        if self.generated_dir() is not None:
-            os.makedirs(self.generated_dir(), exist_ok=True)
+        if (ex_dir := self.external_dir()) is not None:
+            os.makedirs(ex_dir, exist_ok=True)
+        if (gen_dir := self.generated_dir()) is not None:
+            os.makedirs(gen_dir, exist_ok=True)
 
-    def xml_element(self) -> Element:
+    def xml_element(self) -> _Element:
         return self.__xml_element
 
-    def project_path(self):
+    def project_path(self) -> Path:
         return self.__project_path
 
+    # Perform basic schema checking of the project file: the given attribute must be present.
+    def require_str_value(self, value: Optional[str], err: str) -> str:
+        assert value is not None, f"Invalid project file: missing {err}."
+        return value
+
+    def require_tag_text(self, tag_name: str) -> str:
+        element = self.xml_element().find(tag_name)
+        assert element is not None, f"Invalid project file: missing {tag_name} tag."
+        return self.require_str_value(element.text, f"{tag_name} contents")
+
     def name(self) -> str:
-        return self.xml_element().get("name").strip()
+        # Targets should have a name attribute.
+        return self.require_str_value(
+            self.xml_element().get("name"), "name attribute"
+        ).strip()
 
     def pdf_method(self) -> str:
         pdf_method = self.xml_element().get("pdf-method")
         if pdf_method is not None:
             return pdf_method.strip()
         else:
             return "xelatex"  # default
 
     def format(self) -> str:
-        return self.xml_element().find("format").text.strip()
+        return self.require_tag_text("format").strip()
 
     def source(self) -> Path:
-        return self.project_path() / self.xml_element().find("source").text.strip()
+        return self.project_path() / self.require_tag_text("source").strip()
 
     def source_dir(self) -> Path:
         return Path(self.source()).parent
 
-    def source_xml(self):
+    def source_xml(self) -> _Element:
         ele_tree = ET.parse(self.source())
         ele_tree.xinclude()
         return ele_tree.getroot()
 
     def publication(self) -> Path:
-        return self.project_path() / self.xml_element().find("publication").text.strip()
+        return self.project_path() / self.require_tag_text("publication").strip()
 
     def publication_dir(self) -> Path:
         return self.publication().parent
 
     def publication_rel_from_source(self) -> Path:
         return self.publication().relative_to(self.source_dir())
 
-    def publication_xml(self):
+    def publication_xml(self) -> _Element:
         ele_tree = ET.parse(self.publication())
         ele_tree.xinclude()
         return ele_tree.getroot()
 
-    def external_dir(self) -> t.Optional[Path]:
+    def external_dir(self) -> Optional[Path]:
         dir_ele = self.publication_xml().find("source/directories")
         if dir_ele is None:
             log.error("Publication file does not specify asset directories.")
             return None
         rel_dir = dir_ele.get("external")
+        assert (
+            rel_dir is not None
+        ), "Invalid project file: missing value in source/directories/external tag."
         return self.source_dir() / rel_dir
 
-    def generated_dir(self) -> t.Optional[Path]:
+    # Like the above function, but asserts if the external directory wasn't found.
+    def external_dir_found(self) -> Path:
+        ed = self.external_dir()
+        assert ed is not None, "Internal error: external directory not found."
+        return ed
+
+    def generated_dir(self) -> Optional[Path]:
         dir_ele = self.publication_xml().find("source/directories")
         if dir_ele is None:
             log.error("Publication file does not specify asset directories.")
             return None
         rel_dir = dir_ele.get("generated")
+        assert (
+            rel_dir is not None
+        ), "Invalid project file: missing value in source/directories/generated tag."
         return self.source_dir() / rel_dir
 
+    # Like the above function, but asserts if the external directory wasn't found.
+    def generated_dir_found(self) -> Path:
+        gd = self.generated_dir()
+        assert gd is not None, "Internal error: generated directory not found."
+        return gd
+
     def output_dir(self) -> Path:
         return (
-            Path(self.__project_path)
-            / self.xml_element().find("output-dir").text.strip()
+            Path(self.__project_path) / self.require_tag_text("output-dir").strip()
         ).resolve()
 
-    def output_filename(self) -> t.Optional[str]:
+    def output_filename(self) -> Optional[str]:
         if self.xml_element().find("output-filename") is None:
             return None
         else:
-            return self.xml_element().find("output-filename").text.strip()
+            return self.require_tag_text("output-filename").strip()
 
     def port(self) -> int:
         view_ele = self.xml_element().find("view")
-        if view_ele is not None and view_ele.get("port") is not None:
-            return int(view_ele.get("port"))
+        if view_ele is not None and (port := view_ele.get("port")) is not None:
+            return int(port)
         else:
             return 8000
 
-    def stringparams(self):
-        return {
-            sp_ele.get("key").strip(): sp_ele.get("value").strip()
-            for sp_ele in self.xml_element().xpath("stringparam")
-        }
+    def stringparams(self) -> Dict[str, str]:
+        sp = self.xml_element().xpath("stringparam")
+        assert isinstance(sp, List), "Project file error: stringparam is empty."
+        ret = {}
+        for sp_ele in sp:
+            assert isinstance(
+                sp_ele, _Element
+            ), "Project file error: stringparam contents must be key/value pairs."
+            key = self.require_str_value(
+                sp_ele.get("key"), "Project  file error: stringparam missing key."
+            )
+            value = self.require_str_value(
+                sp_ele.get("value"), "Project  file error: stringparam missing value."
+            )
+            ret[key.strip()] = value.strip()
+        return ret
 
-    def xsl_path(self) -> t.Optional[Path]:
+    def xsl_path(self) -> Optional[Path]:
         if self.xml_element().find("xsl") is not None:
             return (
-                Path(self.__project_path) / self.xml_element().find("xsl").text.strip()
+                Path(self.__project_path) / self.require_tag_text("xsl").strip()
             ).resolve()
         else:
             return None
 
-    def xmlid_root(self):
+    def xmlid_root(self) -> Optional[str]:
         ele = self.xml_element().find("xmlid-root")
         if ele is None:
             return None
         else:
-            return ele.text.strip()
+            return self.require_str_value(ele.text, "xmlid-root").strip()
 
-    def asset_hash(self):
+    def asset_hash(self) -> asset_table_type:
         asset_hash_dict = {}
         for asset in ASSETS:
             if asset == "webwork":
+                ww = self.source_xml().xpath(".//webwork[@*|*]")
+                assert isinstance(ww, List)
                 # WeBWorK must be regenerated every time *any* of the ww exercises change.
-                if len(self.source_xml().xpath(".//webwork[@*|*]")) == 0:
+                if len(ww) == 0:
                     # Only generate a hash if there are actually ww exercises in the source
                     continue
                 h = hashlib.sha256()
-                for node in self.source_xml().xpath(".//webwork[@*|*]"):
+                for node in ww:
+                    assert isinstance(node, _Element)
                     h.update(ET.tostring(node))
                 asset_hash_dict[(asset, "")] = h.digest()
             elif asset != "ALL":
                 # everything else can be updated individually, if it has an xml:id
-                if len(self.source_xml().xpath(f".//{asset}")) == 0:
+                source_assets = self.source_xml().xpath(f".//{asset}")
+                assert isinstance(source_assets, List)
+                if len(source_assets) == 0:
                     # Only generate a hash if there are actually assets of this type in the source
                     continue
                 h_no_id = hashlib.sha256()
-                for node in self.source_xml().xpath(f".//{asset}"):
+                for node in source_assets:
+                    assert isinstance(node, _Element)
                     # First see if the node has an xml:id, or if it is a child of a node with an xml:id (but we haven't already made this key)
                     if (
-                        id := node.xpath("@xml:id") or node.xpath("parent::*/@xml:id")
-                    ) and (asset, id[0]) not in asset_hash_dict:
+                        (id := node.xpath("@xml:id") or node.xpath("parent::*/@xml:id"))
+                        and isinstance(id, List)
+                        and (asset, id[0]) not in asset_hash_dict
+                    ):
+                        assert isinstance(id, _Element)
                         asset_hash_dict[(asset, id[0])] = hashlib.sha256(
                             ET.tostring(node)
                         ).digest()
                     # otherwise collect all non-id'd nodes into a single hash
                     else:
                         h_no_id.update(ET.tostring(node))
                 asset_hash_dict[(asset, "")] = h_no_id.digest()
         return asset_hash_dict
 
-    def save_asset_table(self, asset_table: dict):
+    def save_asset_table(self, asset_table: asset_table_type) -> None:
         """
         Saves the asset_table to a pickle file in the generated assets directory based on the target name.
         """
         with open(
-            self.generated_dir().joinpath(f".{self.name()}_assets.pkl"), "wb"
+            self.generated_dir_found().joinpath(f".{self.name()}_assets.pkl"), "wb"
         ) as f:
             pickle.dump(asset_table, f)
 
-    def load_asset_table(self) -> dict:
+    def load_asset_table(self) -> asset_table_type:
         """
         Loads the asset_table from a pickle file in the generated assets directory based on the target name.
         """
         try:
             with open(
-                self.generated_dir().joinpath(f".{self.name()}_assets.pkl"), "rb"
+                self.generated_dir_found().joinpath(f".{self.name()}_assets.pkl"), "rb"
             ) as f:
                 return pickle.load(f)
         except Exception:
             return {}
 
-    def needs_ww_reps(self):
+    def needs_ww_reps(self) -> bool:
         return self.source_xml().find(".//webwork/statement") is not None
 
-    def has_ww_reps(self):
+    def has_ww_reps(self) -> bool:
         return Path.exists(
-            self.generated_dir() / "webwork" / "webwork-representations.xml"
+            self.generated_dir_found() / "webwork" / "webwork-representations.xml"
         )
 
 
 class Project:
-    def __init__(self, project_path=None):
+    def __init__(self, project_path: Optional[Path] = None):
         project_path = project_path or utils.project_path()
+        assert project_path is not None, "Unable to find project path."
         xml_element = ET.parse(project_path / "project.ptx").getroot()
         self.__xml_element = xml_element
         self.__project_path = project_path
         # prepre core PreTeXt python scripts
         self.init_ptxcore()
 
-    def apply_overlay(self, overlay: ShadowXmlDocument):
+    def apply_overlay(self, overlay: ShadowXmlDocument) -> List[str]:
         """
         Modify the internal data structure of the `project.ptx` XML tree by applying the supplied overlay.
         This modification happens in-memory only.
         """
         return overlay.overlay_tree(self.__xml_element)
 
-    def xml_element(self) -> Element:
+    def xml_element(self) -> _Element:
         return self.__xml_element
 
-    def targets(self):
-        return [
-            Target(xml_element=target_element, project_path=self.__project_path)
-            for target_element in self.xml_element().xpath("targets/target")
-        ]
+    def targets(self) -> List[Target]:
+        t = self.xml_element().xpath("targets/target")
+        assert isinstance(
+            t, List
+        ), "Project file error: expected list of targets in targets/target tags."
+        ret: List[Target] = []
+        for target_element in t:
+            assert isinstance(t, _Element), "Project file error: target must be a tag."
+            t.append(
+                Target(xml_element=target_element, project_path=self.__project_path)
+            )
+        return ret
 
-    def target_names(self, *args):
+    def target_names(self, *args: str) -> List[str]:
         # Optional arguments are formats: returns list of targets that have that format.
         names = []
         for target in self.targets():
             if not args or target.format() in args:
                 names.append(target.name())
         return names
 
-    def print_target_names(self):
+    def print_target_names(self) -> None:
         for target in self.targets():
             print(target.name())
 
-    def target(self, name=None) -> Target:
+    def target(self, name: Optional[str] = None) -> Optional[Target]:
         if name is None:
             target_element = self.xml_element().find("targets/target")
         else:
             target_element = self.xml_element().find(f'targets/target[@name="{name}"]')
         if target_element is not None:
             return Target(xml_element=target_element, project_path=self.__project_path)
         else:
+            log.error("Unable to find target.")
             return None
 
     def view(
         self,
         target_name: str,
         access: str,
         port: int,
         watch: bool = False,
         no_launch: bool = False,
-    ):
+    ) -> None:
         target = self.target(target_name)
+        if target is None:
+            log.error("Unable to find target.")
+            return
         directory = target.output_dir()
 
         if watch:
             watch_directory = target.source_dir()
         else:
             watch_directory = None
         if not target.output_dir().exists():
             log.error(f"The directory `{target.output_dir()}` does not exist.")
             log.error(
                 f"Run `pretext view {target.name()} -b` to build your project before viewing."
             )
             return
 
-        def watch_callback():
-            return self.build(target_name)
+        def watch_callback() -> None:
+            self.build(target_name)
 
         utils.run_server(
             directory, access, port, watch_directory, watch_callback, no_launch
         )
 
-    def build(self, target_name, clean=False):
+    def build(self, target_name: str, clean: bool = False) -> None:
         target = self.target(target_name)
+        if target is None:
+            log.error(f"Target `{target_name}` not found.")
+            return
         # Check for xml syntax errors and quit if xml invalid:
         if not self.xml_source_is_valid(target_name):
             return
         if not self.xml_publication_is_valid(target_name):
             return
         # Validate xml against schema; continue with warning if invalid:
         self.xml_schema_validate(target_name)
@@ -296,21 +363,19 @@
             else:
                 log.warning(
                     f"Destroying directory {target.output_dir()} to clean previously built files."
                 )
                 shutil.rmtree(target.output_dir())
         # if custom xsl, copy it into a temporary directory (different from the building temporary directory)
         custom_xsl = None
-        if target.xsl_path() is not None:
+        if (txp := target.xsl_path()) is not None:
             temp_xsl_path = Path(tempfile.mkdtemp())
-            log.info(
-                f"Building with custom xsl {target.xsl_path()} specified in project.ptx"
-            )
-            utils.copy_custom_xsl(target.xsl_path(), temp_xsl_path)
-            custom_xsl = temp_xsl_path / target.xsl_path().name
+            log.info(f"Building with custom xsl {txp} specified in project.ptx")
+            utils.copy_custom_xsl(txp, temp_xsl_path)
+            custom_xsl = temp_xsl_path / txp.name
         # warn if "publisher" is one of the string-param keys:
         if "publisher" in target.stringparams():
             log.warning(
                 "You specified a publication file via a stringparam.  This is ignored in favor of the publication file given by the <publication> element in the project manifest."
             )
         log.info(f"Preparing to build into {target.output_dir()}.")
         try:
@@ -331,20 +396,20 @@
                     target.publication(),
                     target.output_dir(),
                     target.stringparams(),
                     custom_xsl,
                 )
                 # core script doesn't put a copy of images in output for latex builds, so we do it instead here
                 shutil.copytree(
-                    target.external_dir(),
+                    target.external_dir_found(),
                     target.output_dir() / "external",
                     dirs_exist_ok=True,
                 )
                 shutil.copytree(
-                    target.generated_dir(),
+                    target.generated_dir_found(),
                     target.output_dir() / "generated",
                     dirs_exist_ok=True,
                 )
             elif target.format() == "pdf":
                 builder.pdf(
                     target.source(),
                     target.publication(),
@@ -417,129 +482,138 @@
             core.release_temporary_directories()
         # build was successful
         log.info(f"\nSuccess! Run `pretext view {target.name()}` to see the results.\n")
         if custom_xsl is not None:
             # errors may occur in Windows so we do the best we can
             shutil.rmtree(custom_xsl.parent, ignore_errors=True)
 
-    def generate(self, target_name, asset_list=None, all_formats=False, xmlid=None):
+    def generate(
+        self,
+        target_name: str,
+        asset_list: Optional[List[str]] = None,
+        all_formats: bool = False,
+        xmlid: Optional[str] = None,
+    ) -> None:
         if asset_list is None:
             asset_list = []
             gen_all = True
         else:
             gen_all = False
         target = self.target(target_name)
-        xmlid = xmlid or target.xmlid_root()
         if target is None:
             log.error(f"Target `{target_name}` not found.")
             return
+        xmlid = xmlid or target.xmlid_root()
         # build targets:
         if gen_all or "webwork" in asset_list:
-            webwork_output = target.generated_dir() / "webwork"
+            webwork_output = target.generated_dir_found() / "webwork"
             generate.webwork(
                 target.source(),
                 target.publication(),
                 webwork_output,
                 target.stringparams(),
                 xmlid,
             )
         if gen_all or "latex-image" in asset_list:
             generate.latex_image(
                 target.source(),
                 target.publication(),
-                target.generated_dir(),
+                target.generated_dir_found(),
                 target.stringparams(),
                 target.format(),
                 xmlid,
                 target.pdf_method(),
                 all_formats,
             )
         if gen_all or "asymptote" in asset_list:
             generate.asymptote(
                 target.source(),
                 target.publication(),
-                target.generated_dir(),
+                target.generated_dir_found(),
                 target.stringparams(),
                 target.format(),
                 xmlid,
                 all_formats,
             )
         if gen_all or "sageplot" in asset_list:
             generate.sageplot(
                 target.source(),
                 target.publication(),
-                target.generated_dir(),
+                target.generated_dir_found(),
                 target.stringparams(),
                 target.format(),
                 xmlid,
                 all_formats,
             )
         if gen_all or "interactive" in asset_list:
             generate.interactive(
                 target.source(),
                 target.publication(),
-                target.generated_dir(),
+                target.generated_dir_found(),
                 target.stringparams(),
                 xmlid,
             )
         if gen_all or "youtube" in asset_list:
             generate.youtube(
                 target.source(),
                 target.publication(),
-                target.generated_dir(),
+                target.generated_dir_found(),
                 target.stringparams(),
                 xmlid,
             )
             generate.play_button(
-                target.generated_dir(),
+                target.generated_dir_found(),
             )
         if gen_all or "codelens" in asset_list:
             generate.codelens(
                 target.source(),
                 target.publication(),
-                target.generated_dir(),
+                target.generated_dir_found(),
                 target.stringparams(),
                 xmlid,
             )
         if gen_all or "datafile" in asset_list:
             generate.datafiles(
                 target.source(),
                 target.publication(),
-                target.generated_dir(),
+                target.generated_dir_found(),
                 target.stringparams(),
                 xmlid,
             )
         if gen_all or "interactive" in asset_list or "youtube" in asset_list:
             generate.qrcodes(
                 target.source(),
                 target.publication(),
-                target.generated_dir(),
+                target.generated_dir_found(),
                 target.stringparams(),
                 xmlid,
             )
         # Delete temporary directories left behind by core:
         core.release_temporary_directories()
 
-    def deploy(self, target_name, update_source):
+    def deploy(self, target_name: str, update_source: bool) -> None:
         try:
             import git
             import ghp_import
         except ImportError:
             log.error(
                 "Git must be installed to use this feature, but couldn't be found."
             )
             log.error("Visit https://github.com/git-guides/install-git for assistance.")
             return
         target = self.target(target_name)
+        if target is None:
+            log.error(f"Target `{target_name}` not found.")
+            return
         if target.format() != "html":  # redundant for CLI
             log.error("Only HTML format targets are supported.")
             return
         try:
             repo = git.Repo(self.__project_path)
-        except git.exc.InvalidGitRepositoryError:
+        except git.exc.InvalidGitRepositoryError:  # type: ignore
             log.info("Initializing project with Git.")
             repo = git.Repo.init(self.__project_path)
             try:
                 repo.config_reader().get_value("user", "name")
                 repo.config_reader().get_value("user", "email")
             except Exception:
                 log.info("Setting up name/email configuration for Git...")
@@ -621,15 +695,15 @@
         except Exception:
             log.error(f"Unable to parse GitHub URL from {origin.url}")
             log.error("Deploy unsuccessful")
             return
         try:
             origin.push(refspec=f"{repo.active_branch.name}:{repo.active_branch.name}")
             origin.push(refspec="gh-pages:gh-pages")
-        except git.exc.GitCommandError:
+        except git.exc.GitCommandError:  # type: ignore
             log.warning(
                 f"There was an issue connecting to GitHub repository located at {repo_url}"
             )
             log.info("")
             log.info(
                 "If you haven't already, configure SSH with GitHub by following instructions at:"
             )
@@ -655,24 +729,31 @@
         log.info("Visit")
         log.info(f"    {repo_url}actions/")
         log.info("to check on the status of your GitHub Pages deployment.")
         log.info("")
         log.info("Your built project will soon be available to the public at:")
         log.info(f"    {pages_url}")
 
-    def xml_source_is_valid(self, target_name):
+    def xml_source_is_valid(self, target_name: str) -> bool:
         target = self.target(target_name)
+        if target is None:
+            return False
         return utils.xml_syntax_is_valid(target.source())
 
-    def xml_schema_validate(self, target_name):
+    def xml_schema_validate(self, target_name: str) -> bool:
         target = self.target(target_name)
+        if target is None:
+            return False
         return utils.xml_source_validates_against_schema(target.source())
 
-    def xml_publication_is_valid(self, target_name):
+    def xml_publication_is_valid(self, target_name: str) -> bool:
         target = self.target(target_name)
+        if target is None:
+            log.error(f"Target `{target_name}` not found.")
+            return False
         try:
             publication_xml = ET.parse(target.publication())
             # Would we ever have a publication with xi:include?  Just in case...
             publication_xml.xinclude()
         except Exception as e:
             log.critical(f"Unable to read publication file.  Quitting. {e}")
             log.debug("", exc_info=True)
@@ -680,12 +761,28 @@
         if publication_xml.getroot().tag != "publication":
             log.error(
                 f'The publication file {target.publication()} must have "<publication>" as its root element.'
             )
             return False
         return True
 
-    def executables(self):
-        return {ele.tag: ele.text for ele in self.xml_element().xpath("executables/*")}
+    def executables(self) -> Dict[str, str]:
+        ret = {}
+        exec = self.xml_element().xpath("executables/*")
+        assert isinstance(
+            exec, List
+        ), "Invalid project file: executables tag contents must be tags."
+        for ele in exec:
+            assert isinstance(
+                ele, _Element
+            ), "Invalid project file: children of <executables> must be tags."
+            key = ele.tag
+            value = ele.text
+            assert (
+                value is not None
+            ), "Invalid project file: missing value in <executables> tag."
+            ret[key] = value
+
+        return ret
 
-    def init_ptxcore(self):
+    def init_ptxcore(self) -> None:
         core.set_executables(self.executables())
```

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230621/pretext/templates/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from pathlib import Path
+from contextlib import AbstractContextManager
 import importlib.resources as ir
 
 
-def resource_path(filename: str) -> Path:
+def resource_path(filename: str) -> AbstractContextManager:
     """
     Returns resource manager
     Usage:
     with resource_path('foo.bar') as filepath:
         # do things
     """
     from . import resources
```

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230621/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230621/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 160064 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-20 06:20 .gitignore
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-20 06:19 README.md
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-20 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-20 06:20 project.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-20 06:19 assets/frog.jpg
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-20 06:19 source/section-1.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-20 06:19 source/main.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-20 06:19 source/section-2.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-20 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-20 06:19 publication/publication.ptx
-14 files, 164708 bytes uncompressed, 158542 bytes compressed:  3.7%
+Zip file size: 160110 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-21 06:20 .gitignore
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-21 06:19 README.md
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-21 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-21 06:20 project.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-21 06:19 assets/frog.jpg
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-21 06:19 source/section-1.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-21 06:19 source/main.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-21 06:19 source/section-2.ptx
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-21 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-21 06:19 publication/publication.ptx
+14 files, 164841 bytes uncompressed, 158588 bytes compressed:  3.8%
```

#### .devcontainer/devcontainer.json

```diff
@@ -4,15 +4,18 @@
   // This Docker image includes some LaTeX support, but is still not to large.  Note that if you keep your codespace running, it will use up your GitHub free storage quota.  Additional options are listed below.
   "image": "oscarlevin/pretext:small",
   // If you need to generate more complicated assets (such as sageplots) or use additional fonts when building to PDF, comment out the above line and uncomment the following line.
   // "image": "oscarlevin/pretext:full",
   // If you only intend to build for web and don't have any latex-image generated assets, you can use a smaller image:
   // "image": "oscarlevin/pretext:lite",
 
-
+  // Add gh cli as a feature (to support chodechat)
+  "features": {
+    "ghcr.io/devcontainers/features/github-cli:1": {}
+  },
 
   // The following was the previous version of this file, which used the Codespaces base image.  It is still available for reference, but is not recommended.
   // "image": "mcr.microsoft.com/devcontainers/python:3",
   // "features": {
   //   "ghcr.io/devcontainers/features/node:1": {},
   //   "ghcr.io/rocker-org/devcontainer-features/pandoc:1": {}
   // },
@@ -27,31 +30,31 @@
   // 		"requireLocalPort": true,
   // 		"elevateIfNeeded": true,
   // 		"protocol": "https"
   // 	}
   // },
   // "onCreateCommand": "pip install pretext",
   // // Use 'postCreateCommand' to run commands after the container is created.
-  // "postCreateCommand": "sudo bash ./.devcontainer/postCreateCommand.sh",
 
   // Configure tool-specific properties.
   "customizations": {
     "codespaces": {
       "openFiles": [
         "source/main.ptx"
       ]
     },
     "vscode": {
       "settings": {
         "editor.quickSuggestions": {
           "other": "off"
         },
         "editor.snippetSuggestions": "top",
-        "xml.validation.enabled": false
+        "xml.validation.enabled": false,
+        "CodeChat.CodeChatServer.Command": "CodeChat_Server"
       },
-      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools"]
+      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools", "CodeChat.codechat"]
     }
   }
 
   // Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
   // "remoteUser": "root"
 }
```

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230621/pretext/templates/resources/book.zip`

 * *Files 19% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7570 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-20 06:20 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-20 06:19 README.md
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-20 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-20 06:20 project.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-20 06:19 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-20 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-20 06:19 publication/publication.ptx
-10 files, 15676 bytes uncompressed, 6476 bytes compressed:  58.7%
+Zip file size: 7616 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-21 06:20 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-21 06:19 README.md
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-21 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-21 06:20 project.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-21 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-21 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-21 06:19 publication/publication.ptx
+10 files, 15809 bytes uncompressed, 6522 bytes compressed:  58.7%
```

#### .devcontainer/devcontainer.json

```diff
@@ -4,15 +4,18 @@
   // This Docker image includes some LaTeX support, but is still not to large.  Note that if you keep your codespace running, it will use up your GitHub free storage quota.  Additional options are listed below.
   "image": "oscarlevin/pretext:small",
   // If you need to generate more complicated assets (such as sageplots) or use additional fonts when building to PDF, comment out the above line and uncomment the following line.
   // "image": "oscarlevin/pretext:full",
   // If you only intend to build for web and don't have any latex-image generated assets, you can use a smaller image:
   // "image": "oscarlevin/pretext:lite",
 
-
+  // Add gh cli as a feature (to support chodechat)
+  "features": {
+    "ghcr.io/devcontainers/features/github-cli:1": {}
+  },
 
   // The following was the previous version of this file, which used the Codespaces base image.  It is still available for reference, but is not recommended.
   // "image": "mcr.microsoft.com/devcontainers/python:3",
   // "features": {
   //   "ghcr.io/devcontainers/features/node:1": {},
   //   "ghcr.io/rocker-org/devcontainer-features/pandoc:1": {}
   // },
@@ -27,31 +30,31 @@
   // 		"requireLocalPort": true,
   // 		"elevateIfNeeded": true,
   // 		"protocol": "https"
   // 	}
   // },
   // "onCreateCommand": "pip install pretext",
   // // Use 'postCreateCommand' to run commands after the container is created.
-  // "postCreateCommand": "sudo bash ./.devcontainer/postCreateCommand.sh",
 
   // Configure tool-specific properties.
   "customizations": {
     "codespaces": {
       "openFiles": [
         "source/main.ptx"
       ]
     },
     "vscode": {
       "settings": {
         "editor.quickSuggestions": {
           "other": "off"
         },
         "editor.snippetSuggestions": "top",
-        "xml.validation.enabled": false
+        "xml.validation.enabled": false,
+        "CodeChat.CodeChatServer.Command": "CodeChat_Server"
       },
-      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools"]
+      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools", "CodeChat.codechat"]
     }
   }
 
   // Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
   // "remoteUser": "root"
 }
```

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230621/pretext/templates/resources/demo.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
-Zip file size: 173263 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-20 06:20 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-20 06:19 README.md
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-20 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-20 06:20 project.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-20 06:19 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-20 06:19 assets/jsxgraph/infinity.js
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 source/images/
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-20 06:19 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-20 06:19 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-20 06:19 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-20 06:19 source/ch-empty.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-20 06:19 source/main.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-20 06:19 source/ex-first.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-20 06:19 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-20 06:19 source/docinfo.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-20 06:19 source/ch-features.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-20 06:19 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-20 06:19 source/ch-generate.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-20 06:19 source/sec-features.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-20 06:19 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-20 06:19 source/backmatter.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-20 06:19 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-20 06:19 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-20 06:19 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-20 06:19 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-20 06:19 source/images/tikz.tex
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-20 06:19 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-20 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-20 06:19 publication/publication.ptx
-34 files, 189971 bytes uncompressed, 169307 bytes compressed:  10.9%
+Zip file size: 173309 bytes, number of entries: 34
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-21 06:20 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-21 06:19 README.md
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-21 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-21 06:20 project.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-21 06:19 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-21 06:19 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 source/images/
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-21 06:19 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-21 06:19 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-21 06:19 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-21 06:19 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-21 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-21 06:19 source/ex-first.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-21 06:19 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-21 06:19 source/docinfo.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-21 06:19 source/ch-features.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-21 06:19 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-21 06:19 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-21 06:19 source/sec-features.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-21 06:19 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-21 06:19 source/backmatter.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-21 06:19 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-21 06:19 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-21 06:19 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-21 06:19 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-21 06:19 source/images/tikz.tex
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-21 06:19 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-21 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-21 06:19 publication/publication.ptx
+34 files, 190104 bytes uncompressed, 169353 bytes compressed:  10.9%
```

#### .devcontainer/devcontainer.json

```diff
@@ -4,15 +4,18 @@
   // This Docker image includes some LaTeX support, but is still not to large.  Note that if you keep your codespace running, it will use up your GitHub free storage quota.  Additional options are listed below.
   "image": "oscarlevin/pretext:small",
   // If you need to generate more complicated assets (such as sageplots) or use additional fonts when building to PDF, comment out the above line and uncomment the following line.
   // "image": "oscarlevin/pretext:full",
   // If you only intend to build for web and don't have any latex-image generated assets, you can use a smaller image:
   // "image": "oscarlevin/pretext:lite",
 
-
+  // Add gh cli as a feature (to support chodechat)
+  "features": {
+    "ghcr.io/devcontainers/features/github-cli:1": {}
+  },
 
   // The following was the previous version of this file, which used the Codespaces base image.  It is still available for reference, but is not recommended.
   // "image": "mcr.microsoft.com/devcontainers/python:3",
   // "features": {
   //   "ghcr.io/devcontainers/features/node:1": {},
   //   "ghcr.io/rocker-org/devcontainer-features/pandoc:1": {}
   // },
@@ -27,31 +30,31 @@
   // 		"requireLocalPort": true,
   // 		"elevateIfNeeded": true,
   // 		"protocol": "https"
   // 	}
   // },
   // "onCreateCommand": "pip install pretext",
   // // Use 'postCreateCommand' to run commands after the container is created.
-  // "postCreateCommand": "sudo bash ./.devcontainer/postCreateCommand.sh",
 
   // Configure tool-specific properties.
   "customizations": {
     "codespaces": {
       "openFiles": [
         "source/main.ptx"
       ]
     },
     "vscode": {
       "settings": {
         "editor.quickSuggestions": {
           "other": "off"
         },
         "editor.snippetSuggestions": "top",
-        "xml.validation.enabled": false
+        "xml.validation.enabled": false,
+        "CodeChat.CodeChatServer.Command": "CodeChat_Server"
       },
-      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools"]
+      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools", "CodeChat.codechat"]
     }
   }
 
   // Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
   // "remoteUser": "root"
 }
```

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230621/pretext/templates/resources/devcontainer.json`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,18 @@
   // This Docker image includes some LaTeX support, but is still not to large.  Note that if you keep your codespace running, it will use up your GitHub free storage quota.  Additional options are listed below.
   "image": "oscarlevin/pretext:small",
   // If you need to generate more complicated assets (such as sageplots) or use additional fonts when building to PDF, comment out the above line and uncomment the following line.
   // "image": "oscarlevin/pretext:full",
   // If you only intend to build for web and don't have any latex-image generated assets, you can use a smaller image:
   // "image": "oscarlevin/pretext:lite",
 
-
+  // Add gh cli as a feature (to support chodechat)
+  "features": {
+    "ghcr.io/devcontainers/features/github-cli:1": {}
+  },
 
   // The following was the previous version of this file, which used the Codespaces base image.  It is still available for reference, but is not recommended.
   // "image": "mcr.microsoft.com/devcontainers/python:3",
   // "features": {
   //   "ghcr.io/devcontainers/features/node:1": {},
   //   "ghcr.io/rocker-org/devcontainer-features/pandoc:1": {}
   // },
@@ -27,31 +30,31 @@
   // 		"requireLocalPort": true,
   // 		"elevateIfNeeded": true,
   // 		"protocol": "https"
   // 	}
   // },
   // "onCreateCommand": "pip install pretext",
   // // Use 'postCreateCommand' to run commands after the container is created.
-  // "postCreateCommand": "sudo bash ./.devcontainer/postCreateCommand.sh",
 
   // Configure tool-specific properties.
   "customizations": {
     "codespaces": {
       "openFiles": [
         "source/main.ptx"
       ]
     },
     "vscode": {
       "settings": {
         "editor.quickSuggestions": {
           "other": "off"
         },
         "editor.snippetSuggestions": "top",
-        "xml.validation.enabled": false
+        "xml.validation.enabled": false,
+        "CodeChat.CodeChatServer.Command": "CodeChat_Server"
       },
-      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools"]
+      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools", "CodeChat.codechat"]
     }
   }
 
   // Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
   // "remoteUser": "root"
 }
```

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230621/pretext/templates/resources/hello.zip`

 * *Files 21% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4611 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-20 06:20 .gitignore
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-20 06:19 README.md
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-20 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-20 06:19 project.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-20 06:19 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-20 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-20 06:19 publication/publication.ptx
-10 files, 7687 bytes uncompressed, 3517 bytes compressed:  54.2%
+Zip file size: 4657 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-21 06:20 .gitignore
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-21 06:19 README.md
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-21 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-21 06:19 project.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-21 06:19 source/main.ptx
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-21 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-21 06:19 publication/publication.ptx
+10 files, 7820 bytes uncompressed, 3563 bytes compressed:  54.4%
```

#### .devcontainer/devcontainer.json

```diff
@@ -4,15 +4,18 @@
   // This Docker image includes some LaTeX support, but is still not to large.  Note that if you keep your codespace running, it will use up your GitHub free storage quota.  Additional options are listed below.
   "image": "oscarlevin/pretext:small",
   // If you need to generate more complicated assets (such as sageplots) or use additional fonts when building to PDF, comment out the above line and uncomment the following line.
   // "image": "oscarlevin/pretext:full",
   // If you only intend to build for web and don't have any latex-image generated assets, you can use a smaller image:
   // "image": "oscarlevin/pretext:lite",
 
-
+  // Add gh cli as a feature (to support chodechat)
+  "features": {
+    "ghcr.io/devcontainers/features/github-cli:1": {}
+  },
 
   // The following was the previous version of this file, which used the Codespaces base image.  It is still available for reference, but is not recommended.
   // "image": "mcr.microsoft.com/devcontainers/python:3",
   // "features": {
   //   "ghcr.io/devcontainers/features/node:1": {},
   //   "ghcr.io/rocker-org/devcontainer-features/pandoc:1": {}
   // },
@@ -27,31 +30,31 @@
   // 		"requireLocalPort": true,
   // 		"elevateIfNeeded": true,
   // 		"protocol": "https"
   // 	}
   // },
   // "onCreateCommand": "pip install pretext",
   // // Use 'postCreateCommand' to run commands after the container is created.
-  // "postCreateCommand": "sudo bash ./.devcontainer/postCreateCommand.sh",
 
   // Configure tool-specific properties.
   "customizations": {
     "codespaces": {
       "openFiles": [
         "source/main.ptx"
       ]
     },
     "vscode": {
       "settings": {
         "editor.quickSuggestions": {
           "other": "off"
         },
         "editor.snippetSuggestions": "top",
-        "xml.validation.enabled": false
+        "xml.validation.enabled": false,
+        "CodeChat.CodeChatServer.Command": "CodeChat_Server"
       },
-      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools"]
+      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools", "CodeChat.codechat"]
     }
   }
 
   // Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
   // "remoteUser": "root"
 }
```

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230621/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230620/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230621/pretext/templates/resources/slideshow.zip`

 * *Files 26% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8346 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 06:19 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-20 06:20 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-20 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-20 06:19 project.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-20 06:19 source/main.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-20 06:19 xsl/slides.xsl
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-20 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-20 06:19 publication/publication.ptx
-11 files, 20274 bytes uncompressed, 7158 bytes compressed:  64.7%
+Zip file size: 8392 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 06:19 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-21 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-21 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-21 06:19 project.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-21 06:19 source/main.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-21 06:19 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-21 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-21 06:19 publication/publication.ptx
+11 files, 20407 bytes uncompressed, 7204 bytes compressed:  64.7%
```

#### .devcontainer/devcontainer.json

```diff
@@ -4,15 +4,18 @@
   // This Docker image includes some LaTeX support, but is still not to large.  Note that if you keep your codespace running, it will use up your GitHub free storage quota.  Additional options are listed below.
   "image": "oscarlevin/pretext:small",
   // If you need to generate more complicated assets (such as sageplots) or use additional fonts when building to PDF, comment out the above line and uncomment the following line.
   // "image": "oscarlevin/pretext:full",
   // If you only intend to build for web and don't have any latex-image generated assets, you can use a smaller image:
   // "image": "oscarlevin/pretext:lite",
 
-
+  // Add gh cli as a feature (to support chodechat)
+  "features": {
+    "ghcr.io/devcontainers/features/github-cli:1": {}
+  },
 
   // The following was the previous version of this file, which used the Codespaces base image.  It is still available for reference, but is not recommended.
   // "image": "mcr.microsoft.com/devcontainers/python:3",
   // "features": {
   //   "ghcr.io/devcontainers/features/node:1": {},
   //   "ghcr.io/rocker-org/devcontainer-features/pandoc:1": {}
   // },
@@ -27,31 +30,31 @@
   // 		"requireLocalPort": true,
   // 		"elevateIfNeeded": true,
   // 		"protocol": "https"
   // 	}
   // },
   // "onCreateCommand": "pip install pretext",
   // // Use 'postCreateCommand' to run commands after the container is created.
-  // "postCreateCommand": "sudo bash ./.devcontainer/postCreateCommand.sh",
 
   // Configure tool-specific properties.
   "customizations": {
     "codespaces": {
       "openFiles": [
         "source/main.ptx"
       ]
     },
     "vscode": {
       "settings": {
         "editor.quickSuggestions": {
           "other": "off"
         },
         "editor.snippetSuggestions": "top",
-        "xml.validation.enabled": false
+        "xml.validation.enabled": false,
+        "CodeChat.CodeChatServer.Command": "CodeChat_Server"
       },
-      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools"]
+      "extensions": ["ms-vscode.live-server", "oscarlevin.pretext-tools", "CodeChat.codechat"]
     }
   }
 
   // Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
   // "remoteUser": "root"
 }
```

### Comparing `pretext-1.6.1.dev20230620/pretext/utils.py` & `pretext-1.6.1.dev20230621/pretext/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import os
 import random
 import json
+from collections.abc import Generator
 from contextlib import contextmanager
 from http.server import SimpleHTTPRequestHandler
 import shutil
 from pathlib import Path
 import platform
 import re
 import socketserver
 import socket
 import subprocess
 import sys
 import logging
+import logging.handlers
 import threading
 import watchdog.events
 import watchdog.observers
 import time
 import webbrowser
 import typing as t
 from lxml import etree as ET
-from typing import Optional
+from lxml.etree import _ElementTree, _Element
+from typing import Any, cast, Callable, List, Optional
 
 from . import core, templates, BUILD_FORMATS
 
 # Get access to logger
 log = logging.getLogger("ptxlogger")
 
 
 @contextmanager
-def working_directory(path: Path):
+def working_directory(path: Path) -> Generator:
     """
     Temporarily change the current working directory.
 
     Usage:
     with working_directory(path):
         do_things()   # working in the given path
     do_other_things() # back to original path
@@ -44,74 +47,88 @@
         yield
     finally:
         os.chdir(current_directory)
         log.debug(f"Successfully changed directory back to {current_directory}")
 
 
 # Grabs project directory based on presence of `project.ptx`
-def project_path(dirpath: Optional[Path] = None) -> Path:
+def project_path(dirpath: Optional[Path] = None) -> Optional[Path]:
     if dirpath is None:
         dirpath = Path().resolve()  # current directory
     if (dirpath / "project.ptx").is_file():
         # we're at the project root
         return dirpath
     if dirpath.parent == dirpath:
         # cannot ascend higher, no project found
         return None
     else:
         # check parent instead
         return project_path(dirpath=dirpath.parent)
 
 
-def project_xml(dirpath: t.Optional[Path] = None) -> Path:
+# Like above, but asserts if the project path can't be found.
+def project_path_found(dirpath: Optional[Path] = None) -> Path:
+    pp = project_path(dirpath)
+    assert pp is not None, "Invalid project path"
+    return pp
+
+
+def project_xml(dirpath: t.Optional[Path] = None) -> _ElementTree:
     if dirpath is None:
         dirpath = Path()  # current directory
-    if project_path(dirpath) is None:
+    pp = project_path(dirpath)
+    if pp is None:
         with templates.resource_path("project.ptx") as project_manifest:
             return ET.parse(project_manifest)
     else:
-        project_manifest = project_path(dirpath) / "project.ptx"
+        project_manifest = pp / "project.ptx"
         return ET.parse(project_manifest)
 
 
-def requirements_version(dirpath: Optional[Path] = None) -> str:
+def requirements_version(dirpath: Optional[Path] = None) -> Optional[str]:
     if dirpath is None:
         dirpath = Path()  # current directory
+    pp = project_path(dirpath)
+    if pp is None:
+        return None
     try:
-        with open(project_path(dirpath) / "requirements.txt", "r") as f:
+        with open(pp / "requirements.txt", "r") as f:
             for line in f.readlines():
                 if "pretext" or "pretextbook" in line:
                     return line.split("==")[1].strip()
     except Exception as e:
         log.debug("Could not read `requirements.txt`:")
         log.debug(e)
-        return None
+    return None
 
 
 def project_xml_string(dirpath: Optional[Path] = None) -> str:
     if dirpath is None:
         dirpath = Path()  # current directory
     return ET.tostring(project_xml(dirpath), encoding="unicode")
 
 
+# TODO: is this ever called?
 def target_xml(
     alias: t.Optional[str] = None, dirpath: t.Optional[Path] = None
-) -> ET.Element:
+) -> Optional[_Element]:
     if dirpath is None:
         dirpath = Path()  # current directory
     if alias is None:
         return project_xml().find("targets/target")  # first target
     xpath = f'targets/target[@name="{alias}"]'
-    matches = project_xml().xpath(xpath)
+    _matches = project_xml().xpath(xpath)
+    # Given that this is a project target, narrow the type of the match: ``xpath`` can return a wide variety of results.
+    matches = cast(List[_Element], _matches)
     if len(matches) == 0:
         log.info(
             f"No targets with alias {alias} found in project manifest file project.ptx."
         )
         return None
-    return project_xml().xpath(xpath)[0]
+    return matches[0]
 
 
 # check xml syntax
 def xml_syntax_is_valid(xmlfile: Path) -> bool:
     # parse xml
     try:
         source_xml = ET.parse(xmlfile)
@@ -176,73 +193,73 @@
             return json.load(f)["project_id"]
     except Exception:
         return None
 
 
 # watchdog handler for watching changes to source
 class HTMLRebuildHandler(watchdog.events.FileSystemEventHandler):
-    def __init__(self, callback):
+    def __init__(self, callback: Callable[[], None]):
         self.last_trigger_at = time.time() - 5
         self.callback = callback
 
-    def on_any_event(self, event):
+    def on_any_event(self, event: watchdog.events.FileSystemEvent) -> None:
         self.last_trigger_at = time.time()
 
         # only run callback once triggers halt for a second
-        def timeout_callback(handler):
+        def timeout_callback(handler: "HTMLRebuildHandler") -> None:
             time.sleep(1.5)
             if time.time() > handler.last_trigger_at + 1:
                 handler.last_trigger_at = time.time()
                 log.info("\nChanges to source detected.\n")
                 handler.callback()
 
         threading.Thread(target=timeout_callback, args=(self,)).start()
 
 
 # boilerplate to prevent overzealous caching by preview server, and
 # avoid port issues
-def binding_for_access(access="private"):
+def binding_for_access(access: str = "private") -> str:
     if access == "private":
         return "localhost"
     else:
         return "0.0.0.0"
 
 
-def url_for_access(access="private", port=8000):
+def url_for_access(access: str = "private", port: int = 8000) -> str:
     if access == "public":
         return f"http://{socket.gethostbyname(socket.gethostname())}:{port}"
     else:
         return f"http://localhost:{port}"
 
 
 def serve_forever(
-    directory: Path, access="private", port=8000, no_launch: bool = False
-):
+    directory: Path, access: str = "private", port: int = 8000, no_launch: bool = False
+) -> None:
     log.info(f"Now preparing local server to preview directory `{directory}`.")
     log.info(
         "  (Reminder: use `pretext deploy` to deploy your built project to a public"
     )
     log.info(
         "  GitHub Pages site that can be shared with readers who cannot access your"
     )
     log.info("  personal computer.)")
     log.info("")
     binding = binding_for_access(access)
 
     class RequestHandler(SimpleHTTPRequestHandler):
-        def __init__(self, *args, **kwargs):
+        def __init__(self, *args: Any, **kwargs: Any):
             super().__init__(*args, directory=directory.as_posix(), **kwargs)
 
         """HTTP request handler with no caching"""
 
-        def end_headers(self):
+        def end_headers(self) -> None:
             self.send_my_headers()
             SimpleHTTPRequestHandler.end_headers(self)
 
-        def send_my_headers(self):
+        def send_my_headers(self) -> None:
             self.send_header("Cache-Control", "no-cache, no-store, must-revalidate")
             self.send_header("Pragma", "no-cache")
             self.send_header("Expires", "0")
 
     class TCPServer(socketserver.TCPServer):
         allow_reuse_address = True
 
@@ -268,17 +285,17 @@
 
 
 def run_server(
     directory: Path,
     access: str,
     port: int,
     watch_directory: t.Optional[Path] = None,
-    watch_callback=lambda: None,
+    watch_callback: Callable[[], None] = lambda: None,
     no_launch: bool = False,
-):
+) -> None:
     threading.Thread(
         target=lambda: serve_forever(directory, access, port, no_launch), daemon=True
     ).start()
     if watch_directory is not None:
         log.info(f"\nWatching for changes in `{watch_directory}` ...\n")
         event_handler = HTMLRebuildHandler(watch_callback)
         observer = watchdog.observers.Observer()
@@ -302,37 +319,38 @@
 }
 
 
 def nstag(prefix: str, suffix: str) -> str:
     return "{" + NSMAP[prefix] + "}" + suffix
 
 
-def copy_custom_xsl(xsl_path: Path, output_dir: Path):
+def copy_custom_xsl(xsl_path: Path, output_dir: Path) -> None:
     """
     Copy relevant files that share a directory with `xsl_path`.
     Pre-processing the `.xsl` files to point to subdirectory for graceful deprecation.
     """
     xsl_dir = xsl_path.parent.resolve()
     output_dir = output_dir.resolve()
     log.debug(f"Copying all files in {xsl_dir} to {output_dir}")
     shutil.copytree(xsl_dir, output_dir, dirs_exist_ok=True)
     log.debug(f"Copying core XSL to {output_dir}/core")
     shutil.copytree(core.resources.path("xsl"), output_dir / "core")
 
 
-def check_executable(exec_name: str):
+def check_executable(exec_name: str) -> Optional[str]:
     try:
         exec_cmd = core.get_executable_cmd(exec_name)[0]
         log.debug(f"PTX-CLI: Executable command {exec_name} found at {exec_cmd}")
         return exec_cmd
     except OSError as e:
         log.debug(e)
+        return None
 
 
-def check_asset_execs(element, outformats=None):
+def check_asset_execs(element: str, outformats: Optional[List[str]] = None) -> None:
     # outformats is assumed to be a list of formats.
     if outformats is None:
         outformats = []
     # Note that asymptote is done via server, so doesn't require asy.  We could check for an internet connection here for that and webwork, etc.
     log.debug(f"trying to check assets for {element} and output format {outformats}")
     # Create list of executables needed based on output format
     required_execs = []
@@ -398,15 +416,20 @@
         log.critical(
             "Move to such a directory, use `pretext new` to create a new project, or `pretext init` to update existing project for use with the CLI."
         )
         return True
     return False
 
 
-def show_target_hints(target_format: str, project, task: str):
+def show_target_hints(
+    target_format: Optional[str],
+    # TODO: the type is ``project.Project``, but we can't ``import project`` due to circular imports.
+    project: Any,
+    task: str,
+) -> None:
     """
     This will give the user hints about why they have provided a bad target and make helpful suggestions for them to fix the problem.  We will only run this function when the target_name is not the name in any target in project.ptx.
     """
     # just in case this was called in the wrong place:
     if project.target(name=target_format) is not None:
         return
     # Otherwise continue with hints:
@@ -429,28 +452,28 @@
             )
     else:
         log.info(
             f"The available targets to {task} are named: {project.target_names()}.  Try to {task} on of those instead or edit your project.ptx manifest."
         )
 
 
-def npm_install():
+def npm_install() -> None:
     with working_directory(core.resources.path("script", "mjsre")):
         log.info("Attempting to install/update required node packages.")
         try:
             subprocess.run("npm install", shell=True)
         except Exception as e:
             log.critical(
                 "Unable to install required npm packages.  Please see the documentation."
             )
             log.critical(e)
             log.debug("", exc_info=True)
 
 
-def playwright_install():
+def playwright_install() -> None:
     """
     Run `playwright install` to ensure that its required browsers and tools are available to it.
     """
     try:
         log.info("Attempting to install/update required playwright packages.")
         subprocess.run("playwright install-deps", shell=True)
         subprocess.run("playwright install", shell=True)
@@ -459,22 +482,22 @@
         log.critical(
             "Unable to install required playwright packages.  Please see the documentation."
         )
         log.critical(e)
         log.debug("", exc_info=True)
 
 
-def remove_path(path: Path):
+def remove_path(path: Path) -> None:
     if path.is_file() or path.is_symlink():
         path.unlink()  # remove the file
     elif path.is_dir():
         shutil.rmtree(path)  # remove dir and all it contains
 
 
-def exit_command(mh):
+def exit_command(mh: logging.handlers.MemoryHandler) -> None:
     """
     Clean's up at the end of a run.
     Checks to see if anything (errors etc.) is in the memory handler.  If it is, reports that there are errors before the handler gets flushed.  Otherwise, adds a single blank line.
     """
     if len(mh.buffer) > 0:
         print("\n----------------------------------------------------")
         log.info("While running pretext, the following errors occurred:\n")
```

### Comparing `pretext-1.6.1.dev20230620/PKG-INFO` & `pretext-1.6.1.dev20230621/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230620
+Version: 1.6.1.dev20230621
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

