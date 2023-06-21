# Comparing `tmp/img2tags-1.1.1.tar.gz` & `tmp/img2tags-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img2tags-1.1.1.tar", max compression
+gzip compressed data, was "img2tags-1.2.0.tar", max compression
```

## Comparing `img2tags-1.1.1.tar` & `img2tags-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11342 2023-06-18 12:23:44.766767 img2tags-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1822 2023-06-19 01:26:08.388203 img2tags-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-18 12:23:44.766767 img2tags-1.1.1/img2tags/__init__.py
--rw-r--r--   0        0        0     7361 2023-06-19 01:24:55.292352 img2tags-1.1.1/img2tags/cli.py
--rw-r--r--   0        0        0     3085 2023-06-18 12:23:44.766767 img2tags-1.1.1/img2tags/tagger.py
--rw-r--r--   0        0        0     1318 2023-06-19 01:25:11.772318 img2tags-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 img2tags-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-18 12:23:44.766767 img2tags-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1833 2023-06-19 04:51:19.656247 img2tags-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 12:23:44.766767 img2tags-1.2.0/img2tags/__init__.py
+-rw-r--r--   0        0        0     7519 2023-06-21 04:05:12.178341 img2tags-1.2.0/img2tags/cli.py
+-rw-r--r--   0        0        0     3085 2023-06-18 12:23:44.766767 img2tags-1.2.0/img2tags/tagger.py
+-rw-r--r--   0        0        0     1341 2023-06-21 04:07:13.630299 img2tags-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 img2tags-1.2.0/PKG-INFO
```

### Comparing `img2tags-1.1.1/LICENSE.txt` & `img2tags-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2tags-1.1.1/README.md` & `img2tags-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     --batch 4 \
     --ext json \
     --cpu \
     -i input_dir \
     -o output_dir
 ```
 
-The default threshold is used the values stored in ``config.json`` like [this](https://huggingface.co/shirayu/img2tags/blob/main/SmilingWolf__wd-v1-4-moat-tagger-v2/config.json).
-You can set the value in JSON format like ``--th {"0": 0.3, "4":0.2, "9":0.3}``.
+The values of default thresholds are stored in ``config.json`` in each model like [this](https://huggingface.co/shirayu/img2tags/blob/main/SmilingWolf__wd-v1-4-convnext-tagger-v2/config.json).
+You can set values in JSON format like ``--th {"0": 0.3, "4":0.2, "9":0.3}``.
 
 ## LICENSE
 
 Apache 2.0
 
 Some codes are based on codes in the following project.
```

### Comparing `img2tags-1.1.1/img2tags/cli.py` & `img2tags-1.2.0/img2tags/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,19 +78,14 @@
     ext: str,
     threshold_str: Optional[str],
     force_cpu: bool,
 ):
     assert path_in.exists(), f"Not found: {path_in}"
     assert path_in.is_dir(), f"Not directory: {path_in}"
 
-    if path_out is None:
-        path_out = path_in
-    else:
-        path_out.mkdir(exist_ok=True, parents=True)
-
     path_config: Path
     path_model = Path(path_or_name_model)
     if path_model.exists():
         path_config = path_model.joinpath("config.json")
         path_model = path_model.joinpath("model.onnx")
     else:
         items: list[str] = path_or_name_model.split("/")
@@ -138,15 +133,20 @@
         probs = model.run(None, {input_name: imgs})[0]
 
         for (image_path, _), prob in zip(path_imgs, probs):
             result = rconv(
                 prob=prob,
                 thresholds=thresholds,
             )
-            with path_out.joinpath(image_path.stem + f".{ext}").open("w") as outf:
+            my_path_out: Path = image_path.parent
+            if path_out is not None:
+                rel: Path = image_path.parent.relative_to(path_in)
+                my_path_out = path_out.joinpath(rel)
+                my_path_out.mkdir(exist_ok=True, parents=True)
+            with my_path_out.joinpath(image_path.stem + f".{ext}").open("w") as outf:
                 if is_json:
                     outf.write(result.json(indent=4, ensure_ascii=False))
                 else:
                     kvs: list[tuple[str, float]] = []
                     outs: list[str] = []
                     for c, tv in result.tags.items():
                         if c == 9:  # skip rating
```

### Comparing `img2tags-1.1.1/img2tags/tagger.py` & `img2tags-1.2.0/img2tags/tagger.py`

 * *Files identical despite different names*

### Comparing `img2tags-1.1.1/pyproject.toml` & `img2tags-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "img2tags"
-version = "1.1.1"
+version = "1.2.0"
 description = "Tag images"
 authors = ["Yuta Hayashibe <yuta@hayashibe.jp>"]
+license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/shirayu/img2tags"
 repository = "https://github.com/shirayu/img2tags"
 packages = [{include = "img2tags"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
```

### Comparing `img2tags-1.1.1/PKG-INFO` & `img2tags-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: img2tags
-Version: 1.1.1
+Version: 1.2.0
 Summary: Tag images
 Home-page: https://github.com/shirayu/img2tags
+License: Apache-2.0
 Author: Yuta Hayashibe
 Author-email: yuta@hayashibe.jp
 Requires-Python: >=3.9,<3.11
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: convert
 Provides-Extra: cpu
 Provides-Extra: gpu
 Requires-Dist: huggingface-hub (>=0.15.1,<0.16.0)
@@ -61,16 +63,16 @@
     --batch 4 \
     --ext json \
     --cpu \
     -i input_dir \
     -o output_dir
 ```
 
-The default threshold is used the values stored in ``config.json`` like [this](https://huggingface.co/shirayu/img2tags/blob/main/SmilingWolf__wd-v1-4-moat-tagger-v2/config.json).
-You can set the value in JSON format like ``--th {"0": 0.3, "4":0.2, "9":0.3}``.
+The values of default thresholds are stored in ``config.json`` in each model like [this](https://huggingface.co/shirayu/img2tags/blob/main/SmilingWolf__wd-v1-4-convnext-tagger-v2/config.json).
+You can set values in JSON format like ``--th {"0": 0.3, "4":0.2, "9":0.3}``.
 
 ## LICENSE
 
 Apache 2.0
 
 Some codes are based on codes in the following project.
```

