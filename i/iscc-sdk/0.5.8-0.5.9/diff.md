# Comparing `tmp/iscc_sdk-0.5.8.tar.gz` & `tmp/iscc_sdk-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iscc_sdk-0.5.8.tar", max compression
+gzip compressed data, was "iscc_sdk-0.5.9.tar", max compression
```

## Comparing `iscc_sdk-0.5.8.tar` & `iscc_sdk-0.5.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      895 2023-06-21 19:32:14.804988 iscc_sdk-0.5.8/iscc_sdk/__init__.py
--rw-r--r--   0        0        0     4346 2023-06-21 19:32:14.795419 iscc_sdk-0.5.8/iscc_sdk/audio.py
--rw-r--r--   0        0        0     5272 2023-06-21 19:32:14.795419 iscc_sdk-0.5.8/iscc_sdk/cli.py
--rw-r--r--   0        0        0       99 2023-06-21 19:32:14.795419 iscc_sdk-0.5.8/iscc_sdk/compat.py
--rw-r--r--   0        0        0      897 2023-06-21 19:32:14.795419 iscc_sdk-0.5.8/iscc_sdk/docx_.py
--rw-r--r--   0        0        0     1491 2023-06-21 19:32:14.796759 iscc_sdk-0.5.8/iscc_sdk/epub.py
--rw-r--r--   0        0        0      166 2023-06-21 19:32:14.797758 iscc_sdk-0.5.8/iscc_sdk/exceptions.py
--rw-r--r--   0        0        0     8091 2023-06-21 19:32:14.797758 iscc_sdk-0.5.8/iscc_sdk/image.py
--rw-r--r--   0        0        0      683 2023-06-21 19:32:14.798760 iscc_sdk-0.5.8/iscc_sdk/install.py
--rw-r--r--   0        0        0     1274 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/ipfs.py
--rw-r--r--   0        0        0     7218 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/main.py
--rw-r--r--   0        0        0     9258 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/mediatype.py
--rw-r--r--   0        0        0     1898 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/metadata.py
--rw-r--r--   0        0        0     1905 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/monkeys.py
--rw-r--r--   0        0        0     3021 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/mp7.py
--rw-r--r--   0        0        0     2886 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/options.py
--rw-r--r--   0        0        0     2502 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/pdf.py
--rw-r--r--   0        0        0     5761 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/text.py
--rw-r--r--   0        0        0      684 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/thumbnail.py
--rw-r--r--   0        0        0    21133 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/tools.py
--rw-r--r--   0        0        0      602 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/utils.py
--rw-r--r--   0        0        0     6067 2023-06-21 19:32:14.799469 iscc_sdk-0.5.8/iscc_sdk/video.py
--rw-r--r--   0        0        0    11340 2022-03-29 10:37:56.086305 iscc_sdk-0.5.8/LICENSE
--rw-r--r--   0        0        0     3343 2023-06-21 19:32:14.735278 iscc_sdk-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3562 2023-06-21 19:32:14.735278 iscc_sdk-0.5.8/README.md
--rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 iscc_sdk-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      895 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/__init__.py
+-rw-r--r--   0        0        0     4346 2023-06-21 20:26:58.906116 iscc_sdk-0.5.9/iscc_sdk/audio.py
+-rw-r--r--   0        0        0     5272 2023-06-21 20:26:58.906116 iscc_sdk-0.5.9/iscc_sdk/cli.py
+-rw-r--r--   0        0        0       99 2023-06-21 20:26:58.906116 iscc_sdk-0.5.9/iscc_sdk/compat.py
+-rw-r--r--   0        0        0      897 2023-06-21 20:26:58.906116 iscc_sdk-0.5.9/iscc_sdk/docx_.py
+-rw-r--r--   0        0        0     1491 2023-06-21 20:26:58.906116 iscc_sdk-0.5.9/iscc_sdk/epub.py
+-rw-r--r--   0        0        0      166 2023-06-21 20:26:58.906116 iscc_sdk-0.5.9/iscc_sdk/exceptions.py
+-rw-r--r--   0        0        0     8126 2023-06-21 20:26:58.918353 iscc_sdk-0.5.9/iscc_sdk/image.py
+-rw-r--r--   0        0        0      683 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/install.py
+-rw-r--r--   0        0        0     1344 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/ipfs.py
+-rw-r--r--   0        0        0     7218 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/main.py
+-rw-r--r--   0        0        0     9258 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/mediatype.py
+-rw-r--r--   0        0        0     1898 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/metadata.py
+-rw-r--r--   0        0        0     1905 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/monkeys.py
+-rw-r--r--   0        0        0     3021 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/mp7.py
+-rw-r--r--   0        0        0     2886 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/options.py
+-rw-r--r--   0        0        0     2502 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/pdf.py
+-rw-r--r--   0        0        0     5796 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/text.py
+-rw-r--r--   0        0        0      684 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/thumbnail.py
+-rw-r--r--   0        0        0    21250 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/tools.py
+-rw-r--r--   0        0        0      602 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/utils.py
+-rw-r--r--   0        0        0     6102 2023-06-21 20:26:58.918881 iscc_sdk-0.5.9/iscc_sdk/video.py
+-rw-r--r--   0        0        0    11340 2022-03-29 10:37:56.086305 iscc_sdk-0.5.9/LICENSE
+-rw-r--r--   0        0        0     3343 2023-06-21 20:26:58.852241 iscc_sdk-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3562 2023-06-21 20:26:58.852241 iscc_sdk-0.5.9/README.md
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 iscc_sdk-0.5.9/PKG-INFO
```

### Comparing `iscc_sdk-0.5.8/iscc_sdk/__init__.py` & `iscc_sdk-0.5.9/iscc_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ISCC - Software Development Kit."""
 import os
 from platformdirs import PlatformDirs
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 APP_NAME = "iscc-sdk"
 APP_AUTHOR = "iscc"
 dirs = PlatformDirs(appname=APP_NAME, appauthor=APP_AUTHOR)
 os.makedirs(dirs.user_data_dir, exist_ok=True)
 os.environ["LOGURU_AUTOINIT"] = "False"
```

### Comparing `iscc_sdk-0.5.8/iscc_sdk/audio.py` & `iscc_sdk-0.5.9/iscc_sdk/audio.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/cli.py` & `iscc_sdk-0.5.9/iscc_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/docx_.py` & `iscc_sdk-0.5.9/iscc_sdk/docx_.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/epub.py` & `iscc_sdk-0.5.9/iscc_sdk/epub.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/image.py` & `iscc_sdk-0.5.9/iscc_sdk/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,16 @@
 
     :param str fp: Filepath to image file.
     :return: Metadata mapped to IsccMeta schema
     :rtype: dict
     """
     args = ["--all", fp]
     result = idk.run_exiv2json(args)
-    text = result.stdout.decode(sys.stdout.encoding, errors="ignore")
+    encoding = sys.stdout.encoding or "utf-8"
+    text = result.stdout.decode(encoding, errors="ignore")
 
     # We may get all sorts of crazy control-chars, delete them.
     mpa = dict.fromkeys(range(32))
     clean = text.translate(mpa)
 
     meta = json.loads(clean)
     mapped = dict()
```

### Comparing `iscc_sdk-0.5.8/iscc_sdk/install.py` & `iscc_sdk-0.5.9/iscc_sdk/install.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/ipfs.py` & `iscc_sdk-0.5.9/iscc_sdk/ipfs.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     :rtype: str
     """
     args = ["add", "--only-hash", "--cid-version=1", "--offline", "--quieter"]
     if wrap:
         args.append("--wrap-with-directory")
     args.append(fp)
     result = idk.run_ipfs(args)
-    cid = result.stdout.decode(sys.stdout.encoding).strip()
+    encoding = sys.stdout.encoding or "utf-8"
+    cid = result.stdout.decode(encoding).strip()
     if wrap:
         cid += f"/{basename(fp)}"
     return cid
 
 
 def ipfs_cidv1_base16(fp):
     # type: (str) -> str
@@ -48,8 +49,9 @@
         "--cid-version=1",
         "--offline",
         "--quieter",
         "--cid-base=base16",
         fp,
     ]
     result = idk.run_ipfs(args)
-    return result.stdout.decode(sys.stdout.encoding).strip()
+    encoding = sys.stdout.encoding or "utf-8"
+    return result.stdout.decode(encoding).strip()
```

### Comparing `iscc_sdk-0.5.8/iscc_sdk/main.py` & `iscc_sdk-0.5.9/iscc_sdk/main.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/mediatype.py` & `iscc_sdk-0.5.9/iscc_sdk/mediatype.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/metadata.py` & `iscc_sdk-0.5.9/iscc_sdk/metadata.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/monkeys.py` & `iscc_sdk-0.5.9/iscc_sdk/monkeys.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/mp7.py` & `iscc_sdk-0.5.9/iscc_sdk/mp7.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/options.py` & `iscc_sdk-0.5.9/iscc_sdk/options.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/pdf.py` & `iscc_sdk-0.5.9/iscc_sdk/pdf.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/text.py` & `iscc_sdk-0.5.9/iscc_sdk/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
     :param str fp: Filepath to text document file.
     :return: Metadata mapped to IsccMeta schema
     :rtype: dict
     """
     args = ["--metadata", "-j", "--encoding=UTF-8", fp]
 
     result = idk.run_tika(args)
-    meta = json.loads(result.stdout.decode(sys.stdout.encoding, errors="ignore"))
+    encoding = sys.stdout.encoding or "utf-8"
+    meta = json.loads(result.stdout.decode(encoding, errors="ignore"))
     mapped = dict()
     done = set()
     for tag, mapped_field in TEXT_META_MAP.items():
         if mapped_field in done:  # pragma nocover
             continue
         value = meta.get(tag)
         if value:
```

### Comparing `iscc_sdk-0.5.8/iscc_sdk/thumbnail.py` & `iscc_sdk-0.5.9/iscc_sdk/thumbnail.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/tools.py` & `iscc_sdk-0.5.9/iscc_sdk/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,16 @@
 
 def exiv2_version_info():  # pragma: no cover
     """Get exiv2 version info."""
     try:
         r = subprocess.run(
             [exiv2_bin(), "--version"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         )
-        vi = r.stdout.decode(sys.stdout.encoding)
+        encoding = sys.stdout.encoding or "utf-8"
+        vi = r.stdout.decode(encoding)
         return vi.splitlines()[0]
     except FileNotFoundError:
         return "exiv2 not installed"
 
 
 def run_exiv2(args: List[str]):
     """Run exiv2 command with `args`. Install exiv2 if not found."""
@@ -492,15 +493,16 @@
     log.critical("installing java")
     return jdk.install("16", impl="openj9", jre=True, path=idk.dirs.user_data_dir)
 
 
 def java_version_info():  # pragma: no cover
     try:
         r = subprocess.run([java_bin(), "-version"], stderr=subprocess.PIPE)
-        return r.stderr.decode(sys.stdout.encoding).splitlines()[0]
+        encoding = sys.stdout.encoding or "utf-8"
+        return r.stderr.decode(encoding).splitlines()[0]
     except subprocess.CalledProcessError:
         return "JAVA not installed"
 
 
 ########################################################################################
 # Apache Tika                                                                          #
 ########################################################################################
@@ -560,15 +562,16 @@
     Check tika-app version.
 
     :return: Tika version info string
     :rtype: str
     """
     try:
         r = subprocess.run([java_bin(), "-jar", tika_bin(), "--version"], stdout=subprocess.PIPE)
-        return r.stdout.decode(sys.stdout.encoding).strip()
+        encoding = sys.stdout.encoding or "utf-8"
+        return r.stdout.decode(encoding).strip()
     except subprocess.CalledProcessError:
         return "Tika not installed"
 
 
 def run_tika(args: List[str]):
     """Run tika command with `args`. Install tika if not found."""
     cmd = [java_bin(), "-jar", tika_bin()] + args
```

### Comparing `iscc_sdk-0.5.8/iscc_sdk/utils.py` & `iscc_sdk-0.5.9/iscc_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/iscc_sdk/video.py` & `iscc_sdk-0.5.9/iscc_sdk/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     :return: Metdata mpped to IsccMeta schema
     :rtype: dict
     """
 
     args = ["-i", fp, "-movflags", "use_metadata_tags", "-f", "ffmetadata", "-"]
 
     result = idk.run_ffmpeg(args)
-    text = result.stdout.decode(sys.stdout.encoding, errors="ignore")
+    encoding = sys.stdout.encoding or "utf-8"
+    text = result.stdout.decode(encoding, errors="ignore")
 
     # parse metadata
     meta = dict()
     for line in text.splitlines(keepends=False):
         if not line.startswith(";FFMETA"):
             key, value = line.split("=", 1)
             if value:
```

### Comparing `iscc_sdk-0.5.8/LICENSE` & `iscc_sdk-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/pyproject.toml` & `iscc_sdk-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iscc-sdk"
-version = "0.5.8"
+version = "0.5.9"
 description = "SDK for creating ISCCs (International Standard Content Codes)"
 authors = ["Titusz <tp@py7.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://sdk.iscc.codes"
 repository = "https://github.com/iscc/iscc-sdk"
 keywords=["iscc", "identifier", "media", "content", "hash", "blockchain", "similarity"]
```

### Comparing `iscc_sdk-0.5.8/README.md` & `iscc_sdk-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `iscc_sdk-0.5.8/PKG-INFO` & `iscc_sdk-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iscc-sdk
-Version: 0.5.8
+Version: 0.5.9
 Summary: SDK for creating ISCCs (International Standard Content Codes)
 Home-page: https://sdk.iscc.codes
 License: Apache-2.0
 Keywords: iscc,identifier,media,content,hash,blockchain,similarity
 Author: Titusz
 Author-email: tp@py7.de
 Requires-Python: >=3.8,<4.0
```

