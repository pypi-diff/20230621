# Comparing `tmp/sdqrcode-0.0.4.tar.gz` & `tmp/sdqrcode-0.0.5.tar.gz`

## Comparing `sdqrcode-0.0.4.tar` & `sdqrcode-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/requirements.txt
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/colabs/demo.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/configs/custom.yaml
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/configs/default.yaml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/LICENSE
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/README.md
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 sdqrcode-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0   632523 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/colabs/demo.ipynb
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/colabs/demo_sdqrcode.ipynb
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/colabs/configs/default.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/configs/custom.yaml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/configs/default.yaml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/README.md
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 sdqrcode-0.0.5/PKG-INFO
```

### Comparing `sdqrcode-0.0.4/.github/workflows/publish-release.yml` & `sdqrcode-0.0.5/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.0.4/configs/default.yaml` & `sdqrcode-0.0.5/colabs/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.0.4/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.0.5/src/sdqrcode/sdqrcode.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.0.4/LICENSE` & `sdqrcode-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.0.4/README.md` & `sdqrcode-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Stable Diffusion QR Code
-alpha unstable version
+alpha version
 
 call automatic1111 webui to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770)
 
+<a target="_blank" href="https://colab.research.google.com/github/koll-ai/stable-difusion-qrcode/blob/master/colabs/demo_sdqrcode.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
+![file (4)](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305)
 
 # Install
 ```
 pip install sdqrcode
 ```
 
 # Usage
```

### Comparing `sdqrcode-0.0.4/pyproject.toml` & `sdqrcode-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.hatch.build.targets.wheel.sources]
 "src" = ""
 
 
 [project]
 name = "sdqrcode"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Philippe Saade", email="contactskollai@gmail.com" },
   { name="Ruben Gres", email="contactskollai@gmail.com" },
 ]
 description = "Generate qr codes with stable diffusion and controlnet with standardised methods"
 
 readme = "README.md"
```

### Comparing `sdqrcode-0.0.4/PKG-INFO` & `sdqrcode-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate qr codes with stable diffusion and controlnet with standardised methods
 Project-URL: Homepage, https://github.com/koll-ai/stable-difusion-qrcode
 Project-URL: Bug Tracker, https://github.com/koll-ai/stable-difusion-qrcode/issues
 Author-email: Philippe Saade <contactskollai@gmail.com>, Ruben Gres <contactskollai@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,18 +12,23 @@
 Requires-Python: >=3.7
 Requires-Dist: pyyaml
 Requires-Dist: qrcode[pil]
 Requires-Dist: webuiapi
 Description-Content-Type: text/markdown
 
 # Stable Diffusion QR Code
-alpha unstable version
+alpha version
 
 call automatic1111 webui to generate qrcodes, will add a pure diffusers version once [this PR is completed](https://github.com/huggingface/diffusers/pull/3770)
 
+<a target="_blank" href="https://colab.research.google.com/github/koll-ai/stable-difusion-qrcode/blob/master/colabs/demo_sdqrcode.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
+![file (4)](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305)
 
 # Install
 ```
 pip install sdqrcode
 ```
 
 # Usage
```

