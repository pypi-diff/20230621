# Comparing `tmp/iscc_sdk-0.5.6.tar.gz` & `tmp/iscc_sdk-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iscc_sdk-0.5.6.tar", max compression
+gzip compressed data, was "iscc_sdk-0.5.7.tar", max compression
```

## Comparing `iscc_sdk-0.5.6.tar` & `iscc_sdk-0.5.7.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0      866 2023-04-28 18:57:50.903193 iscc_sdk-0.5.6/iscc_sdk/__init__.py
--rw-r--r--   0        0        0     3859 2023-04-28 18:56:24.488929 iscc_sdk-0.5.6/iscc_sdk/audio.py
--rw-r--r--   0        0        0       99 2023-04-28 18:56:24.488929 iscc_sdk-0.5.6/iscc_sdk/compat.py
--rw-r--r--   0        0        0      897 2023-04-28 18:56:24.489929 iscc_sdk-0.5.6/iscc_sdk/docx_.py
--rw-r--r--   0        0        0     1491 2023-04-28 18:56:24.489929 iscc_sdk-0.5.6/iscc_sdk/epub.py
--rw-r--r--   0        0        0      166 2023-04-28 18:56:24.489929 iscc_sdk-0.5.6/iscc_sdk/exceptions.py
--rw-r--r--   0        0        0     8091 2023-04-28 18:56:24.490929 iscc_sdk-0.5.6/iscc_sdk/image.py
--rw-r--r--   0        0        0      683 2023-04-28 18:56:24.490929 iscc_sdk-0.5.6/iscc_sdk/install.py
--rw-r--r--   0        0        0     1274 2023-04-28 18:56:24.490929 iscc_sdk-0.5.6/iscc_sdk/ipfs.py
--rw-r--r--   0        0        0     6772 2023-04-28 18:56:24.491929 iscc_sdk-0.5.6/iscc_sdk/main.py
--rw-r--r--   0        0        0     9258 2023-04-28 18:56:24.491929 iscc_sdk-0.5.6/iscc_sdk/mediatype.py
--rw-r--r--   0        0        0     1898 2023-04-28 18:56:24.491929 iscc_sdk-0.5.6/iscc_sdk/metadata.py
--rw-r--r--   0        0        0     1905 2023-04-28 18:56:24.492930 iscc_sdk-0.5.6/iscc_sdk/monkeys.py
--rw-r--r--   0        0        0     3021 2023-04-28 18:56:24.492930 iscc_sdk-0.5.6/iscc_sdk/mp7.py
--rw-r--r--   0        0        0     2720 2023-04-28 18:56:24.492930 iscc_sdk-0.5.6/iscc_sdk/options.py
--rw-r--r--   0        0        0     2502 2023-04-28 18:56:24.492930 iscc_sdk-0.5.6/iscc_sdk/pdf.py
--rw-r--r--   0        0        0     5761 2023-04-28 18:56:24.493929 iscc_sdk-0.5.6/iscc_sdk/text.py
--rw-r--r--   0        0        0      684 2023-04-28 18:56:24.493929 iscc_sdk-0.5.6/iscc_sdk/thumbnail.py
--rw-r--r--   0        0        0    21133 2023-04-28 18:57:50.904193 iscc_sdk-0.5.6/iscc_sdk/tools.py
--rw-r--r--   0        0        0     5802 2023-04-28 18:56:24.494930 iscc_sdk-0.5.6/iscc_sdk/video.py
--rw-r--r--   0        0        0    11340 2022-03-29 10:37:56.086305 iscc_sdk-0.5.6/LICENSE
--rw-r--r--   0        0        0     3259 2023-04-28 18:57:50.906193 iscc_sdk-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     3392 2023-04-28 18:57:50.902194 iscc_sdk-0.5.6/README.md
--rw-r--r--   0        0        0     6025 1970-01-01 00:00:00.000000 iscc_sdk-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      895 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/__init__.py
+-rw-r--r--   0        0        0     4346 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/audio.py
+-rw-r--r--   0        0        0     5183 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/cli.py
+-rw-r--r--   0        0        0       99 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/compat.py
+-rw-r--r--   0        0        0      897 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/docx_.py
+-rw-r--r--   0        0        0     1491 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/epub.py
+-rw-r--r--   0        0        0      166 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/exceptions.py
+-rw-r--r--   0        0        0     8091 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/image.py
+-rw-r--r--   0        0        0      683 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/install.py
+-rw-r--r--   0        0        0     1274 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/ipfs.py
+-rw-r--r--   0        0        0     7218 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/main.py
+-rw-r--r--   0        0        0     9258 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/mediatype.py
+-rw-r--r--   0        0        0     1898 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/metadata.py
+-rw-r--r--   0        0        0     1905 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/monkeys.py
+-rw-r--r--   0        0        0     3021 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/mp7.py
+-rw-r--r--   0        0        0     2886 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/options.py
+-rw-r--r--   0        0        0     2502 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/pdf.py
+-rw-r--r--   0        0        0     5761 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/text.py
+-rw-r--r--   0        0        0      684 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/thumbnail.py
+-rw-r--r--   0        0        0    21133 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/tools.py
+-rw-r--r--   0        0        0      602 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/utils.py
+-rw-r--r--   0        0        0     6067 2023-06-21 15:10:58.086653 iscc_sdk-0.5.7/iscc_sdk/video.py
+-rw-r--r--   0        0        0    11340 2022-03-29 10:37:56.086305 iscc_sdk-0.5.7/LICENSE
+-rw-r--r--   0        0        0     3343 2023-06-21 15:10:58.024147 iscc_sdk-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3562 2023-06-21 15:10:58.024147 iscc_sdk-0.5.7/README.md
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 iscc_sdk-0.5.7/PKG-INFO
```

### Comparing `iscc_sdk-0.5.6/iscc_sdk/__init__.py` & `iscc_sdk-0.5.7/iscc_sdk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ISCC - Software Development Kit."""
 import os
 from platformdirs import PlatformDirs
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 APP_NAME = "iscc-sdk"
 APP_AUTHOR = "iscc"
 dirs = PlatformDirs(appname=APP_NAME, appauthor=APP_AUTHOR)
 os.makedirs(dirs.user_data_dir, exist_ok=True)
 os.environ["LOGURU_AUTOINIT"] = "False"
 
 
@@ -25,7 +25,8 @@
 from iscc_sdk.mp7 import *
 from iscc_sdk.exceptions import *
 from iscc_sdk.metadata import *
 from iscc_sdk.pdf import *
 from iscc_sdk.epub import *
 from iscc_sdk.docx_ import *
 from iscc_sdk.thumbnail import *
+from iscc_sdk.utils import *
```

### Comparing `iscc_sdk-0.5.6/iscc_sdk/audio.py` & `iscc_sdk-0.5.7/iscc_sdk/audio.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,47 +71,58 @@
     """
     Extract metadata from audio file.
 
     :param str fp: Filepath to audio file.
     :return: Metadata mapped to IsccMeta schema
     :rtype: dict
     """
-    try:
-        obj = taglib.File(fp)
-    except OSError as e:
-        log.error(f"Failed metadata extraction for {basename(fp)}: {e}")
-        return {}
-    meta = dict(obj.tags)
     mapped = dict()
     done = set()
+
+    try:
+        obj = taglib.File(fp)
+        meta = dict(obj.tags)
+        mapped["duration"] = obj.length
+        obj.close()
+    except OSError as e:  # pragma: no cover
+        # This is a workaround for the issue that taglib requires exclusive access even for reading.
+        log.warning(f"Create tempfile for taglib access {basename(fp)}: {e}")
+        try:
+            with idk.TempFile(fp) as tmp_path:
+                obj = taglib.File(tmp_path.as_posix())
+                meta = dict(obj.tags)
+                mapped["duration"] = obj.length
+                obj.close()
+        except Exception as e:
+            log.warning(f"Failed metadata extraction for {basename(fp)}: {e}")
+            return mapped
+
     for tag, mapped_field in AUDIO_META_MAP.items():
         if mapped_field in done:
             continue
         value = meta.get(tag)
         if value:
             log.debug(f"Mapping audio metadata: {tag} -> {mapped_field} -> {value[0]}")
             mapped[mapped_field] = value[0]
             done.add(mapped_field)
-    mapped["duration"] = obj.length
     # Todo - add bitrate, channels, samplerate to iscc-schema
     # mapped["bitrate"] = obj.bitrate
     # mapped["channels"] = obj.channels
     # mapped["samplerate"] = obj.sampleRate
-    obj.close()
     return mapped
 
 
 def audio_meta_embed(fp, meta):
     # type: (str, idk.IsccMeta) -> str
     """
     Embed metadata into a copy of the audio file.
 
     :param str fp: Filepath to source audio file
     :param IsccMeta meta: Metadata to embed into audio file
-    :return: Filepath to new video file with updated metadata
+    :return: Filepath to new audio file with updated metadata
     :rtype: str
     """
     tdir = tempfile.mkdtemp()
     tfile = shutil.copy(fp, tdir)
     obj = taglib.File(tfile)
     if meta.name:
         obj.tags["TITLE"] = [meta.name]
```

### Comparing `iscc_sdk-0.5.6/iscc_sdk/docx_.py` & `iscc_sdk-0.5.7/iscc_sdk/docx_.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/epub.py` & `iscc_sdk-0.5.7/iscc_sdk/epub.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/image.py` & `iscc_sdk-0.5.7/iscc_sdk/image.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/install.py` & `iscc_sdk-0.5.7/iscc_sdk/install.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/ipfs.py` & `iscc_sdk-0.5.7/iscc_sdk/ipfs.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/main.py` & `iscc_sdk-0.5.7/iscc_sdk/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """*SDK main top-level functions*."""
+from concurrent.futures import ThreadPoolExecutor
 from os.path import basename
-
 from PIL import Image
 import iscc_core as ic
 import iscc_sdk as idk
 
 
 __all__ = [
     "code_iscc",
@@ -27,19 +27,28 @@
     The ISCC-CODE is a composite of Meta, Content, Data and Instance Codes.
 
     :param str fp: Filepath used for ISCC-CODE creation.
     :return: ISCC metadata including ISCC-CODE and merged metadata from ISCC-UNITs.
     :rtype: IsccMeta
     """
 
-    # Generate ISCC-UNITs
-    instance = code_instance(fp)
-    data = code_data(fp)
-    content = code_content(fp)
-    meta = code_meta(fp)
+    # Generate ISCC-UNITs in parallel
+    with ThreadPoolExecutor() as executor:
+        instance = executor.submit(code_instance, fp)
+        data = executor.submit(code_data, fp)
+        content = executor.submit(code_content, fp)
+        meta = executor.submit(code_meta, fp)
+
+    # Wait for all futures to complete and retrieve their results
+    instance, data, content, meta = (
+        instance.result(),
+        data.result(),
+        content.result(),
+        meta.result(),
+    )
 
     # Compose ISCC-CODE
     iscc_code = ic.gen_iscc_code_v0([meta.iscc, content.iscc, data.iscc, instance.iscc])
 
     # Merge ISCC Metadata
     iscc_meta = dict(filename=basename(fp))
     iscc_meta.update(instance.dict())
@@ -196,16 +205,17 @@
     :rtype: IsccMeta
     """
     meta = dict()
 
     if idk.sdk_opts.extract_metadata:
         meta = idk.video_meta_extract(fp)
         thumbnail_image = idk.video_thumbnail(fp)
-        thumbnail_durl = idk.image_to_data_url(thumbnail_image)
-        meta["thumbnail"] = thumbnail_durl
+        if thumbnail_image is not None:
+            thumbnail_durl = idk.image_to_data_url(thumbnail_image)
+            meta["thumbnail"] = thumbnail_durl
 
     features = idk.video_features_extract(fp)
     code_obj = ic.gen_video_code_v0(features, bits=idk.core_opts.video_bits)
     meta.update(code_obj)
 
     return idk.IsccMeta.construct(**meta)
```

### Comparing `iscc_sdk-0.5.6/iscc_sdk/mediatype.py` & `iscc_sdk-0.5.7/iscc_sdk/mediatype.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/metadata.py` & `iscc_sdk-0.5.7/iscc_sdk/metadata.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/monkeys.py` & `iscc_sdk-0.5.7/iscc_sdk/monkeys.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/mp7.py` & `iscc_sdk-0.5.7/iscc_sdk/mp7.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/options.py` & `iscc_sdk-0.5.7/iscc_sdk/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,19 @@
     )
 
     video_fps: int = Field(
         5,
         description="ISCC_SDK_VIDEO_FPS - Frames per second to process for video hash (ignored when 0).",
     )
 
+    video_store_mp7sig: bool = Field(
+        False,
+        description="ISCC_SDK_VIDEO_STORE_MP7SIG - Store extracted MP7 Video as <videofile>.iscc.mp7sig",
+    )
+
     @validator("image_max_pixels")
     def set_pillow(cls, v):
         Image.MAX_IMAGE_PIXELS = v
         return v
 
 
 sdk_opts = SdkOptions()
```

### Comparing `iscc_sdk-0.5.6/iscc_sdk/pdf.py` & `iscc_sdk-0.5.7/iscc_sdk/pdf.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/text.py` & `iscc_sdk-0.5.7/iscc_sdk/text.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/thumbnail.py` & `iscc_sdk-0.5.7/iscc_sdk/thumbnail.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/tools.py` & `iscc_sdk-0.5.7/iscc_sdk/tools.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/iscc_sdk/video.py` & `iscc_sdk-0.5.7/iscc_sdk/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """*Video handling module*"""
 import os
-from typing import Tuple, List
-
+from typing import Tuple, List, Optional
 from loguru import logger as log
 import io
-import subprocess
 import sys
 import tempfile
 from os.path import join, basename
 from pathlib import Path
 from secrets import token_hex
 from PIL import Image, ImageEnhance
 import iscc_sdk as idk
@@ -155,15 +153,15 @@
         videofile,
     ]
     idk.run_ffmpeg(args)
     return videofile
 
 
 def video_thumbnail(fp):
-    # type: (str) -> Image.Image
+    # type: (str) -> Optional[Image.Image]
     """
     Create a thumbnail for a video.
 
     :param str fp: Filepath to video file.
     :return: Raw PNG byte data
     :rtype: bytes
     """
@@ -178,16 +176,19 @@
         "1",
         "-c:v",
         "png",
         "-f",
         "image2pipe",
         "-",
     ]
-
-    result = idk.run_ffmpeg(args)
+    try:
+        result = idk.run_ffmpeg(args)
+    except Exception as e:
+        log.error(f"Failed video thumbnail extraction: {e}")
+        return None
     img_obj = Image.open(io.BytesIO(result.stdout))
     return ImageEnhance.Sharpness(img_obj.convert("RGB")).enhance(1.4)
 
 
 def video_features_extract(fp):
     # type: (str) -> List[Tuple[int, ...]]
     """
@@ -195,14 +196,20 @@
 
     :param str fp: Filepath to video file.
     :return: A sequence of frame signatures.
     :rtype: Sequence[Tuple[int, ...]]
     """
     # TODO use confidence value to improve simililarity hash.
     sig = video_mp7sig_extract(fp)
+
+    if idk.sdk_opts.video_store_mp7sig:
+        outp = fp + ".iscc.mp7sig"
+        with open(outp, "wb") as outf:
+            outf.write(sig)
+
     frames = idk.read_mp7_signature(sig)
     return [tuple(frame.vector.tolist()) for frame in frames]
 
 
 def video_mp7sig_extract(fp):
     # type: (str) -> bytes
     """Extract MPEG-7 Video Signature.
```

### Comparing `iscc_sdk-0.5.6/LICENSE` & `iscc_sdk-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.6/pyproject.toml` & `iscc_sdk-0.5.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iscc-sdk"
-version = "0.5.6"
+version = "0.5.7"
 description = "SDK for creating ISCCs (International Standard Content Codes)"
 authors = ["Titusz <tp@py7.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://sdk.iscc.codes"
 repository = "https://github.com/iscc/iscc-sdk"
 keywords=["iscc", "identifier", "media", "content", "hash", "blockchain", "similarity"]
@@ -33,46 +33,53 @@
 [tool.poetry.urls]
 "Changelog" = "https://sdk.iscc.codes/changelog"
 "Coverage" = "https://app.codecov.io/gh/iscc/iscc-sdk"
 "Bug Tracker" = "https://github.com/iscc/iscc-sdk/issues"
 "Twitter" = "https://twitter.com/iscc_foundation"
 "Donate" = "https://iscc.foundation/support"
 
+
+[tool.poetry.scripts]
+idk = 'iscc_sdk.cli:app'
+
+
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-cython = "^0.29.33"
-iscc-core = "^1.0.3"
+cython = "^0.29"
+iscc-core = "^1.0"
 iscc-schema = "^0.4"
 python-magic-bin = { version = "^0.4", markers = "sys_platform == 'win32' or (sys_platform == 'darwin' and platform_machine == 'x86_64')" }
 python-magic = { version = "^0.4", markers = "sys_platform == 'linux' or (sys_platform == 'darwin' and platform_machine == 'arm64')" }
 install-jdk = "^0.3"
 platformdirs = "^3.1"
 jmespath = "^1.0"
 Pillow = "^9.0"
 pytaglib = "^2.0"
 numpy = "^1.22"
 pymupdf = "^1.21"
 ebookmeta = "^1.2"
 python-docx = "^0.8"
+typer = {extras = ["all"], version = "^0.9.0"}
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 black = "^22.1"
 coverage = "^7.0"
 pytest-cov = "^4.0"
 poethepoet = "^0.16"
 bandit = "^1.7"
 mkdocs-material = "^9.1"
-mkdocstrings = {extras = ["python"], version = "^0.20"}
+mkdocstrings-python = "<1.1"
 iscc-samples = "^0.6"
 codetiming = "^1.3"
 mdformat = "*"
 mdformat_admon = "*"
 mdformat_tables = "*"
+griffe = "<0.27.4"
 
 [tool.black]
 skip-string-normalization = false
 line-length = 100
 target-version = ['py37']
 
 [tool.coverage.run]
```

### Comparing `iscc_sdk-0.5.6/README.md` & `iscc_sdk-0.5.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,26 @@
 
 ```python
 import iscc_sdk as idk
 
 print(idk.code_iscc("/path/to/mediafile.jpg"))
 ```
 
+Using the CLI tool to create an ISCC-CODE
+
+```shell
+idk create /path/to/mediafile.jpg
+```
+
+Batch creation of ISCC-CODEs
+
+```shell
+idk batch /folder_with_media_files
+```
+
 ## Documentation
 
 <https://sdk.iscc.codes>
 
 ## Troubleshooting
 
 On Linux and MacOS you might need to install taglib as a prerequisite. On Ubuntu, Mint and other
```

### Comparing `iscc_sdk-0.5.6/PKG-INFO` & `iscc_sdk-0.5.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iscc-sdk
-Version: 0.5.6
+Version: 0.5.7
 Summary: SDK for creating ISCCs (International Standard Content Codes)
 Home-page: https://sdk.iscc.codes
 License: Apache-2.0
 Keywords: iscc,identifier,media,content,hash,blockchain,similarity
 Author: Titusz
 Author-email: tp@py7.de
 Requires-Python: >=3.8,<4.0
@@ -29,27 +29,28 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Indexing
 Requires-Dist: Pillow (>=9.0,<10.0)
-Requires-Dist: cython (>=0.29.33,<0.30.0)
+Requires-Dist: cython (>=0.29,<0.30)
 Requires-Dist: ebookmeta (>=1.2,<2.0)
 Requires-Dist: install-jdk (>=0.3,<0.4)
-Requires-Dist: iscc-core (>=1.0.3,<2.0.0)
+Requires-Dist: iscc-core (>=1.0,<2.0)
 Requires-Dist: iscc-schema (>=0.4,<0.5)
 Requires-Dist: jmespath (>=1.0,<2.0)
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: platformdirs (>=3.1,<4.0)
 Requires-Dist: pymupdf (>=1.21,<2.0)
 Requires-Dist: pytaglib (>=2.0,<3.0)
 Requires-Dist: python-docx (>=0.8,<0.9)
 Requires-Dist: python-magic (>=0.4,<0.5) ; sys_platform == "linux" or sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: python-magic-bin (>=0.4,<0.5) ; sys_platform == "win32" or sys_platform == "darwin" and platform_machine == "x86_64"
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/iscc/iscc-sdk/issues
 Project-URL: Changelog, https://sdk.iscc.codes/changelog
 Project-URL: Coverage, https://app.codecov.io/gh/iscc/iscc-sdk
 Project-URL: Donate, https://iscc.foundation/support
 Project-URL: Repository, https://github.com/iscc/iscc-sdk
 Project-URL: Twitter, https://twitter.com/iscc_foundation
 Description-Content-Type: text/markdown
@@ -109,14 +110,26 @@
 
 ```python
 import iscc_sdk as idk
 
 print(idk.code_iscc("/path/to/mediafile.jpg"))
 ```
 
+Using the CLI tool to create an ISCC-CODE
+
+```shell
+idk create /path/to/mediafile.jpg
+```
+
+Batch creation of ISCC-CODEs
+
+```shell
+idk batch /folder_with_media_files
+```
+
 ## Documentation
 
 <https://sdk.iscc.codes>
 
 ## Troubleshooting
 
 On Linux and MacOS you might need to install taglib as a prerequisite. On Ubuntu, Mint and other
```

