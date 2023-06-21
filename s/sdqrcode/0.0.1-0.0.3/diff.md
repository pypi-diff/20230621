# Comparing `tmp/sdqrcode-0.0.1.tar.gz` & `tmp/sdqrcode-0.0.3.tar.gz`

## Comparing `sdqrcode-0.0.1.tar` & `sdqrcode-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/colabs/demo.ipynb
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/colabs/sdqrcode -> /home/philippehenrisaade/stable-difusion-qrcode-1/sdqrcode/
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/configs/custom.yaml
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/configs/default.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/LICENSE
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/README.md
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 sdqrcode-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/colabs/demo.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/configs/custom.yaml
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/configs/default.yaml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/LICENSE
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/README.md
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 sdqrcode-0.0.3/PKG-INFO
```

### Comparing `sdqrcode-0.0.1/configs/default.yaml` & `sdqrcode-0.0.3/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.0.1/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.0.3/src/sdqrcode/sdqrcode.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.0.1/LICENSE` & `sdqrcode-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.0.1/pyproject.toml` & `sdqrcode-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 [tool.hatch.build.targets.wheel.sources]
 "src" = ""
 
 
 [project]
 name = "sdqrcode"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
   { name="Philippe Saade", email="contactskollai@gmail.com" },
   { name="Ruben Gres", email="contactskollai@gmail.com" },
 ]
 description = "Generate qr codes with stable diffusion and controlnet with standardised methods"
+
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sdqrcode-0.0.1/PKG-INFO` & `sdqrcode-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.0.1
+Version: 0.0.3
 Summary: Generate qr codes with stable diffusion and controlnet with standardised methods
 Project-URL: Homepage, https://github.com/koll-ai/stable-difusion-qrcode
 Project-URL: Bug Tracker, https://github.com/koll-ai/stable-difusion-qrcode/issues
 Author-email: Philippe Saade <contactskollai@gmail.com>, Ruben Gres <contactskollai@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,8 +12,16 @@
 Requires-Python: >=3.7
 Requires-Dist: pyyaml
 Requires-Dist: qrcode[pil]
 Requires-Dist: webuiapi
 Description-Content-Type: text/markdown
 
 # Stable Diffusion QR Code
+unstable
 
+
+
+# build from source
+
+```bash
+git clone
+python3 -m build
```

