# Comparing `tmp/rm_anime_bg-0.1.2.tar.gz` & `tmp/rm_anime_bg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rm_anime_bg-0.1.2.tar", max compression
+gzip compressed data, was "rm_anime_bg-0.2.0.tar", max compression
```

## Comparing `rm_anime_bg-0.1.2.tar` & `rm_anime_bg-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11358 2023-01-30 11:43:16.168972 rm_anime_bg-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1601 2023-06-12 05:27:19.997268 rm_anime_bg-0.1.2/README.md
--rw-r--r--   0        0        0      956 2023-06-21 18:23:28.470147 rm_anime_bg-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4472 2023-03-21 03:55:37.978299 rm_anime_bg-0.1.2/rm_anime_bg/cli.py
--rw-r--r--   0        0        0     2338 1970-01-01 00:00:00.000000 rm_anime_bg-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-30 11:43:16.168972 rm_anime_bg-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1885 2023-06-21 18:30:20.997860 rm_anime_bg-0.2.0/README.md
+-rw-r--r--   0        0        0     1083 2023-06-21 18:32:46.605767 rm_anime_bg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4739 2023-06-21 18:28:35.413930 rm_anime_bg-0.2.0/rm_anime_bg/cli.py
+-rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 rm_anime_bg-0.2.0/PKG-INFO
```

### Comparing `rm_anime_bg-0.1.2/LICENSE.txt` & `rm_anime_bg-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rm_anime_bg-0.1.2/README.md` & `rm_anime_bg-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 
 # rm_anime_bg
 
+[![PyPI version](https://badge.fury.io/py/rm_anime_bg.svg)](https://badge.fury.io/py/rm_anime_bg)
+[![Python Versions](https://img.shields.io/pypi/pyversions/rm_anime_bg.svg)](https://pypi.org/project/rm_anime_bg/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-![Python Versions](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
+[![Downloads](https://pepy.tech/badge/rm_anime_bg/week)](https://pepy.tech/project/rm_anime_bg)
+
 [![CI](https://github.com/shirayu/rm_anime_bg/actions/workflows/ci.yml/badge.svg)](https://github.com/shirayu/rm_anime_bg/actions/workflows/ci.yml)
 [![CodeQL](https://github.com/shirayu/rm_anime_bg/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/shirayu/rm_anime_bg/actions/workflows/codeql-analysis.yml)
 [![Typos](https://github.com/shirayu/rm_anime_bg/actions/workflows/typos.yml/badge.svg)](https://github.com/shirayu/rm_anime_bg/actions/workflows/typos.yml)
 
 A simple CLI of anime background remover with [SkyTNT/anime-segmentation](https://github.com/SkyTNT/anime-segmentation)
 
 ![An example of input image](example/example_0_original.png)
 ![An example of output image](example/example_0_after.png)
 
 [Image source](https://ja.wikipedia.org/wiki/%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB:Wikipe-tan_meets_mathematics.png), licensed under CC-BY-SA-3.0, Funa Funa
 
 ## Setup
 
 ```bash
-pip install -U git+https://github.com/shirayu/rm_anime_bg.git@v0.1.2
+# For CPU
+pip install -U 'rm_anime_bg[cpu]'
+
+# For GPU
+pip install -U 'rm_anime_bg[gpu]'
 ```
 
 ## Usage
 
 ```bash
 rm_anime_bg -o [Output directory] [Input 1] [Input 2] [Input 3] ... [Input N]
 ```
 
+- ``--cpu``: Force use of CPU
+
 Run ``rm_anime_bg --help`` to check full command options
 
 ### Example
 
 ```bash
 rm_anime_bg -o /path/to/output_dir input1.png input2.png
 ```
```

### Comparing `rm_anime_bg-0.1.2/pyproject.toml` & `rm_anime_bg-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-[misc]
-stable_version = "0.1.3"
 
 [tool.poetry]
 name = "rm_anime_bg"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 license = "Apache-2.0"
 authors = ["Yuta Hayashibe <yuta@hayashibe.jp>"]
 readme = "README.md"
 repository = "https://github.com/shirayu/rm_anime_bg.git"
 packages = [{include = "rm_anime_bg"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 opencv-python = ">=4.7.0.72"
 huggingface-hub = ">=0.14.1"
 numpy = ">=1.24.2"
-onnxruntime = ">=1.14.1"
 torch = "^2.0.1"
+onnxruntime = { version = "^1.15.1", optional = true }
+onnxruntime-gpu = { version = "^1.15.1", optional = true }
+
+[tool.poetry.extras]
+cpu = ["onnxruntime"]
+gpu = ["onnxruntime-gpu"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
 toml = "^0.10.2"
 flake8 = ">=5.0.4"
 pydocstyle = ">=6.1.1"
```

### Comparing `rm_anime_bg-0.1.2/rm_anime_bg/cli.py` & `rm_anime_bg-0.2.0/rm_anime_bg/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -74,28 +74,31 @@
     model_repo_id: str,
     model_filename: str,
     targets: List[str],
     output_matted: Optional[Path],
     output_dir: Optional[Path],
     alpha_min: float,
     alpha_max: float,
+    force_cpu: bool,
 ) -> None:
     if output_matted is None and output_dir is None:
         raise ValueError("No output directory names are given")
 
     session_infer_path = hf_hub_download(
         repo_id=model_repo_id,
         filename=model_filename,
     )
+
+    providers: list[str] = ["CPUExecutionProvider"]
+    if not force_cpu and "CUDAExecutionProvider" in rt.get_available_providers():
+        providers = ["CUDAExecutionProvider"]
+
     session_infer = rt.InferenceSession(
         session_infer_path,
-        providers=[
-            "CUDAExecutionProvider",
-            "CPUExecutionProvider",
-        ],
+        providers=providers,
     )
 
     for path in targets:
         img = cv2.cvtColor(cv2.imread(path, cv2.IMREAD_COLOR), cv2.COLOR_BGR2RGB)
         mask = get_mask(session_infer, img)
 
         mask[mask < alpha_min] = 0.0
@@ -148,25 +151,31 @@
         default=0.0,
     )
     oparser.add_argument(
         "--alpha-max",
         type=float,
         default=1.0,
     )
+    oparser.add_argument(
+        "--cpu",
+        action="store_true",
+        help="Force to use CPU",
+    )
     return oparser.parse_known_args()
 
 
 def main() -> None:
     (opts, targets) = get_opts()
     operation(
         model_repo_id=opts.model_repo_id,
         model_filename=opts.model_filename,
         targets=targets,
         output_dir=opts.output,
         output_matted=opts.matted,
         alpha_min=opts.alpha_min,
         alpha_max=opts.alpha_max,
+        force_cpu=opts.cpu,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `rm_anime_bg-0.1.2/PKG-INFO` & `rm_anime_bg-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,68 @@
 Metadata-Version: 2.1
 Name: rm-anime-bg
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/shirayu/rm_anime_bg.git
 License: Apache-2.0
 Author: Yuta Hayashibe
 Author-email: yuta@hayashibe.jp
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: cpu
+Provides-Extra: gpu
 Requires-Dist: huggingface-hub (>=0.14.1)
 Requires-Dist: numpy (>=1.24.2)
-Requires-Dist: onnxruntime (>=1.14.1)
+Requires-Dist: onnxruntime (>=1.15.1,<2.0.0) ; extra == "cpu"
+Requires-Dist: onnxruntime-gpu (>=1.15.1,<2.0.0) ; extra == "gpu"
 Requires-Dist: opencv-python (>=4.7.0.72)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/shirayu/rm_anime_bg.git
 Description-Content-Type: text/markdown
 
 
 # rm_anime_bg
 
+[![PyPI version](https://badge.fury.io/py/rm_anime_bg.svg)](https://badge.fury.io/py/rm_anime_bg)
+[![Python Versions](https://img.shields.io/pypi/pyversions/rm_anime_bg.svg)](https://pypi.org/project/rm_anime_bg/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-![Python Versions](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
+[![Downloads](https://pepy.tech/badge/rm_anime_bg/week)](https://pepy.tech/project/rm_anime_bg)
+
 [![CI](https://github.com/shirayu/rm_anime_bg/actions/workflows/ci.yml/badge.svg)](https://github.com/shirayu/rm_anime_bg/actions/workflows/ci.yml)
 [![CodeQL](https://github.com/shirayu/rm_anime_bg/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/shirayu/rm_anime_bg/actions/workflows/codeql-analysis.yml)
 [![Typos](https://github.com/shirayu/rm_anime_bg/actions/workflows/typos.yml/badge.svg)](https://github.com/shirayu/rm_anime_bg/actions/workflows/typos.yml)
 
 A simple CLI of anime background remover with [SkyTNT/anime-segmentation](https://github.com/SkyTNT/anime-segmentation)
 
 ![An example of input image](example/example_0_original.png)
 ![An example of output image](example/example_0_after.png)
 
 [Image source](https://ja.wikipedia.org/wiki/%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB:Wikipe-tan_meets_mathematics.png), licensed under CC-BY-SA-3.0, Funa Funa
 
 ## Setup
 
 ```bash
-pip install -U git+https://github.com/shirayu/rm_anime_bg.git@v0.1.2
+# For CPU
+pip install -U 'rm_anime_bg[cpu]'
+
+# For GPU
+pip install -U 'rm_anime_bg[gpu]'
 ```
 
 ## Usage
 
 ```bash
 rm_anime_bg -o [Output directory] [Input 1] [Input 2] [Input 3] ... [Input N]
 ```
 
+- ``--cpu``: Force use of CPU
+
 Run ``rm_anime_bg --help`` to check full command options
 
 ### Example
 
 ```bash
 rm_anime_bg -o /path/to/output_dir input1.png input2.png
 ```
```

