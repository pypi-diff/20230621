# Comparing `tmp/napari-labelprop-0.0.1.tar.gz` & `tmp/napari-labelprop-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-labelprop-0.0.1.tar", last modified: Mon Jun 19 12:44:48 2023, max compression
+gzip compressed data, was "napari-labelprop-1.0.0.tar", last modified: Wed Jun 21 07:14:26 2023, max compression
```

## Comparing `napari-labelprop-0.0.1.tar` & `napari-labelprop-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-19 12:44:48.688300 napari-labelprop-0.0.1/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1487 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/LICENSE
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       96 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/MANIFEST.in
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4503 2023-06-19 12:44:48.688300 napari-labelprop-0.0.1/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3698 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/README.md
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      172 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/pyproject.toml
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1033 2023-06-19 12:44:48.688300 napari-labelprop-0.0.1/setup.cfg
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-19 12:44:48.684300 napari-labelprop-0.0.1/src/
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-19 12:44:48.688300 napari-labelprop-0.0.1/src/napari_labelprop/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      266 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    16430 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_label_prop_widget.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3256 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_reader.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      380 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_sample_data.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-19 12:44:48.688300 napari-labelprop-0.0.1/src/napari_labelprop/_tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1250 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_tests/test_dock_widget.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      977 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_tests/test_reader.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      107 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_tests/test_sample_data.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1250 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_tests/test_widget.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      125 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_tests/test_writer.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1707 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_widget.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      841 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/_writer.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3588 2023-06-16 15:29:02.000000 napari-labelprop-0.0.1/src/napari_labelprop/napari.yaml
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-19 12:44:48.688300 napari-labelprop-0.0.1/src/napari_labelprop.egg-info/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4503 2023-06-19 12:44:48.000000 napari-labelprop-0.0.1/src/napari_labelprop.egg-info/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      827 2023-06-19 12:44:48.000000 napari-labelprop-0.0.1/src/napari_labelprop.egg-info/SOURCES.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2023-06-19 12:44:48.000000 napari-labelprop-0.0.1/src/napari_labelprop.egg-info/dependency_links.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       66 2023-06-19 12:44:48.000000 napari-labelprop-0.0.1/src/napari_labelprop.egg-info/entry_points.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       15 2023-06-19 12:44:48.000000 napari-labelprop-0.0.1/src/napari_labelprop.egg-info/requires.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       17 2023-06-19 12:44:48.000000 napari-labelprop-0.0.1/src/napari_labelprop.egg-info/top_level.txt
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-21 07:14:26.515107 napari-labelprop-1.0.0/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1487 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/LICENSE
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       96 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/MANIFEST.in
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6468 2023-06-21 07:14:26.515107 napari-labelprop-1.0.0/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5639 2023-06-21 06:18:29.000000 napari-labelprop-1.0.0/README.md
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      172 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/pyproject.toml
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1302 2023-06-21 07:14:26.515107 napari-labelprop-1.0.0/setup.cfg
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-21 07:14:26.511107 napari-labelprop-1.0.0/src/
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-21 07:14:26.511107 napari-labelprop-1.0.0/src/napari_labelprop/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      266 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/src/napari_labelprop/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    19191 2023-06-21 06:18:48.000000 napari-labelprop-1.0.0/src/napari_labelprop/_label_prop_widget.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3256 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/src/napari_labelprop/_reader.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      380 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/src/napari_labelprop/_sample_data.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-21 07:14:26.515107 napari-labelprop-1.0.0/src/napari_labelprop/_tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/src/napari_labelprop/_tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      107 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/src/napari_labelprop/_tests/test_sample_data.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      756 2023-06-21 06:58:13.000000 napari-labelprop-1.0.0/src/napari_labelprop/_tests/test_widget.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1707 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/src/napari_labelprop/_widget.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      841 2023-06-16 15:29:02.000000 napari-labelprop-1.0.0/src/napari_labelprop/_writer.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3632 2023-06-20 16:35:36.000000 napari-labelprop-1.0.0/src/napari_labelprop/napari.yaml
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2023-06-21 07:14:26.515107 napari-labelprop-1.0.0/src/napari_labelprop.egg-info/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6468 2023-06-21 07:14:26.000000 napari-labelprop-1.0.0/src/napari_labelprop.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      693 2023-06-21 07:14:26.000000 napari-labelprop-1.0.0/src/napari_labelprop.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2023-06-21 07:14:26.000000 napari-labelprop-1.0.0/src/napari_labelprop.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       66 2023-06-21 07:14:26.000000 napari-labelprop-1.0.0/src/napari_labelprop.egg-info/entry_points.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      104 2023-06-21 07:14:26.000000 napari-labelprop-1.0.0/src/napari_labelprop.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       17 2023-06-21 07:14:26.000000 napari-labelprop-1.0.0/src/napari_labelprop.egg-info/top_level.txt
```

### Comparing `napari-labelprop-0.0.1/LICENSE` & `napari-labelprop-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-labelprop-0.0.1/PKG-INFO` & `napari-labelprop-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-labelprop
-Version: 0.0.1
+Version: 1.0.0
 Summary: Label propagation through deep registration
 Author: nathandecaux
 Author-email: nathan.decaux@imt-atlantique.fr
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
@@ -14,84 +14,110 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 # napari-labelprop
 
 [![License](https://img.shields.io/pypi/l/napari-labelprop.svg?color=green)](https://github.com/nathandecaux/napari-labelprop/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-labelprop.svg?color=green)](https://pypi.org/project/napari-labelprop)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-labelprop.svg?color=green)](https://python.org)
 [![tests](https://github.com/nathandecaux/napari-labelprop/workflows/tests/badge.svg)](https://github.com/nathandecaux/napari-labelprop/actions)
 [![codecov](https://codecov.io/gh/nathandecaux/napari-labelprop/branch/main/graph/badge.svg)](https://codecov.io/gh/nathandecaux/napari-labelprop)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-labelprop)](https://napari-hub.org/plugins/napari-labelprop)
 
-Label propagation through deep registration.
 
-----------------------------------
 
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+3D semi-automatic segmentation using deep registration-based 2D label propagation
+---------------------------------------------------------------------------------
+---
+
+This [napari][napari] plugin was generated with [Cookiecutter][Cookiecutter] using [@napari][@napari]'s [cookiecutter-napari-plugin][cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/plugins/stable/index.html
 -->
 
+## About
+
+See "Semi-automatic muscle segmentation in MR images using deep registration-based label propagation" paper : 
+
+[[Paper]![Paper](https://www.integrad.nl/assets/uploads/2016/02/cta-elsevier_logo-no_bg.png)](https://www.sciencedirect.com/science/article/pii/S0031320323002297?casa_token=r5FPBVXYXX4AAAAA:mStyUXb0i4lGqBmfF1j5fV1T9FuCMrpYfwh3lwQve2XAnzUBPZviAiFgMtH7lv6hdcWsA7yM) [[PDF]![PDF](https://www.ouvrirlascience.fr/wp-content/uploads/2018/12/HAL-3.png)](https://hal.science/hal-03945559/document)
+<p>
+  <img src="https://github.com/nathandecaux/labelprop.github.io/raw/main/demo_cut.gif" width="600">
+</p>
+
 ## Installation
 
 To install this project :
 
     pip install napari['all']
-    git clone https://github.com/nathandecaux/napari-labelprop.git
-    cd napari-labelprop
-    pip install -e .
-
+    pip install git+https://github.com/nathandecaux/napari-labelprop.git
 
 ## Usage
 
-Open napari from terminal and start using functions from 'napari-labelprop' plugin (Under Plugins scrolling menu). 
+Download [pretrained weights](https://raw.githubusercontent.com/nathandecaux/napari-labelprop/main/pretrained.ckpt).
+
+Open napari from terminal and start using functions from 'napari-labelprop' plugin (Under Plugins scrolling menu).
 
 Available functions are :
+
 - Inference : Propagate labels from trained weights (Pytorch checkpoint required)
-- Training : Start training from scratch or from a pretrained model
-- Remove annotated slices : (testing purpose) Function to remove every annotations except for declared slices. Kept slices must be declared in the 'slices' field using comma (',') separation (eg. 5,12,43)
+- Training : Start training from scratch or from the pretrained weights.
+
+PS : "Unsupervised pretraining" is not yet implemented. See CLI option at [LabelProp](https://github.com/nathandecaux/labelprop) repository.
 
-PS : "pretraining" option in the Training menu is still under development
+Every operation is done in the main thread. So, napari is not responsive during training or inference, but you can still follow the progress in the terminal.
 
-Alternatively, napari and plugin widgets can be called directly from python scripts : 
+##### Training
 
-```python
-import nibabel as ni
-import napari
-
-viewer = napari.view_image(ni.load('images.nii.gz').get_fdata())
-viewer.add_labels(ni.load('segmentation.nii.gz').get_fdata().astype('uint8'))
-dw, my_widget = viewer.window.add_plugin_dock_widget('napari-labelprop', 'Training')
-my_widget.checkpoint_output_dir.value='~'
-my_widget.checkpoint_name.value='checkpoint_name'
-my_widget.z_axis.value=2
-my_widget.pretraining.value=False
-napari.run()
-```
+To train a model, reach the plugin in the menu bar :
+
+    Plugins > napari-labelprop > Training
+
+Fill the fields with the following information :
+
+- `Image` : Select a loaded napari.layers.Image layer to segment
+- `Labels` : Select a loaded napari.layers.Labels layer with the initial labels
+- `hints` : Select a loaded napari.layers.Labels layer with scribbled pseudo labels
+- `Pretrained checkpoint` : Select a pretrained checkpoint from the server-side checkpoint directory
+- `Slices shape` : Slices are resample to this shape for training and inference, then resampled to original shape. So far, slices must be squares.  
+- `Propagation axis` : Set the axis to use for the propagation dimension
+- `Max epochs` : Set the maximum number of epochs to train the model
+- `Checkpoint output directory`
+- `Checkpoint name`
+- `Weighting criteria` : Defines the criteria used to weight each direction of propagation `ncc = normalized cross correlation (slow but smooth), distance = distance to the nearest label (fast but less accurate)`
+- `Reduction` : When using ncc, defines the reduction to apply to the ncc map `mean / local_mean / none`. Default is `none`
+- `Use GPU` : Set if whether to use the GPU or not. Default is `True` (GPU). GPU:0 is used by default. To use another GPU, set the `CUDA_VISIBLE_DEVICES` environment variable before launching napari.
+
+##### Inference
+
+To run inference on a model, reach the plugin in the menu bar :
+
+    Plugins > napari-labelprop-remote > Inference
+
+Fill the fields like in the training section. Then, click on the `Run` button.
 
 ## Contributing
 
-Contributions are very welcome. Tests can be run with [tox], please ensure
+Contributions are very welcome. Tests can be run with [tox][tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
-Distributed under the terms of the [BSD-3] license,
+Distributed under the terms of the [BSD-3][BSD-3] license,
 "napari-labelprop" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
@@ -100,12 +126,11 @@
 [MIT]: http://opensource.org/licenses/MIT
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
 [GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
```

### Comparing `napari-labelprop-0.0.1/setup.cfg` & `napari-labelprop-1.0.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-labelprop
-version = 0.0.1
+version = 1.0.0
 author = nathandecaux
 author_email = nathan.decaux@imt-atlantique.fr
 license = BSD-3-Clause
 description = Label propagation through deep registration
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -22,23 +22,35 @@
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 package_dir = 
 	=src
-install_requires = 
-	deep-labelprop
+install_requires = deep-labelprop
+	napari-nifti
+	numpy
+	magicgui
+	qtpy
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.yaml
 
+[options.extras_require]
+testing = 
+	tox
+	pytest  # https://docs.pytest.org/en/latest/contents.html
+	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
+	pytest-qt  # https://pytest-qt.readthedocs.io/en/latest/
+	napari
+	pyqt5
+
 [options.entry_points]
 napari.manifest = 
 	napari-labelprop = napari_labelprop:napari.yaml
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `napari-labelprop-0.0.1/src/napari_labelprop/_label_prop_widget.py` & `napari-labelprop-1.0.0/src/napari_labelprop/_label_prop_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 from magicgui.widgets import FileEdit
 from magicgui.types import FileDialogMode
 from os import listdir
 from os.path import isfile, join
 import fnmatch
 from magicgui.widgets import create_widget
 import torch
+import time
+from contextlib import redirect_stdout
+import io
 from torch.nn.functional import one_hot
 from monai.metrics import compute_meandice
 from copy import deepcopy
 import numpy as np
 import datetime
 import napari
 from skimage import morphology
@@ -157,34 +160,58 @@
     print(f"you have selected {img_layer.data.shape}")
 
 
 # Uses the `autogenerate: true` flag in the plugin manifest
 # to indicate it should be wrapped as a magicgui to autogenerate
 # a widget
 
-def inference_function(image: "napari.layers.Image", labels: "napari.layers.Labels", checkpoint: "napari.types.Path", z_axis: int, label : int,criteria='ncc',reduction='none',gpu=True) -> "napari.types.LayerDataTuple":
+def inference_function(image: "napari.layers.Image", labels_layer: "napari.layers.Labels", hints: "napari.layers.Labels", checkpoint: "napari.types.Path", z_axis: int, label_n : int,criteria='ncc',reduction='none',gpu=True) -> "napari.types.LayerDataTuple":
     """Generate thresholded image.
 
     This function will be turned into a widget using `autogenerate: true`.
     """
     shape=torch.load(checkpoint)['hyper_parameters']['shape'][0]
     device='cuda' if gpu else 'cpu'
     kwargs={'criteria':criteria,'reduction':reduction,'device':device}
     checkpoint=str(checkpoint)
-    if label==0: label='all'
+    labels_data=labels_layer.data.astype('uint8')
+    if hints==labels_layer:
+        hints=''
+
+    if hints!='':
+        hints_data=hints.data.astype('uint8')
+    else:
+        hints_data=None
+    if label_n>0:
+        labels_data=(labels_data==label_n)*1
+        if hints!='':
+            hints_data=(hints_data==label_n)*1
+    if label_n==0: label_n='all'
     Y_up, Y_down, Y_fused = propagate_from_ckpt(
-        image.data, labels.data, checkpoint, z_axis=z_axis,label=label,shape=shape,**kwargs)
- 
-    return [((Y_up).astype('uint8'), {'name': 'propagated_up','metadata':labels.metadata}, 'labels'), ((Y_down).astype('uint8'), {'name': 'propagated_down','metadata':labels.metadata}, 'labels'), ((Y_fused).astype('uint8'), {'name': 'propagated_fused','metadata':labels.metadata}, 'labels')]
+        image.data, labels_data, checkpoint, hints=hints_data, z_axis=z_axis,label=label_n,shape=shape,**kwargs)
+    
+    return (Y_fused, {"name":"Propagated","affine": labels_layer.affine, "metadata": labels_layer.metadata}, "labels")
+    # return [((Y_up).astype('uint8'), {'name': 'propagated_up','metadata':labels.metadata}, 'labels'), ((Y_down).astype('uint8'), {'name': 'propagated_down','metadata':labels.metadata}, 'labels'), ((Y_fused).astype('uint8'), {'name': 'propagated_fused','metadata':labels.metadata}, 'labels')]
 
 class inference(FunctionGui):
-    def __init__(self):
+    def __init__(self,viewer: "napari.viewer.Viewer"):         
         super().__init__(inference_function,call_button=True,param_options={'criteria':{'choices':['distance','ncc']},'reduction':{'choices':['none','local_mean','mean']},'checkpoint':{'filter':'*.ckpt'}})
+        #Change display name of parameters
         self.criteria.changed.connect(self.update_reduction)
-  
+        self.image.label='Image'
+        self.labels_layer.label='Labels'
+        self.hints.label='(Optional) Additional Scribbles'
+
+        self.checkpoint.label='Checkpoint'
+        self.z_axis.label='Propagation axis'
+        self.label_n.label='Label to propagate (0 for all)'
+        self.criteria.label='Weighting criteria'
+        self.reduction.label='Reduction'
+        self.gpu.label='Use GPU'
+
     def __call__(self):
         napari.utils.notifications.show_info('Inference started')
         #Call super in an unblocking thread (avoid WARNING QObject::setParent: Cannot set parent, new parent is in a different thread)
         worker=self._call_super()
     #     worker.returned.connect(self._on_finished)
     #     worker.start()
     # # @nqt.thread_worker(connect={'returned':_on_finished})
@@ -202,43 +229,89 @@
             self.reduction.hide()
         else:
             self.reduction.show()
 
 
 #@magicgui(call_button='run')#(checkpoint_output_dir={'mode': 'd'}, call_button='Run') , checkpoint_output_dir: pathlib.Path.home()
 # @magic_factory(checkpoint_output_dir=dict(widget_type='FileEdit', mode='d'))
-def training_function(image: "napari.layers.Image", labels: "napari.layers.Labels", pretrained_checkpoint: "napari.types.Path" = '/home/', shape: int=256, z_axis: int=0, max_epochs: int=10,checkpoint_output_dir = '/home/',checkpoint_name='',criteria='ncc',reduction='none',gpu=True) -> "napari.types.LayerDataTuple":
+def training_function(image: "napari.layers.Image", labels_layer: "napari.layers.Labels",hints: "napari.layers.Labels", pretrained_checkpoint: "napari.types.Path", shape=(256,256), z_axis: int=0,label_n: int=0, max_epochs: int=50,checkpoint_output_dir = '/tmp/checkpoints/',checkpoint_name='',criteria='ncc',reduction='none',gpu=True) -> "napari.types.LayerDataTuple":
     """Generate thresholded image.
 
     This function will be turned into a widget using `autogenerate: true`.
     """
-    if not 'ckpt' in str(pretrained_checkpoint): pretrained_checkpoint=None
+    pretrained_checkpoint=None if not 'ckpt' in str(pretrained_checkpoint) else str(pretrained_checkpoint)
+    print(pretrained_checkpoint)
     device='cuda' if gpu else 'cpu'
     kwargs={'criteria':criteria,'reduction':reduction,'device':device}
+    labels_data=labels_layer.data.astype('uint8')
+
+    if hints==labels_layer:
+        hints=''
+
+    if hints!='':
+        hints_data=hints.data.astype('uint8')
+    else:
+        hints_data=None
+
+    if label_n>0:
+        labels_data=(labels_data==label_n)*1
+        if hints!='':
+            hints_data=(hints_data==label_n)*1
+    if label_n==0: label_n='all'
+    print(checkpoint_name)
     Y_up, Y_down, Y_fused = train_and_infer(
-        image.data, labels.data, str(pretrained_checkpoint),shape,max_epochs,z_axis,str(checkpoint_output_dir),checkpoint_name,pretraining=False,**kwargs)
+        image.data, labels_data, pretrained_checkpoint,shape[0],max_epochs,z_axis,str(checkpoint_output_dir),checkpoint_name,hints=hints_data,pretraining=False,**kwargs)
     torch.cuda.empty_cache()
-    return [((Y_up).astype('uint8'), {'name': 'propagated_up','metadata':labels.metadata}, 'labels'), ((Y_down).astype('uint8'), {'name': 'propagated_down','metadata':labels.metadata}, 'labels'), ((Y_fused).astype('uint8'), {'name': 'propagated_fused','metadata':labels.metadata}, 'labels')]
+    napari.utils.notifications.show_info('Training finished')
 
+    return (Y_fused, {"name":"Propagated","affine": labels_layer.affine, "metadata": labels_layer.metadata}, "labels")
 class training(FunctionGui):
-    def __init__(self):
+    def __init__(self,viewer: "napari.viewer.Viewer"):
         super().__init__(training_function,call_button=True,param_options={'criteria':{'choices':['distance','ncc']},'reduction':{'choices':['none','local_mean','mean']}, 'checkpoint_output_dir':{'widget_type':'FileEdit','mode': 'd'},'pretrained_checkpoint':{'filter':'*.ckpt'}})
         self.criteria.changed.connect(self.update_reduction)
-    def __call__(self):
+        self.image.label='Image'
+        self.labels_layer.label='Labels'
+        self.hints.label='(Optional) Additional Scribbles'
+        self.pretrained_checkpoint.label='Pretrained checkpoint'
+        self.shape.label='Slices shape'
+        self.z_axis.label='Propagation axis'
+        self.label_n.label='Label to propagate (0 for all)'
+        self.max_epochs.label='Max epochs'
+        self.checkpoint_output_dir.label='Checkpoint output directory'
+        #Get current directory
+        self.checkpoint_output_dir.value=str(pathlib.Path.cwd())
+        self.checkpoint_name.label='Checkpoint name'
+        self.criteria.label='Weighting criteria'
+        self.reduction.label='Reduction'
+        self.gpu.label='Use GPU'
+
+        #Disable shape second dimension
+        self.shape[1].enabled=False
+        self.shape[0].changed.connect(self.update_shape_2)
+        self.image.changed.connect(self.update_shape)
+        self.z_axis.changed.connect(self.update_shape)
+        self.call_button.clicked.connect(self._on_click)
+    
+    def _on_click(self):
         napari.utils.notifications.show_info('Training started')
-        super().__call__()
-        napari.utils.notifications.show_info('Training finished')
 
     def update_reduction(self):
         if self.criteria.value=='distance':
             self.reduction.value='mean'
             self.reduction.hide()
         else:
             self.reduction.show()
 
+    def update_shape(self):
+        if self.image.value is not None:
+            img_shape=self.image.value.data.shape[:self.z_axis.value]+self.image.value.data.shape[self.z_axis.value+1:]
+            self.shape.value=tuple(img_shape)
+    
+    def update_shape_2(self):
+        self.shape[1].value=self.shape[0].value
 
 def filter_slices(labels: "napari.layers.Labels",slices : str,z_axis: int=0) -> "napari.types.LayerDataTuple":
     slices=slices.replace(' ','').split(',')
     print(slices)
     labels_filtered=deepcopy(labels.data)
     indx = [slice(None)]*labels.ndim
```

### Comparing `napari-labelprop-0.0.1/src/napari_labelprop/_reader.py` & `napari-labelprop-1.0.0/src/napari_labelprop/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-labelprop-0.0.1/src/napari_labelprop/_widget.py` & `napari-labelprop-1.0.0/src/napari_labelprop/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-labelprop-0.0.1/src/napari_labelprop/_writer.py` & `napari-labelprop-1.0.0/src/napari_labelprop/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-labelprop-0.0.1/src/napari_labelprop/napari.yaml` & `napari-labelprop-1.0.0/src/napari_labelprop/napari.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,25 @@
       title: Show metrics between two label slices
     - id: napari-labelprop.remove_small_objects
       python_name: napari_labelprop._label_prop_widget:remove_small_objects
       title: Remove objects smaller than the specified size.
     - id: napari-labelprop.get_supervoxels
       python_name: napari_labelprop._label_prop_widget:get_supervoxels
       title: Get supervoxels
-  readers:
-    - command: napari-labelprop.get_reader
-      accepts_directories: false
-      filename_patterns: ['*.nii.gz'] 
-  writers:
-    - command: napari-labelprop.write_multiple
-      layer_types: ['image*','labels*']
-      filename_extensions: []
-    - command: napari-labelprop.write_single_image
-      layer_types: ['image']
-      filename_extensions: ['.npy'] 
+  # readers:
+  #   - command: napari-labelprop.get_reader
+  #     accepts_directories: false
+  #     filename_patterns: ['*.nii.gz'] 
+  # writers:
+  #   - command: napari-labelprop.write_multiple
+  #     layer_types: ['image*','labels*']
+  #     filename_extensions: []
+  #   - command: napari-labelprop.write_single_image
+  #     layer_types: ['image']
+  #     filename_extensions: ['.npy'] 
   sample_data:
     - command: napari-labelprop.make_sample_data
       display_name: napari Label Propagation
       key: unique_id.1 
   widgets:
     # - command: napari-labelprop.make_qwidget
     #   display_name: Example QWidget
@@ -66,20 +66,20 @@
     #   display_name: Example Function Widget 
     - command: napari-labelprop.inference_widget
       # autogenerate: true
       display_name: Inference
     - command: napari-labelprop.training_widget
       # autogenerate: true
       display_name:  Training
-    - command: napari-labelprop.filter_widget
-      autogenerate: true
-      display_name:  Remove annotated slices
-    - command: napari-labelprop.get_metrics
-      display_name:  Get metrics
-    - command: napari-labelprop.remove_small_objects
-      autogenerate: true
-      display_name:  Remove small objects
-    - command: napari-labelprop.get_supervoxels
-      autogenerate: true
-      display_name:  Get supervoxels
+    # - command: napari-labelprop.filter_widget
+    #   autogenerate: true
+    #   display_name:  Remove annotated slices
+    # - command: napari-labelprop.get_metrics
+    #   display_name:  Get metrics
+    # - command: napari-labelprop.remove_small_objects
+    #   autogenerate: true
+    #   display_name:  Remove small objects
+    # - command: napari-labelprop.get_supervoxels
+    #   autogenerate: true
+    #   display_name:  Get supervoxels
```

### Comparing `napari-labelprop-0.0.1/src/napari_labelprop.egg-info/PKG-INFO` & `napari-labelprop-1.0.0/src/napari_labelprop.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-labelprop
-Version: 0.0.1
+Version: 1.0.0
 Summary: Label propagation through deep registration
 Author: nathandecaux
 Author-email: nathan.decaux@imt-atlantique.fr
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
@@ -14,84 +14,110 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 # napari-labelprop
 
 [![License](https://img.shields.io/pypi/l/napari-labelprop.svg?color=green)](https://github.com/nathandecaux/napari-labelprop/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-labelprop.svg?color=green)](https://pypi.org/project/napari-labelprop)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-labelprop.svg?color=green)](https://python.org)
 [![tests](https://github.com/nathandecaux/napari-labelprop/workflows/tests/badge.svg)](https://github.com/nathandecaux/napari-labelprop/actions)
 [![codecov](https://codecov.io/gh/nathandecaux/napari-labelprop/branch/main/graph/badge.svg)](https://codecov.io/gh/nathandecaux/napari-labelprop)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-labelprop)](https://napari-hub.org/plugins/napari-labelprop)
 
-Label propagation through deep registration.
 
-----------------------------------
 
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+3D semi-automatic segmentation using deep registration-based 2D label propagation
+---------------------------------------------------------------------------------
+---
+
+This [napari][napari] plugin was generated with [Cookiecutter][Cookiecutter] using [@napari][@napari]'s [cookiecutter-napari-plugin][cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/plugins/stable/index.html
 -->
 
+## About
+
+See "Semi-automatic muscle segmentation in MR images using deep registration-based label propagation" paper : 
+
+[[Paper]![Paper](https://www.integrad.nl/assets/uploads/2016/02/cta-elsevier_logo-no_bg.png)](https://www.sciencedirect.com/science/article/pii/S0031320323002297?casa_token=r5FPBVXYXX4AAAAA:mStyUXb0i4lGqBmfF1j5fV1T9FuCMrpYfwh3lwQve2XAnzUBPZviAiFgMtH7lv6hdcWsA7yM) [[PDF]![PDF](https://www.ouvrirlascience.fr/wp-content/uploads/2018/12/HAL-3.png)](https://hal.science/hal-03945559/document)
+<p>
+  <img src="https://github.com/nathandecaux/labelprop.github.io/raw/main/demo_cut.gif" width="600">
+</p>
+
 ## Installation
 
 To install this project :
 
     pip install napari['all']
-    git clone https://github.com/nathandecaux/napari-labelprop.git
-    cd napari-labelprop
-    pip install -e .
-
+    pip install git+https://github.com/nathandecaux/napari-labelprop.git
 
 ## Usage
 
-Open napari from terminal and start using functions from 'napari-labelprop' plugin (Under Plugins scrolling menu). 
+Download [pretrained weights](https://raw.githubusercontent.com/nathandecaux/napari-labelprop/main/pretrained.ckpt).
+
+Open napari from terminal and start using functions from 'napari-labelprop' plugin (Under Plugins scrolling menu).
 
 Available functions are :
+
 - Inference : Propagate labels from trained weights (Pytorch checkpoint required)
-- Training : Start training from scratch or from a pretrained model
-- Remove annotated slices : (testing purpose) Function to remove every annotations except for declared slices. Kept slices must be declared in the 'slices' field using comma (',') separation (eg. 5,12,43)
+- Training : Start training from scratch or from the pretrained weights.
+
+PS : "Unsupervised pretraining" is not yet implemented. See CLI option at [LabelProp](https://github.com/nathandecaux/labelprop) repository.
 
-PS : "pretraining" option in the Training menu is still under development
+Every operation is done in the main thread. So, napari is not responsive during training or inference, but you can still follow the progress in the terminal.
 
-Alternatively, napari and plugin widgets can be called directly from python scripts : 
+##### Training
 
-```python
-import nibabel as ni
-import napari
-
-viewer = napari.view_image(ni.load('images.nii.gz').get_fdata())
-viewer.add_labels(ni.load('segmentation.nii.gz').get_fdata().astype('uint8'))
-dw, my_widget = viewer.window.add_plugin_dock_widget('napari-labelprop', 'Training')
-my_widget.checkpoint_output_dir.value='~'
-my_widget.checkpoint_name.value='checkpoint_name'
-my_widget.z_axis.value=2
-my_widget.pretraining.value=False
-napari.run()
-```
+To train a model, reach the plugin in the menu bar :
+
+    Plugins > napari-labelprop > Training
+
+Fill the fields with the following information :
+
+- `Image` : Select a loaded napari.layers.Image layer to segment
+- `Labels` : Select a loaded napari.layers.Labels layer with the initial labels
+- `hints` : Select a loaded napari.layers.Labels layer with scribbled pseudo labels
+- `Pretrained checkpoint` : Select a pretrained checkpoint from the server-side checkpoint directory
+- `Slices shape` : Slices are resample to this shape for training and inference, then resampled to original shape. So far, slices must be squares.  
+- `Propagation axis` : Set the axis to use for the propagation dimension
+- `Max epochs` : Set the maximum number of epochs to train the model
+- `Checkpoint output directory`
+- `Checkpoint name`
+- `Weighting criteria` : Defines the criteria used to weight each direction of propagation `ncc = normalized cross correlation (slow but smooth), distance = distance to the nearest label (fast but less accurate)`
+- `Reduction` : When using ncc, defines the reduction to apply to the ncc map `mean / local_mean / none`. Default is `none`
+- `Use GPU` : Set if whether to use the GPU or not. Default is `True` (GPU). GPU:0 is used by default. To use another GPU, set the `CUDA_VISIBLE_DEVICES` environment variable before launching napari.
+
+##### Inference
+
+To run inference on a model, reach the plugin in the menu bar :
+
+    Plugins > napari-labelprop-remote > Inference
+
+Fill the fields like in the training section. Then, click on the `Run` button.
 
 ## Contributing
 
-Contributions are very welcome. Tests can be run with [tox], please ensure
+Contributions are very welcome. Tests can be run with [tox][tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
-Distributed under the terms of the [BSD-3] license,
+Distributed under the terms of the [BSD-3][BSD-3] license,
 "napari-labelprop" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
@@ -100,12 +126,11 @@
 [MIT]: http://opensource.org/licenses/MIT
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
 [GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
```

### Comparing `napari-labelprop-0.0.1/src/napari_labelprop.egg-info/SOURCES.txt` & `napari-labelprop-1.0.0/src/napari_labelprop.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,12 +13,9 @@
 src/napari_labelprop.egg-info/PKG-INFO
 src/napari_labelprop.egg-info/SOURCES.txt
 src/napari_labelprop.egg-info/dependency_links.txt
 src/napari_labelprop.egg-info/entry_points.txt
 src/napari_labelprop.egg-info/requires.txt
 src/napari_labelprop.egg-info/top_level.txt
 src/napari_labelprop/_tests/__init__.py
-src/napari_labelprop/_tests/test_dock_widget.py
-src/napari_labelprop/_tests/test_reader.py
 src/napari_labelprop/_tests/test_sample_data.py
-src/napari_labelprop/_tests/test_widget.py
-src/napari_labelprop/_tests/test_writer.py
+src/napari_labelprop/_tests/test_widget.py
```

