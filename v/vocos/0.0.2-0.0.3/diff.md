# Comparing `tmp/vocos-0.0.2.tar.gz` & `tmp/vocos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocos-0.0.2.tar", last modified: Mon Jun 12 16:58:46 2023, max compression
+gzip compressed data, was "vocos-0.0.3.tar", last modified: Wed Jun 21 10:46:12 2023, max compression
```

## Comparing `vocos-0.0.2.tar` & `vocos-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:58:46.802756 vocos-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 16:58:40.000000 vocos-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-12 16:58:46.802756 vocos-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-12 16:58:40.000000 vocos-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:58:46.806756 vocos-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 16:58:40.000000 vocos-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:58:46.802756 vocos-0.0.2/vocos/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/discriminators.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/heads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/spectral_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:58:46.802756 vocos-0.0.2/vocos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:46:12.938567 vocos-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 10:46:09.000000 vocos-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-21 10:46:12.938567 vocos-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-21 10:46:09.000000 vocos-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:46:12.938567 vocos-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-21 10:46:09.000000 vocos-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:46:12.938567 vocos-0.0.3/vocos/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/discriminators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-21 10:46:09.000000 vocos-0.0.3/vocos/spectral_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:46:12.938567 vocos-0.0.3/vocos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-21 10:46:12.000000 vocos-0.0.3/vocos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 10:46:12.000000 vocos-0.0.3/vocos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:46:12.000000 vocos-0.0.3/vocos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-21 10:46:12.000000 vocos-0.0.3/vocos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 10:46:12.000000 vocos-0.0.3/vocos.egg-info/top_level.txt
```

### Comparing `vocos-0.0.2/LICENSE` & `vocos-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/PKG-INFO` & `vocos-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-Metadata-Version: 2.1
-Name: vocos
-Version: 0.0.2
-Summary: Fourier-based neural vocoder for high-quality audio synthesis
-Home-page: https://github.com/charactr-platform/vocos
-Author: Hubert Siuzdak
-Author-email: huberts@charactr.com
-Description-Content-Type: text/markdown
-Provides-Extra: train
-License-File: LICENSE
-
 # Vocos: Closing the gap between time-domain and Fourier-based neural vocoders for high-quality audio synthesis
 
 [Audio samples](https://charactr-platform.github.io/vocos/) |
 Paper [[abs]](https://arxiv.org/abs/2306.00814) [[pdf]](https://arxiv.org/pdf/2306.00814.pdf)
 
+Vocos is a fast neural vocoder designed to synthesize audio waveforms from acoustic features. Trained using a Generative
+Adversarial Network (GAN) objective, Vocos can generate waveforms in a single forward pass. Unlike other typical
+GAN-based vocoders, Vocos does not model audio samples in the time domain. Instead, it generates spectral
+coefficients, facilitating rapid audio reconstruction through inverse Fourier transform.
+
 ## Installation
 
 To use Vocos only in inference mode, install it using:
 
 ```bash
 pip install vocos
 ```
@@ -36,61 +30,60 @@
 import torch
 
 from vocos import Vocos
 
 vocos = Vocos.from_pretrained("charactr/vocos-mel-24khz")
 
 mel = torch.randn(1, 100, 256)  # B, C, T
-
-with torch.no_grad():
-    audio = vocos.decode(mel)
+audio = vocos.decode(mel)
 ```
 
 Copy-synthesis from a file:
 
 ```python
 import torchaudio
 
 y, sr = torchaudio.load(YOUR_AUDIO_FILE)
 if y.size(0) > 1:  # mix to mono
     y = y.mean(dim=0, keepdim=True)
 y = torchaudio.functional.resample(y, orig_freq=sr, new_freq=24000)
-
-with torch.no_grad():
-    y_hat = vocos(y)
+y_hat = vocos(y)
 ```
 
-### Reconstruct audio from EnCodec
+### Reconstruct audio from EnCodec tokens
 
-Additionally, you need to provide a `bandwidth_id` which corresponds to the lookup embedding for bandwidth from the
+Additionally, you need to provide a `bandwidth_id` which corresponds to the embedding for bandwidth from the
 list: `[1.5, 3.0, 6.0, 12.0]`.
 
 ```python
 vocos = Vocos.from_pretrained("charactr/vocos-encodec-24khz")
 
-quantized_features = torch.randn(1, 128, 256)
-bandwidth_id = torch.tensor([3])  # 12 kbps
+audio_tokens = torch.randint(low=0, high=1024, size=(8, 200))  # 8 codeboooks, 200 frames
+features = vocos.codes_to_features(audio_tokens)
+bandwidth_id = torch.tensor([2])  # 6 kbps
 
-with torch.no_grad():
-    audio = vocos.decode(quantized_features, bandwidth_id=bandwidth_id)  
+audio = vocos.decode(features, bandwidth_id=bandwidth_id)
 ```
 
 Copy-synthesis from a file: It extracts and quantizes features with EnCodec, then reconstructs them with Vocos in a
 single forward pass.
 
 ```python
 y, sr = torchaudio.load(YOUR_AUDIO_FILE)
 if y.size(0) > 1:  # mix to mono
     y = y.mean(dim=0, keepdim=True)
 y = torchaudio.functional.resample(y, orig_freq=sr, new_freq=24000)
 
-with torch.no_grad():
-    y_hat = vocos(y, bandwidth_id=bandwidth_id)
+y_hat = vocos(y, bandwidth_id=bandwidth_id)
 ```
 
+### Integrate with 🐶 [Bark](https://github.com/suno-ai/bark) text-to-audio model
+
+See [example notebook](notebooks%2FBark%2BVocos.ipynb).
+
 ## Pre-trained models
 
 The provided models were trained up to 2.5 million generator iterations, which resulted in slightly better objective
 scores
 compared to those reported in the paper.
 
 | Model Name                                                                          | Dataset       | Training Iterations | Parameters 
@@ -128,8 +121,8 @@
   year={2023}
 }
 ```
 
 ## License
 
 The code in this repository is released under the MIT license as found in the
-[LICENSE](LICENSE) file.
+[LICENSE](LICENSE) file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vocos-0.0.2/README.md` & `vocos-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,28 @@
+Metadata-Version: 2.1
+Name: vocos
+Version: 0.0.3
+Summary: Fourier-based neural vocoder for high-quality audio synthesis
+Home-page: https://github.com/charactr-platform/vocos
+Author: Hubert Siuzdak
+Author-email: huberts@charactr.com
+Description-Content-Type: text/markdown
+Provides-Extra: train
+License-File: LICENSE
+
 # Vocos: Closing the gap between time-domain and Fourier-based neural vocoders for high-quality audio synthesis
 
 [Audio samples](https://charactr-platform.github.io/vocos/) |
 Paper [[abs]](https://arxiv.org/abs/2306.00814) [[pdf]](https://arxiv.org/pdf/2306.00814.pdf)
 
+Vocos is a fast neural vocoder designed to synthesize audio waveforms from acoustic features. Trained using a Generative
+Adversarial Network (GAN) objective, Vocos can generate waveforms in a single forward pass. Unlike other typical
+GAN-based vocoders, Vocos does not model audio samples in the time domain. Instead, it generates spectral
+coefficients, facilitating rapid audio reconstruction through inverse Fourier transform.
+
 ## Installation
 
 To use Vocos only in inference mode, install it using:
 
 ```bash
 pip install vocos
 ```
@@ -25,61 +41,60 @@
 import torch
 
 from vocos import Vocos
 
 vocos = Vocos.from_pretrained("charactr/vocos-mel-24khz")
 
 mel = torch.randn(1, 100, 256)  # B, C, T
-
-with torch.no_grad():
-    audio = vocos.decode(mel)
+audio = vocos.decode(mel)
 ```
 
 Copy-synthesis from a file:
 
 ```python
 import torchaudio
 
 y, sr = torchaudio.load(YOUR_AUDIO_FILE)
 if y.size(0) > 1:  # mix to mono
     y = y.mean(dim=0, keepdim=True)
 y = torchaudio.functional.resample(y, orig_freq=sr, new_freq=24000)
-
-with torch.no_grad():
-    y_hat = vocos(y)
+y_hat = vocos(y)
 ```
 
-### Reconstruct audio from EnCodec
+### Reconstruct audio from EnCodec tokens
 
-Additionally, you need to provide a `bandwidth_id` which corresponds to the lookup embedding for bandwidth from the
+Additionally, you need to provide a `bandwidth_id` which corresponds to the embedding for bandwidth from the
 list: `[1.5, 3.0, 6.0, 12.0]`.
 
 ```python
 vocos = Vocos.from_pretrained("charactr/vocos-encodec-24khz")
 
-quantized_features = torch.randn(1, 128, 256)
-bandwidth_id = torch.tensor([3])  # 12 kbps
+audio_tokens = torch.randint(low=0, high=1024, size=(8, 200))  # 8 codeboooks, 200 frames
+features = vocos.codes_to_features(audio_tokens)
+bandwidth_id = torch.tensor([2])  # 6 kbps
 
-with torch.no_grad():
-    audio = vocos.decode(quantized_features, bandwidth_id=bandwidth_id)  
+audio = vocos.decode(features, bandwidth_id=bandwidth_id)
 ```
 
 Copy-synthesis from a file: It extracts and quantizes features with EnCodec, then reconstructs them with Vocos in a
 single forward pass.
 
 ```python
 y, sr = torchaudio.load(YOUR_AUDIO_FILE)
 if y.size(0) > 1:  # mix to mono
     y = y.mean(dim=0, keepdim=True)
 y = torchaudio.functional.resample(y, orig_freq=sr, new_freq=24000)
 
-with torch.no_grad():
-    y_hat = vocos(y, bandwidth_id=bandwidth_id)
+y_hat = vocos(y, bandwidth_id=bandwidth_id)
 ```
 
+### Integrate with 🐶 [Bark](https://github.com/suno-ai/bark) text-to-audio model
+
+See [example notebook](notebooks%2FBark%2BVocos.ipynb).
+
 ## Pre-trained models
 
 The provided models were trained up to 2.5 million generator iterations, which resulted in slightly better objective
 scores
 compared to those reported in the paper.
 
 | Model Name                                                                          | Dataset       | Training Iterations | Parameters 
@@ -117,8 +132,8 @@
   year={2023}
 }
 ```
 
 ## License
 
 The code in this repository is released under the MIT license as found in the
-[LICENSE](LICENSE) file.
+[LICENSE](LICENSE) file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vocos-0.0.2/setup.py` & `vocos-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/dataset.py` & `vocos-0.0.3/vocos/dataset.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/discriminators.py` & `vocos-0.0.3/vocos/discriminators.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/experiment.py` & `vocos-0.0.3/vocos/experiment.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/feature_extractors.py` & `vocos-0.0.3/vocos/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/heads.py` & `vocos-0.0.3/vocos/heads.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,23 @@
         Returns:
             Tensor: Reconstructed time-domain audio signal of shape (B, T), where T is the length of the output signal.
         """
         x = self.out(x).transpose(1, 2)
         mag, p = x.chunk(2, dim=1)
         mag = torch.exp(mag)
         mag = torch.clip(mag, max=1e2)  # safeguard to prevent excessively large magnitudes
+        # wrapping happens here. These two lines produce real and imaginary value
         x = torch.cos(p)
         y = torch.sin(p)
-        phase = torch.atan2(y, x)
-        S = mag * torch.exp(phase * 1j)
+        # recalculating phase here does not produce anything new
+        # only costs time
+        # phase = torch.atan2(y, x)
+        # S = mag * torch.exp(phase * 1j)
+        # better directly produce the complex value 
+        S = mag * (x + 1j * y)
         audio = self.istft(S)
         return audio
 
 
 class IMDCTSymExpHead(FourierHead):
     """
     IMDCT Head module for predicting MDCT coefficients with symmetric exponential function
```

### Comparing `vocos-0.0.2/vocos/helpers.py` & `vocos-0.0.3/vocos/helpers.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/loss.py` & `vocos-0.0.3/vocos/loss.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/models.py` & `vocos-0.0.3/vocos/models.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/modules.py` & `vocos-0.0.3/vocos/modules.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/pretrained.py` & `vocos-0.0.3/vocos/pretrained.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos/spectral_ops.py` & `vocos-0.0.3/vocos/spectral_ops.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.2/vocos.egg-info/PKG-INFO` & `vocos-0.0.3/vocos.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: vocos
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fourier-based neural vocoder for high-quality audio synthesis
 Home-page: https://github.com/charactr-platform/vocos
 Author: Hubert Siuzdak
 Author-email: huberts@charactr.com
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
 
 # Vocos: Closing the gap between time-domain and Fourier-based neural vocoders for high-quality audio synthesis
 
 [Audio samples](https://charactr-platform.github.io/vocos/) |
 Paper [[abs]](https://arxiv.org/abs/2306.00814) [[pdf]](https://arxiv.org/pdf/2306.00814.pdf)
 
+Vocos is a fast neural vocoder designed to synthesize audio waveforms from acoustic features. Trained using a Generative
+Adversarial Network (GAN) objective, Vocos can generate waveforms in a single forward pass. Unlike other typical
+GAN-based vocoders, Vocos does not model audio samples in the time domain. Instead, it generates spectral
+coefficients, facilitating rapid audio reconstruction through inverse Fourier transform.
+
 ## Installation
 
 To use Vocos only in inference mode, install it using:
 
 ```bash
 pip install vocos
 ```
@@ -36,61 +41,60 @@
 import torch
 
 from vocos import Vocos
 
 vocos = Vocos.from_pretrained("charactr/vocos-mel-24khz")
 
 mel = torch.randn(1, 100, 256)  # B, C, T
-
-with torch.no_grad():
-    audio = vocos.decode(mel)
+audio = vocos.decode(mel)
 ```
 
 Copy-synthesis from a file:
 
 ```python
 import torchaudio
 
 y, sr = torchaudio.load(YOUR_AUDIO_FILE)
 if y.size(0) > 1:  # mix to mono
     y = y.mean(dim=0, keepdim=True)
 y = torchaudio.functional.resample(y, orig_freq=sr, new_freq=24000)
-
-with torch.no_grad():
-    y_hat = vocos(y)
+y_hat = vocos(y)
 ```
 
-### Reconstruct audio from EnCodec
+### Reconstruct audio from EnCodec tokens
 
-Additionally, you need to provide a `bandwidth_id` which corresponds to the lookup embedding for bandwidth from the
+Additionally, you need to provide a `bandwidth_id` which corresponds to the embedding for bandwidth from the
 list: `[1.5, 3.0, 6.0, 12.0]`.
 
 ```python
 vocos = Vocos.from_pretrained("charactr/vocos-encodec-24khz")
 
-quantized_features = torch.randn(1, 128, 256)
-bandwidth_id = torch.tensor([3])  # 12 kbps
+audio_tokens = torch.randint(low=0, high=1024, size=(8, 200))  # 8 codeboooks, 200 frames
+features = vocos.codes_to_features(audio_tokens)
+bandwidth_id = torch.tensor([2])  # 6 kbps
 
-with torch.no_grad():
-    audio = vocos.decode(quantized_features, bandwidth_id=bandwidth_id)  
+audio = vocos.decode(features, bandwidth_id=bandwidth_id)
 ```
 
 Copy-synthesis from a file: It extracts and quantizes features with EnCodec, then reconstructs them with Vocos in a
 single forward pass.
 
 ```python
 y, sr = torchaudio.load(YOUR_AUDIO_FILE)
 if y.size(0) > 1:  # mix to mono
     y = y.mean(dim=0, keepdim=True)
 y = torchaudio.functional.resample(y, orig_freq=sr, new_freq=24000)
 
-with torch.no_grad():
-    y_hat = vocos(y, bandwidth_id=bandwidth_id)
+y_hat = vocos(y, bandwidth_id=bandwidth_id)
 ```
 
+### Integrate with 🐶 [Bark](https://github.com/suno-ai/bark) text-to-audio model
+
+See [example notebook](notebooks%2FBark%2BVocos.ipynb).
+
 ## Pre-trained models
 
 The provided models were trained up to 2.5 million generator iterations, which resulted in slightly better objective
 scores
 compared to those reported in the paper.
 
 | Model Name                                                                          | Dataset       | Training Iterations | Parameters
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

