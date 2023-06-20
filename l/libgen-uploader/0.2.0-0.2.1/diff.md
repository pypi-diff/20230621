# Comparing `tmp/libgen_uploader-0.2.0.tar.gz` & `tmp/libgen_uploader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libgen_uploader-0.2.0.tar", max compression
+gzip compressed data, was "libgen_uploader-0.2.1.tar", max compression
```

## Comparing `libgen_uploader-0.2.0.tar` & `libgen_uploader-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1073 2021-03-28 20:22:43.869846 libgen_uploader-0.2.0/LICENSE
--rw-r--r--   0        0        0     2999 2021-03-28 20:22:43.869846 libgen_uploader-0.2.0/README.md
--rw-r--r--   0        0        0       60 2021-03-28 20:22:43.869846 libgen_uploader-0.2.0/libgen_uploader/__init__.py
--rw-r--r--   0        0        0     2402 2021-03-28 20:22:43.869846 libgen_uploader-0.2.0/libgen_uploader/__main__.py
--rw-r--r--   0        0        0      807 2021-03-28 20:22:43.869846 libgen_uploader-0.2.0/libgen_uploader/constants.py
--rw-r--r--   0        0        0     3009 2021-03-28 20:22:43.869846 libgen_uploader-0.2.0/libgen_uploader/helpers.py
--rw-r--r--   0        0        0    11656 2021-03-28 20:22:43.869846 libgen_uploader-0.2.0/libgen_uploader/libgen_uploader.py
--rw-r--r--   0        0        0      565 2021-03-28 20:22:43.869846 libgen_uploader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3810 2021-03-28 20:23:35.775101 libgen_uploader-0.2.0/setup.py
--rw-r--r--   0        0        0     3682 2021-03-28 20:23:35.775525 libgen_uploader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-20 22:02:29.885114 libgen_uploader-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3196 2023-06-20 22:02:29.885114 libgen_uploader-0.2.1/README.md
+-rw-r--r--   0        0        0       60 2023-06-20 22:02:29.885114 libgen_uploader-0.2.1/libgen_uploader/__init__.py
+-rw-r--r--   0        0        0     2429 2023-06-20 22:02:29.885114 libgen_uploader-0.2.1/libgen_uploader/__main__.py
+-rw-r--r--   0        0        0      807 2023-06-20 22:02:29.885114 libgen_uploader-0.2.1/libgen_uploader/constants.py
+-rw-r--r--   0        0        0     3008 2023-06-20 22:02:29.885114 libgen_uploader-0.2.1/libgen_uploader/helpers.py
+-rw-r--r--   0        0        0    12929 2023-06-20 22:02:29.885114 libgen_uploader-0.2.1/libgen_uploader/libgen_uploader.py
+-rw-r--r--   0        0        0      631 2023-06-20 22:02:29.889114 libgen_uploader-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 libgen_uploader-0.2.1/PKG-INFO
```

### Comparing `libgen_uploader-0.2.0/LICENSE` & `libgen_uploader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libgen_uploader-0.2.0/README.md` & `libgen_uploader-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -81,8 +81,18 @@
 )
 
 # custom, user-provided metadata (override default/fetched)
 from libgen_uploader import LibgenMetadata
 
 m = LibgenMetadata(title="new title", authors=["John Smith", "Jack Black"])
 u.upload_scitech("book.epub", metadata=m)
-```
+```
+
+## Donations
+
+Just in case you want to say thanks :)
+
+**BTC**: 3Kdyv75GpzwZ1b19QECwr3znsjSSkoRAVq
+
+**ETH**: 0x1Af2121BaF1795Ce3685893d89E5eC66E1DC510
+
+**DOGE**: DLdbw36tgSqK52njimJKsitCtVg1D4n8t9
```

### Comparing `libgen_uploader-0.2.0/libgen_uploader/__main__.py` & `libgen_uploader-0.2.1/libgen_uploader/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from libgen_uploader import LibgenUploader
 from returns.pipeline import is_successful
 
 
 def main(args):
-    u = LibgenUploader(metadata_source=args.metadata_source)
+    u = LibgenUploader(metadata_source=args.metadata_source, show_upload_progress=True)
 
     if args.scitech:
         result = u.upload_scitech(
             file_path=args.file, metadata_query=args.metadata_query
         )
     else:
         result = u.upload_fiction(
```

### Comparing `libgen_uploader-0.2.0/libgen_uploader/constants.py` & `libgen_uploader-0.2.1/libgen_uploader/constants.py`

 * *Files identical despite different names*

### Comparing `libgen_uploader-0.2.0/libgen_uploader/helpers.py` & `libgen_uploader-0.2.1/libgen_uploader/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     raise LibgenUploadException("Upload failed: unknown error")
 
 
 @safe
 def check_metadata_form_response(
     response: BeautifulSoup,
 ) -> str:
-
     if error_el := response.select_one(".error") or response.select_one(".form_error"):
         error_text = error_el.text.strip()
         raise LibgenUploadException(f"File save failed: {error_text}")
 
     if "successfully saved" in str(response).lower():
         return (
             response.find(lambda el: el.name == "div" and "to share" in el.text)
```

### Comparing `libgen_uploader-0.2.0/libgen_uploader/libgen_uploader.py` & `libgen_uploader-0.2.1/libgen_uploader/libgen_uploader.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 import logging
 import os
 
 from io import BytesIO
 from ntpath import basename
 from typing import List, Union
 
+import filetype
+
 # https://github.com/jmcarp/robobrowser/issues/93
 import werkzeug
 
-werkzeug.cached_property = werkzeug.utils.cached_property
+werkzeug.cached_property = werkzeug.utils.cached_property  # type: ignore
 
 from bs4 import BeautifulSoup
 from cerberus import schema
+from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 from returns.curry import partial
 from returns.result import Failure, Result, Success, safe
 from returns.pointfree import alt, bind, lash, map_
 from returns.pipeline import flow, is_successful
 from robobrowser import RoboBrowser
 from robobrowser.forms.form import Form
 from robobrowser.forms.fields import Submit
+from tqdm import tqdm
 
 from .constants import (
     LIBGEN_UPLOADER_VERSION,
     FICTION_UPLOAD_URL,
     SCITECH_UPLOAD_URL,
     UPLOAD_USERNAME,
     UPLOAD_PASSWORD,
@@ -74,25 +78,28 @@
             self.comment = comment
         else:
             logging.error(f"Metadata validation failed: {result}")
 
 
 class LibgenUploader:
     metadata_source = None
+    show_upload_progress: bool = False
 
-    def __init__(self, metadata_source: str = None):
+    def __init__(
+        self, *, metadata_source: str = None, show_upload_progress: bool = False
+    ):
         if metadata_source:
             self.metadata_source = metadata_source
 
+        self.show_upload_progress = show_upload_progress
         self._init_browser()
 
     def _init_browser(self):
         self._browser = RoboBrowser(
             parser="html.parser",
-            user_agent=f"libgen_uploader-v{LIBGEN_UPLOADER_VERSION}",
         )
         self._browser.session.auth = (UPLOAD_USERNAME, UPLOAD_PASSWORD)
 
     @safe
     def _submit_form_get_response(
         self,
         form: Form,
@@ -120,30 +127,61 @@
         if isinstance(file, str):
             if not os.path.isfile(file):
                 raise FileNotFoundError(f"Upload failed: {file} is not a file.")
 
             if file.endswith(".epub") and epub_has_drm(file):
                 raise LibgenUploadException("Your .epub file seems to have DRM.")
 
-            logging.info(f"Selected file {basename(file)}")
             return file
 
     @safe
-    def _upload_file(self, file: Union[str, bytes]) -> BeautifulSoup:
-        form = self._browser.get_form()
+    def _upload_file(self, file: Union[str, bytes], library: str) -> BeautifulSoup:
+        if library == "scitech":
+            self._init_browser()
+            upload_url = SCITECH_UPLOAD_URL
+        elif library == "fiction":
+            self._init_browser()
+            upload_url = FICTION_UPLOAD_URL
+        else:
+            raise ValueError(f"Unknown library to upload to: {library}")
+
+        self._browser.open(upload_url)
+
         if isinstance(file, str):
-            form["file"].value = open(file, mode="rb")
+            encoder = MultipartEncoder(
+                fields={"file": (basename(file), open(file, "rb"))}
+            )
         elif isinstance(file, bytes):
-            form["file"].value = BytesIO(file)
+            file_ext = filetype.guess_extension(file)
+            encoder = MultipartEncoder(
+                fields={"file": (f"book.{file_ext}", BytesIO(file))}
+            )
 
-        response = self._submit_form_get_response(form)
-        if is_successful(response):
-            return response.unwrap()
+        with tqdm(
+            desc=basename(file) if isinstance(file, str) else str(file),
+            total=encoder.len,
+            disable=self.show_upload_progress is False,
+            dynamic_ncols=True,
+            unit="B",
+            unit_scale=True,
+            unit_divisor=1024,
+        ) as bar:
+            monitor = MultipartEncoderMonitor(
+                encoder, lambda monitor: bar.update(monitor.bytes_read - bar.n)
+            )
+            session = self._browser.session
+            response = session.post(
+                upload_url,
+                data=monitor,
+                headers={"Content-Type": monitor.content_type},
+            )
+            response.raise_for_status()
+            self._browser._update_state(response)
 
-        raise response.failure()
+        return BeautifulSoup(response.text, "html.parser")
 
     @safe
     def _fetch_metadata_from_query(
         self, form, *, metadata_source: str, metadata_query: str
     ) -> Form:
         form["metadata_source"].value = metadata_source
         form["metadata_query"].value = metadata_query
@@ -281,27 +319,27 @@
                 form = self._browser.get_form()
                 form["asin"].value = ""
                 return self._submit_and_check_form(form)
 
         # failed to recover, re-raise
         return Failure(exception)
 
-    def _upload(self, **kwargs) -> Result[str, Exception]:
+    def _upload(self, library: str, **kwargs) -> Result[str, Exception]:
         if [kwargs["metadata_query"], kwargs["metadata_source"]].count(None) == 1:
             if kwargs["metadata_source"] is None and self.metadata_source is not None:
                 kwargs["metadata_source"] = self.metadata_source
             else:
                 raise LibgenUploadException(
                     "Both metadata_source and metadata_query are required to fetch metadata."
                 )
 
         upload_url: Result[str, Exception] = flow(
             kwargs["file_path"],
             self._validate_file,
-            bind(self._upload_file),
+            bind(partial(self._upload_file, library=library)),
             bind(check_upload_form_response),
             map_(lambda *_: self._browser.get_form()),  # type: ignore
             bind(
                 partial(
                     self._fetch_metadata,
                     metadata_query=kwargs["metadata_query"],
                     metadata_source=kwargs["metadata_source"],
@@ -324,32 +362,30 @@
         self,
         file_path: Union[str, bytes],
         *,
         metadata: LibgenMetadata = None,
         metadata_source: str = None,
         metadata_query: Union[str, List] = None,
     ) -> Result[str, Exception]:
-        self._init_browser()
-        self._browser.open(FICTION_UPLOAD_URL)
         return self._upload(
             file_path=file_path,
+            library="fiction",
             metadata=metadata,
             metadata_source=metadata_source,
             metadata_query=metadata_query,
         )
 
     def upload_scitech(
         self,
         file_path: Union[str, bytes],
         *,
         metadata: LibgenMetadata = None,
         metadata_source: str = None,
         metadata_query: Union[str, List] = None,
     ) -> Result[str, Exception]:
-        self._init_browser()
-        self._browser.open(SCITECH_UPLOAD_URL)
         return self._upload(
             file_path=file_path,
+            library="scitech",
             metadata=metadata,
             metadata_source=metadata_source,
             metadata_query=metadata_query,
         )
```

### Comparing `libgen_uploader-0.2.0/pyproject.toml` & `libgen_uploader-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [tool.poetry]
 name = "libgen_uploader"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Library Genesis ebook uploader"
 authors = ["Francesco Truzzi <francesco@truzzi.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ftruzzi/libgen_uploader"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 robobrowser = "^0.5.3"
 Cerberus = "^1.3.2"
 returns = "0.16.0"
+tqdm = "^4.59.0"
+requests-toolbelt = "^1.0.0"
+filetype = "^1.0.7"
 
 [tool.poetry.dev-dependencies]
-black = "^20.8b1"
+black = "^23.3.0"
 pytest = "^6.2.2"
 pytest-recording = "^0.11.0"
 mypy = "^0.812"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `libgen_uploader-0.2.0/setup.py` & `libgen_uploader-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,122 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: libgen-uploader
+Version: 0.2.1
+Summary: A Library Genesis ebook uploader
+Home-page: https://github.com/ftruzzi/libgen_uploader
+License: MIT
+Author: Francesco Truzzi
+Author-email: francesco@truzzi.me
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Cerberus (>=1.3.2,<2.0.0)
+Requires-Dist: filetype (>=1.0.7,<2.0.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
+Requires-Dist: returns (==0.16.0)
+Requires-Dist: robobrowser (>=0.5.3,<0.6.0)
+Requires-Dist: tqdm (>=4.59.0,<5.0.0)
+Project-URL: Repository, https://github.com/ftruzzi/libgen_uploader
+Description-Content-Type: text/markdown
+
+_A Library Genesis ebook uploader._
+
+**This library is to be considered unstable/beta until v1.0.0. API may change until then.**
+
+## Installation
+
+```bash
+pip install libgen-uploader
+```
+
+## Usage from command-line
+
+```bash
+python -m libgen_uploader (--scitech|--fiction) [args] book.epub
+```
+
+Optional arguments:
+```
+--metadata-source {local,amazon_us,amazon_uk,amazon_de,amazon_fr,amazon_it,amazon_es,amazon_jp,bl,douban,goodreads,google_books,loc,rsl,worldcat}
+    Source to fetch book metadata from
+
+--metadata-query METADATA_QUERY
+    Metadata query for selected source (supports multiple, comma-separated)
+
+-d, --debug
+    Activate debug logging
+```
+
+## Usage as library
+
+This library uses [returns](https://github.com/dry-python/returns), and returns [Result containers](https://returns.readthedocs.io/en/latest/pages/result.html) which can either contain a success value or a failure/exception. Exception values are returned, not raised, so you can handle them as you wish and avoid wide `try/except` blocks or program crashes due to unforeseen exceptions.
+
+### Uploading books
+
+Two methods are exposed for uploading books: `upload_scitech` and `upload_fiction`.
+
+```python
+from libgen_uploader import LibgenUploader
+from returns.pipeline import is_successful
+
+u = LibgenUploader()
+
+result = u.upload_fiction("book.epub")
+if is_successful(result):
+    upload_url = result.unwrap() # type: str
+else:
+    failure = result.failure() # type: Exception
+```
+
+### Fetching metadata
+
+Metadata support is not complete yet. The default metadata are the one contained in the book itself. You can then fetch additional metadata from the sources supported by the Library Genesis upload form, namely:
+
+- Other Library Genesis record (`"local"`)
+- Amazon US/UK/DE/FR/IT/ES/JP (`"amazon_us"`, `"amazon_uk"`, `"amazon_de"`, `"amazon_fr"`, `"amazon_it"`, `"amazon_es"`, `"amazon_jp"`)
+- British Library (`"bl"`)
+- Douban.com (`"douban"`)
+- Goodreads (`"goodreads"`)
+- Google Books (`"google_books"`)
+- Library of Congress (`"loc"`)
+- Russian State Library (`"rsl"`)
+- WorldCat (`"worldcat"`)
+
+Any fetched metadata completely replaces all metadata contained in the ebook itself (this is how the upload form works), and any custom (user-provided) metadata overrides the default/fetched ones.
+
+```python
+# use metadata contained in the book
+u = LibgenUploader()
+u.upload_scitech("book.epub")
+
+# session-wide metadata source
+u = LibgenUploader(metadata_source="amazon_it")
+u.upload_scitech("book.epub", metadata_query="9788812312312")
+
+# book-level metadata source
+u = LibgenUploader()
+u.upload_scitech(
+    "book.epub",
+    metadata_source="amazon_it",
+    metadata_query=["9788812312312", "another_isbn"] # you can pass an array of values in case the first ones don't return results
+)
+
+# custom, user-provided metadata (override default/fetched)
+from libgen_uploader import LibgenMetadata
+
+m = LibgenMetadata(title="new title", authors=["John Smith", "Jack Black"])
+u.upload_scitech("book.epub", metadata=m)
+```
+
+## Donations
 
-packages = \
-['libgen_uploader']
+Just in case you want to say thanks :)
 
-package_data = \
-{'': ['*']}
+**BTC**: 3Kdyv75GpzwZ1b19QECwr3znsjSSkoRAVq
 
-install_requires = \
-['Cerberus>=1.3.2,<2.0.0', 'returns==0.16.0', 'robobrowser>=0.5.3,<0.6.0']
-
-setup_kwargs = {
-    'name': 'libgen-uploader',
-    'version': '0.2.0',
-    'description': 'A Library Genesis ebook uploader',
-    'long_description': '_A Library Genesis ebook uploader._\n\n**This library is to be considered unstable/beta until v1.0.0. API may change until then.**\n\n## Installation\n\n```bash\npip install libgen-uploader\n```\n\n## Usage from command-line\n\n```bash\npython -m libgen_uploader (--scitech|--fiction) [args] book.epub\n```\n\nOptional arguments:\n```\n--metadata-source {local,amazon_us,amazon_uk,amazon_de,amazon_fr,amazon_it,amazon_es,amazon_jp,bl,douban,goodreads,google_books,loc,rsl,worldcat}\n    Source to fetch book metadata from\n\n--metadata-query METADATA_QUERY\n    Metadata query for selected source (supports multiple, comma-separated)\n\n-d, --debug\n    Activate debug logging\n```\n\n## Usage as library\n\nThis library uses [returns](https://github.com/dry-python/returns), and returns [Result containers](https://returns.readthedocs.io/en/latest/pages/result.html) which can either contain a success value or a failure/exception. Exception values are returned, not raised, so you can handle them as you wish and avoid wide `try/except` blocks or program crashes due to unforeseen exceptions.\n\n### Uploading books\n\nTwo methods are exposed for uploading books: `upload_scitech` and `upload_fiction`.\n\n```python\nfrom libgen_uploader import LibgenUploader\nfrom returns.pipeline import is_successful\n\nu = LibgenUploader()\n\nresult = u.upload_fiction("book.epub")\nif is_successful(result):\n    upload_url = result.unwrap() # type: str\nelse:\n    failure = result.failure() # type: Exception\n```\n\n### Fetching metadata\n\nMetadata support is not complete yet. The default metadata are the one contained in the book itself. You can then fetch additional metadata from the sources supported by the Library Genesis upload form, namely:\n\n- Other Library Genesis record (`"local"`)\n- Amazon US/UK/DE/FR/IT/ES/JP (`"amazon_us"`, `"amazon_uk"`, `"amazon_de"`, `"amazon_fr"`, `"amazon_it"`, `"amazon_es"`, `"amazon_jp"`)\n- British Library (`"bl"`)\n- Douban.com (`"douban"`)\n- Goodreads (`"goodreads"`)\n- Google Books (`"google_books"`)\n- Library of Congress (`"loc"`)\n- Russian State Library (`"rsl"`)\n- WorldCat (`"worldcat"`)\n\nAny fetched metadata completely replaces all metadata contained in the ebook itself (this is how the upload form works), and any custom (user-provided) metadata overrides the default/fetched ones.\n\n```python\n# use metadata contained in the book\nu = LibgenUploader()\nu.upload_scitech("book.epub")\n\n# session-wide metadata source\nu = LibgenUploader(metadata_source="amazon_it")\nu.upload_scitech("book.epub", metadata_query="9788812312312")\n\n# book-level metadata source\nu = LibgenUploader()\nu.upload_scitech(\n    "book.epub",\n    metadata_source="amazon_it",\n    metadata_query=["9788812312312", "another_isbn"] # you can pass an array of values in case the first ones don\'t return results\n)\n\n# custom, user-provided metadata (override default/fetched)\nfrom libgen_uploader import LibgenMetadata\n\nm = LibgenMetadata(title="new title", authors=["John Smith", "Jack Black"])\nu.upload_scitech("book.epub", metadata=m)\n```',
-    'author': 'Francesco Truzzi',
-    'author_email': 'francesco@truzzi.me',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ftruzzi/libgen_uploader',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+**ETH**: 0x1Af2121BaF1795Ce3685893d89E5eC66E1DC510
 
-
-setup(**setup_kwargs)
+**DOGE**: DLdbw36tgSqK52njimJKsitCtVg1D4n8t9
```

