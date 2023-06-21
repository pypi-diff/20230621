# Comparing `tmp/descript-audio-codec-0.0.3.tar.gz` & `tmp/descript-audio-codec-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descript-audio-codec-0.0.3.tar", last modified: Mon Jun 19 19:31:56 2023, max compression
+gzip compressed data, was "descript-audio-codec-0.0.4.tar", last modified: Wed Jun 21 17:49:04 2023, max compression
```

## Comparing `descript-audio-codec-0.0.3.tar` & `descript-audio-codec-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/
--rw-r--r--   0 ishaan    (1016) research  (1001)     1074 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/LICENSE
--rw-r--r--   0 ishaan    (1016) research  (1001)     5933 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/PKG-INFO
--rw-r--r--   0 ishaan    (1016) research  (1001)     5176 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.3/README.md
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.564479 descript-audio-codec-0.0.3/dac/
--rw-r--r--   0 ishaan    (1016) research  (1001)      198 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/dac/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)      690 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.3/dac/__main__.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.564479 descript-audio-codec-0.0.3/dac/compare/
--rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/compare/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     1592 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/compare/encodec.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.564479 descript-audio-codec-0.0.3/dac/model/
--rw-r--r--   0 ishaan    (1016) research  (1001)       91 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/model/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     4190 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/model/base.py
--rw-r--r--   0 ishaan    (1016) research  (1001)    10483 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.3/dac/model/dac.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     7056 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/model/discriminator.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/dac/nn/
--rw-r--r--   0 ishaan    (1016) research  (1001)       63 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/nn/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)      809 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/nn/layers.py
--rw-r--r--   0 ishaan    (1016) research  (1001)    12042 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/nn/loss.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     9151 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/dac/nn/quantize.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/dac/utils/
--rw-r--r--   0 ishaan    (1016) research  (1001)     1421 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/dac/utils/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     4826 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/dac/utils/decode.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     5252 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/dac/utils/encode.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/
--rw-r--r--   0 ishaan    (1016) research  (1001)     5933 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/PKG-INFO
--rw-r--r--   0 ishaan    (1016) research  (1001)      596 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/SOURCES.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)        1 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/dependency_links.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)      194 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/requires.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)       10 2023-06-19 19:31:56.000000 descript-audio-codec-0.0.3/descript_audio_codec.egg-info/top_level.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)       38 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/setup.cfg
--rw-r--r--   0 ishaan    (1016) research  (1001)     1548 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/setup.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-19 19:31:56.568479 descript-audio-codec-0.0.3/tests/
--rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/tests/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     1913 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.3/tests/test_cli.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     2752 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.3/tests/test_train.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1074 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/LICENSE
+-rw-r--r--   0 ishaan    (1016) research  (1001)     6260 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/PKG-INFO
+-rw-r--r--   0 ishaan    (1016) research  (1001)     5503 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/README.md
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/
+-rw-r--r--   0 ishaan    (1016) research  (1001)      237 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/dac/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)      690 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.4/dac/__main__.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/compare/
+-rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/compare/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1592 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/compare/encodec.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/model/
+-rw-r--r--   0 ishaan    (1016) research  (1001)       91 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/model/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     4190 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/model/base.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)    10483 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.4/dac/model/dac.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     7056 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/model/discriminator.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/nn/
+-rw-r--r--   0 ishaan    (1016) research  (1001)       63 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/nn/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)      809 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/nn/layers.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)    12042 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/dac/nn/loss.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     9151 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.4/dac/nn/quantize.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/dac/utils/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2580 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/dac/utils/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     5891 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/dac/utils/decode.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     6357 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/dac/utils/encode.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     6260 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/PKG-INFO
+-rw-r--r--   0 ishaan    (1016) research  (1001)      596 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)        1 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)      194 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/requires.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)       10 2023-06-21 17:49:04.000000 descript-audio-codec-0.0.4/descript_audio_codec.egg-info/top_level.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)       38 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/setup.cfg
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1548 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/setup.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-06-21 17:49:04.223930 descript-audio-codec-0.0.4/tests/
+-rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/tests/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2232 2023-06-21 17:48:45.000000 descript-audio-codec-0.0.4/tests/test_cli.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2752 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.4/tests/test_train.py
```

### Comparing `descript-audio-codec-0.0.3/LICENSE` & `descript-audio-codec-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/PKG-INFO` & `descript-audio-codec-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descript-audio-codec
-Version: 0.0.3
+Version: 0.0.4
 Summary: A high-quality general neural audio codec.
 Home-page: https://github.com/descriptinc/descript-audio-codec
 Author: Prem Seetharaman, Rithesh Kumar
 Author-email: prem@descript.com
 License: MIT
 Keywords: audio,compression,machine learning
 Classifier: Intended Audience :: Developers
@@ -49,19 +49,22 @@
 
 ```
 pip install git+https://github.com/descriptinc/descript-audio-codec
 ```
 
 ### Weights
 Weights are released as part of this repo under MIT license.
-They are automatically downloaded when you first run `encode` or `decode` command. They can be cached locally with
+We release weights for models that can natively support 24kHz and 44.1kHz sampling rates.
+Weights are automatically downloaded when you first run `encode` or `decode` command. You can cache them using one of the following commands
+```bash
+python3 -m dac download # downloads the default 44kHz variant
+python3 -m dac download --model_type 44khz # downloads the 44kHz variant
+python3 -m dac download --model_type 24khz # downloads the 24kHz variant
 ```
-python3 -m dac download
-```
-We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
+We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches the default model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
 
 
 ### Compress audio
 ```
 python3 -m dac encode /path/to/input --output /path/to/output/codes
 ```
 
@@ -91,15 +94,15 @@
 
 from audiotools import AudioSignal
 
 # Init an empty model
 model = DAC()
 
 # Load compatible pre-trained model
-model = load_model(dac.__model_version__)
+model = load_model(tag="latest", model_type="44khz")
 model.eval()
 model.to('cuda')
 
 # Load audio signal file
 signal = AudioSignal('input.wav')
 
 # Encode audio signal
```

### Comparing `descript-audio-codec-0.0.3/README.md` & `descript-audio-codec-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -28,19 +28,22 @@
 
 ```
 pip install git+https://github.com/descriptinc/descript-audio-codec
 ```
 
 ### Weights
 Weights are released as part of this repo under MIT license.
-They are automatically downloaded when you first run `encode` or `decode` command. They can be cached locally with
+We release weights for models that can natively support 24kHz and 44.1kHz sampling rates.
+Weights are automatically downloaded when you first run `encode` or `decode` command. You can cache them using one of the following commands
+```bash
+python3 -m dac download # downloads the default 44kHz variant
+python3 -m dac download --model_type 44khz # downloads the 44kHz variant
+python3 -m dac download --model_type 24khz # downloads the 24kHz variant
 ```
-python3 -m dac download
-```
-We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
+We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches the default model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
 
 
 ### Compress audio
 ```
 python3 -m dac encode /path/to/input --output /path/to/output/codes
 ```
 
@@ -70,15 +73,15 @@
 
 from audiotools import AudioSignal
 
 # Init an empty model
 model = DAC()
 
 # Load compatible pre-trained model
-model = load_model(dac.__model_version__)
+model = load_model(tag="latest", model_type="44khz")
 model.eval()
 model.to('cuda')
 
 # Load audio signal file
 signal = AudioSignal('input.wav')
 
 # Encode audio signal
```

### Comparing `descript-audio-codec-0.0.3/dac/__main__.py` & `descript-audio-codec-0.0.4/dac/__main__.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/dac/compare/encodec.py` & `descript-audio-codec-0.0.4/dac/compare/encodec.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/dac/model/base.py` & `descript-audio-codec-0.0.4/dac/model/base.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/dac/model/dac.py` & `descript-audio-codec-0.0.4/dac/model/dac.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/dac/model/discriminator.py` & `descript-audio-codec-0.0.4/dac/model/discriminator.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/dac/nn/layers.py` & `descript-audio-codec-0.0.4/dac/nn/layers.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/dac/nn/loss.py` & `descript-audio-codec-0.0.4/dac/nn/loss.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/dac/nn/quantize.py` & `descript-audio-codec-0.0.4/dac/nn/quantize.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/dac/utils/decode.py` & `descript-audio-codec-0.0.4/dac/utils/decode.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import argbind
 import numpy as np
 import torch
 from audiotools import AudioSignal
 from tqdm import tqdm
 
-import dac
 from dac.utils import load_model
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
 @torch.no_grad()
 @torch.inference_mode()
@@ -95,21 +94,44 @@
 @argbind.bind(group="decode", positional=True, without_prefix=True)
 @torch.inference_mode()
 @torch.no_grad()
 def decode(
     input: str,
     output: str = "",
     weights_path: str = "",
-    model_tag: str = dac.__model_version__,
+    model_tag: str = "latest",
     preserve_sample_rate: bool = False,
     device: str = "cuda",
+    model_type: str = "44khz",
 ):
+    """Decode audio from codes.
+
+    Parameters
+    ----------
+    input : str
+        Path to input directory or file
+    output : str, optional
+        Path to output directory, by default "".
+        If `input` is a directory, the directory sub-tree relative to `input` is re-created in `output`.
+    weights_path : str, optional
+        Path to weights file, by default "". If not specified, the weights file will be downloaded from the internet using the
+        model_tag and model_type.
+    model_tag : str, optional
+        Tag of the model to use, by default "latest". Ignored if `weights_path` is specified.
+    preserve_sample_rate : bool, optional
+        If True, return audio will have the same sample rate as the original
+    device : str, optional
+        Device to use, by default "cuda". If "cpu", the model will be loaded on the CPU.
+    model_type : str, optional
+        The type of model to download. Must be one of "44khz" or "24khz". Defaults to "44khz". Ignored if `weights_path` is specified.
+    """
     generator = load_model(
         tag=model_tag,
         load_path=weights_path,
+        model_type=model_type,
     )
     generator.to(device)
     generator.eval()
 
     # Find all .dac files in input directory
     _input = Path(input)
     input_files = list(_input.glob("**/*.dac"))
```

### Comparing `descript-audio-codec-0.0.3/dac/utils/encode.py` & `descript-audio-codec-0.0.4/dac/utils/encode.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import argbind
 import numpy as np
 import torch
 from audiotools import AudioSignal
 from audiotools.core import util
 from tqdm import tqdm
 
-import dac
 from dac.utils import load_model
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
 @torch.no_grad()
 @torch.inference_mode()
@@ -120,21 +119,43 @@
 @argbind.bind(group="encode", positional=True, without_prefix=True)
 @torch.inference_mode()
 @torch.no_grad()
 def encode(
     input: str,
     output: str = "",
     weights_path: str = "",
-    model_tag: str = dac.__model_version__,
+    model_tag: str = "latest",
     n_quantizers: int = None,
     device: str = "cuda",
+    model_type: str = "44khz",
 ):
+    """Encode audio files in input path to .dac format.
+
+    Parameters
+    ----------
+    input : str
+        Path to input audio file or directory
+    output : str, optional
+        Path to output directory, by default "". If `input` is a directory, the directory sub-tree relative to `input` is re-created in `output`.
+    weights_path : str, optional
+        Path to weights file, by default "". If not specified, the weights file will be downloaded from the internet using the
+        model_tag and model_type.
+    model_tag : str, optional
+        Tag of the model to use, by default "latest". Ignored if `weights_path` is specified.
+    n_quantizers : int, optional
+        Number of quantizers to use, by default None. If not specified, all the quantizers will be used and the model will compress at maximum bitrate.
+    device : str, optional
+        Device to use, by default "cuda"
+    model_type : str, optional
+        The type of model to download. Must be one of "44khz" or "24khz". Defaults to "44khz". Ignored if `weights_path` is specified.
+    """
     generator = load_model(
         tag=model_tag,
         load_path=weights_path,
+        model_type=model_type,
     )
     generator.to(device)
     generator.eval()
     kwargs = {"n_quantizers": n_quantizers}
 
     # Find all audio files in input path
     input = Path(input)
```

### Comparing `descript-audio-codec-0.0.3/descript_audio_codec.egg-info/PKG-INFO` & `descript-audio-codec-0.0.4/descript_audio_codec.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descript-audio-codec
-Version: 0.0.3
+Version: 0.0.4
 Summary: A high-quality general neural audio codec.
 Home-page: https://github.com/descriptinc/descript-audio-codec
 Author: Prem Seetharaman, Rithesh Kumar
 Author-email: prem@descript.com
 License: MIT
 Keywords: audio,compression,machine learning
 Classifier: Intended Audience :: Developers
@@ -49,19 +49,22 @@
 
 ```
 pip install git+https://github.com/descriptinc/descript-audio-codec
 ```
 
 ### Weights
 Weights are released as part of this repo under MIT license.
-They are automatically downloaded when you first run `encode` or `decode` command. They can be cached locally with
+We release weights for models that can natively support 24kHz and 44.1kHz sampling rates.
+Weights are automatically downloaded when you first run `encode` or `decode` command. You can cache them using one of the following commands
+```bash
+python3 -m dac download # downloads the default 44kHz variant
+python3 -m dac download --model_type 44khz # downloads the 44kHz variant
+python3 -m dac download --model_type 24khz # downloads the 24kHz variant
 ```
-python3 -m dac download
-```
-We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
+We provide a Dockerfile that installs all required dependencies for encoding and decoding. The build process caches the default model weights inside the image. This allows the image to be used without an internet connection. [Please refer to instructions below.](#docker-image)
 
 
 ### Compress audio
 ```
 python3 -m dac encode /path/to/input --output /path/to/output/codes
 ```
 
@@ -91,15 +94,15 @@
 
 from audiotools import AudioSignal
 
 # Init an empty model
 model = DAC()
 
 # Load compatible pre-trained model
-model = load_model(dac.__model_version__)
+model = load_model(tag="latest", model_type="44khz")
 model.eval()
 model.to('cuda')
 
 # Load audio signal file
 signal = AudioSignal('input.wav')
 
 # Encode audio signal
```

### Comparing `descript-audio-codec-0.0.3/descript_audio_codec.egg-info/SOURCES.txt` & `descript-audio-codec-0.0.4/descript_audio_codec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.3/setup.py` & `descript-audio-codec-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="descript-audio-codec",
-    version="0.0.3",
+    version="0.0.4",
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Topic :: Artistic Software",
         "Topic :: Multimedia",
         "Topic :: Multimedia :: Sound/Audio",
```

### Comparing `descript-audio-codec-0.0.3/tests/test_cli.py` & `descript-audio-codec-0.0.4/tests/test_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Tests for CLI.
 """
 import subprocess
 from pathlib import Path
 
 import argbind
 import numpy as np
+import pytest
+import torch
 from audiotools import AudioSignal
 
 from dac.__main__ import run
 
 
 def setup_module(module):
     data_dir = Path(__file__).parent / "assets"
@@ -24,41 +26,49 @@
 
 
 def teardown_module(module):
     repo_root = Path(__file__).parent.parent
     subprocess.check_output(["rm", "-rf", f"{repo_root}/tests/assets"])
 
 
-def test_reconstruction():
+@pytest.mark.parametrize("model_type", ["44khz", "24khz"])
+def test_reconstruction(model_type):
     # Test encoding
     input_dir = Path(__file__).parent / "assets" / "input"
-    output_dir = input_dir.parent / "encoded_output"
+    output_dir = input_dir.parent / model_type / "encoded_output"
     args = {
         "input": str(input_dir),
         "output": str(output_dir),
+        "device": "cuda" if torch.cuda.is_available() else "cpu",
+        "model_type": model_type,
     }
     with argbind.scope(args):
         run("encode")
 
     # Test decoding
     input_dir = output_dir
-    output_dir = input_dir.parent / "decoded_output"
+    output_dir = input_dir.parent / model_type / "decoded_output"
     args = {
         "input": str(input_dir),
         "output": str(output_dir),
     }
     with argbind.scope(args):
         run("decode")
 
 
 def test_compression():
     # Test encoding
     input_dir = Path(__file__).parent / "assets" / "input"
     output_dir = input_dir.parent / "encoded_output_quantizers"
-    args = {"input": str(input_dir), "output": str(output_dir), "n_quantizers": 3}
+    args = {
+        "input": str(input_dir),
+        "output": str(output_dir),
+        "n_quantizers": 3,
+        "device": "cuda" if torch.cuda.is_available() else "cpu",
+    }
     with argbind.scope(args):
         run("encode")
 
     # Open .dac file
     dac_file = output_dir / "sample_0.dac"
     artifacts = np.load(dac_file, allow_pickle=True)[()]
     codes = artifacts["codes"]
```

### Comparing `descript-audio-codec-0.0.3/tests/test_train.py` & `descript-audio-codec-0.0.4/tests/test_train.py`

 * *Files identical despite different names*

