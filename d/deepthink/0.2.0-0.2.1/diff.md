# Comparing `tmp/deepthink-0.2.0.tar.gz` & `tmp/deepthink-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepthink-0.2.0.tar", last modified: Tue Jun 20 18:44:43 2023, max compression
+gzip compressed data, was "deepthink-0.2.1.tar", last modified: Wed Jun 21 14:32:50 2023, max compression
```

## Comparing `deepthink-0.2.0.tar` & `deepthink-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-20 18:44:43.411838 deepthink-0.2.0/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1059 2023-06-19 08:10:39.000000 deepthink-0.2.0/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2629 2023-06-20 18:44:43.411838 deepthink-0.2.0/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2112 2023-06-19 08:10:39.000000 deepthink-0.2.0/README.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-20 18:44:43.411838 deepthink-0.2.0/deepthink/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-06-19 08:10:39.000000 deepthink-0.2.0/deepthink/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6885 2023-06-20 10:51:11.000000 deepthink-0.2.0/deepthink/activations.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7036 2023-06-20 11:08:14.000000 deepthink-0.2.0/deepthink/history.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    35071 2023-06-20 16:21:01.000000 deepthink-0.2.0/deepthink/layers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6430 2023-06-20 16:11:39.000000 deepthink-0.2.0/deepthink/loss.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3779 2023-06-20 16:14:35.000000 deepthink-0.2.0/deepthink/metrics.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13416 2023-06-20 17:40:26.000000 deepthink-0.2.0/deepthink/model.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14734 2023-06-20 16:20:20.000000 deepthink-0.2.0/deepthink/optimizers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7421 2023-06-20 18:39:16.000000 deepthink-0.2.0/deepthink/utils.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-20 18:44:43.411838 deepthink-0.2.0/deepthink.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2629 2023-06-20 18:44:43.000000 deepthink-0.2.0/deepthink.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      379 2023-06-20 18:44:43.000000 deepthink-0.2.0/deepthink.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-06-20 18:44:43.000000 deepthink-0.2.0/deepthink.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       79 2023-06-20 18:44:43.000000 deepthink-0.2.0/deepthink.egg-info/requires.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       10 2023-06-20 18:44:43.000000 deepthink-0.2.0/deepthink.egg-info/top_level.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-06-20 18:44:43.411838 deepthink-0.2.0/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1005 2023-06-20 16:24:28.000000 deepthink-0.2.0/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-21 14:32:49.998134 deepthink-0.2.1/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1059 2023-06-19 08:10:39.000000 deepthink-0.2.1/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2629 2023-06-21 14:32:49.998134 deepthink-0.2.1/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2112 2023-06-19 08:10:39.000000 deepthink-0.2.1/README.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-21 14:32:49.994135 deepthink-0.2.1/deepthink/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-06-19 08:10:39.000000 deepthink-0.2.1/deepthink/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6885 2023-06-20 10:51:11.000000 deepthink-0.2.1/deepthink/activations.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6957 2023-06-21 10:22:13.000000 deepthink-0.2.1/deepthink/history.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    35071 2023-06-20 16:21:01.000000 deepthink-0.2.1/deepthink/layers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6426 2023-06-21 10:49:38.000000 deepthink-0.2.1/deepthink/loss.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4188 2023-06-21 13:12:29.000000 deepthink-0.2.1/deepthink/metrics.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14283 2023-06-21 14:29:13.000000 deepthink-0.2.1/deepthink/model.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14734 2023-06-20 16:20:20.000000 deepthink-0.2.1/deepthink/optimizers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7421 2023-06-20 18:39:16.000000 deepthink-0.2.1/deepthink/utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-21 14:32:49.998134 deepthink-0.2.1/deepthink.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2629 2023-06-21 14:32:49.000000 deepthink-0.2.1/deepthink.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      379 2023-06-21 14:32:49.000000 deepthink-0.2.1/deepthink.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-06-21 14:32:49.000000 deepthink-0.2.1/deepthink.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       79 2023-06-21 14:32:49.000000 deepthink-0.2.1/deepthink.egg-info/requires.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       10 2023-06-21 14:32:49.000000 deepthink-0.2.1/deepthink.egg-info/top_level.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-06-21 14:32:49.998134 deepthink-0.2.1/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1005 2023-06-21 14:31:45.000000 deepthink-0.2.1/setup.py
```

### Comparing `deepthink-0.2.0/LICENSE` & `deepthink-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepthink-0.2.0/PKG-INFO` & `deepthink-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepthink
-Version: 0.2.0
+Version: 0.2.1
 Summary: Deep Learning library
 Home-page: https://github.com/Caff1982/DeepThink
 Author: Stephen Cafferty
 Author-email: stephencafferty@hotmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `deepthink-0.2.0/README.md` & `deepthink-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `deepthink-0.2.0/deepthink/activations.py` & `deepthink-0.2.1/deepthink/activations.py`

 * *Files identical despite different names*

### Comparing `deepthink-0.2.0/deepthink/history.py` & `deepthink-0.2.1/deepthink/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 
 from deepthink.metrics import (mean_squared_error,
                                root_mean_squared_error,
                                mean_absolute_error,
-                               accuracy,
-                               binary_accuracy)
+                               accuracy)
 
 
 class History:
     """
     A class to record model training history.
 
     Initialized when Model.train is called, this class records the
@@ -43,15 +42,14 @@
     Attributes
     ----------
     metric_dict : dict
         A dictionary which maps strings to metric loss function.
     """
     metric_dict = {
         'accuracy': accuracy,
-        'binary_accuracy': binary_accuracy,
         'RMSE': root_mean_squared_error,
         'MAE': mean_absolute_error,
         'MSE': mean_squared_error,
         }
 
     def __init__(self, metrics, n_epochs, verbose=True):
         self.metrics = metrics
@@ -158,15 +156,15 @@
         axes[0].xaxis.set_major_locator(MaxNLocator(20))
 
         if len(self.metrics) > 1:
             # Plot additional metric if included
             metric = self.metrics[1]
             axes[1].plot(self.history[metric], label=f'Train {metric}')
             axes[1].plot(self.history[f'val_{metric}'], label=f'Val {metric}')
-            axes[1].set_ylabel(metric, fontsize='x-large')
+            axes[1].set_ylabel(metric.capitalize(), fontsize='x-large')
             axes[1].legend(fontsize='large', framealpha=1, fancybox=True)
             axes[1].set_xticks(ticks=x_labels, labels=x_labels)
             axes[1].xaxis.set_major_locator(MaxNLocator(20))
 
         plt.xlabel('Epoch', fontsize='large')
         plt.legend(fontsize='large', framealpha=1, fancybox=True)
         if save_fname:
```

### Comparing `deepthink-0.2.0/deepthink/layers.py` & `deepthink-0.2.1/deepthink/layers.py`

 * *Files identical despite different names*

### Comparing `deepthink-0.2.0/deepthink/loss.py` & `deepthink-0.2.1/deepthink/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "loss" and "grads" methods. The "loss" method should take two
     arguments, y_true and y_hat, and return the loss value. If the
     arrays are not the same length then both will be resized to match.
     """
 
     def __call__(self, y_true, y_hat):
         # If arrays are not the same length then resize
-        if not y_true.shape != y_hat.shape:
+        if y_true.shape != y_hat.shape:
             min_len = min(y_true.shape[0], y_hat.shape[0])
             y_true = y_true[:min_len]
             y_hat = y_hat[:min_len]
         return self.loss(y_true, y_hat)
 
     def loss(self, y_true, y_hat):
         raise NotImplementedError(
```

### Comparing `deepthink-0.2.0/deepthink/metrics.py` & `deepthink-0.2.1/deepthink/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,127 @@
 import numpy as np
 
 
+def _set_array_lengths(y_true, y_hat):
+    """
+    A helper function to resize arrays to the same length.
+    If arrays are not the same length then they are resized
+    to the minimum length.
+    """
+    if y_true.shape[0] != y_hat.shape[0]:
+        min_len = min(y_true.shape[0], y_hat.shape[0])
+        y_true = y_true[:min_len]
+        y_hat = y_hat[:min_len]
+    return y_true, y_hat
+
+
 def mean_squared_error(y_true, y_hat):
     """
-    Return the Mean Squared Error (MSE) loss between labels and
-    predictions. Both arrays should be the same length.
+    Return the Mean Squared Error (MSE) loss between labels
+    and predictions. MSE is calculated as the mean of the
+    squared differences between the predicted and true values.
 
     Parameters
     ----------
     y_true : np.array
         The ground truth values
     y_hat : np.array
         The predicted values.
 
     Returns
     -------
-    np.array
+    float
         The MSE loss between predictions and labels.
     """
-    assert y_true.shape == y_hat.shape
+    y_true, y_hat = _set_array_lengths(y_true, y_hat)
     return np.square(y_true - y_hat).mean()
 
 
 def root_mean_squared_error(y_true, y_hat):
     """
-    Return the Root Mean Squared Error (RMSE) loss between labels and
-    predictions. Both arrays should be the same length.
+    Return the Root Mean Squared Error (RMSE) loss between labels
+    and predictions. RMSE is the square root of the MSE.
 
     Parameters
     ----------
     y_true : np.array
         The ground truth values
     y_hat : np.array
         The predicted values.
 
     Returns
     -------
-    np.array
+    float
         The RMSE loss between predictions and labels.
     """
-    assert y_true.shape == y_hat.shape
+    y_true, y_hat = _set_array_lengths(y_true, y_hat)
     return np.mean(np.sqrt(np.square(y_true - y_hat)))
 
 
 def mean_absolute_error(y_true, y_hat):
     """
-    Return the Mean Absolute Error (MSE) loss between labels and
-    predictions. Both arrays should be the same length.
+    Return the Mean Absolute Error (MSE) loss between labels
+    and predictions. This is also known as the L1 loss.
 
     Parameters
     ----------
     y_true : np.array
         The ground truth values
     y_hat : np.array
         The predicted values.
 
     Returns
     -------
-    np.array
+    float
         The MAE loss between predictions and labels.
     """
-    assert y_true.shape == y_hat.shape
+    y_true, y_hat = _set_array_lengths(y_true, y_hat)
     return np.mean(np.abs(y_true - y_hat))
 
 
 def accuracy(y_true, y_hat):
     """
     Return how often predictions equal labels.
 
-    Both input arrays should be 2D; y_true should be one-hot-encoded
-    and y_hat should be probabilities from softmax layer.
-
-    Parameters
-    ----------
-    y_true : np.array
-        The ground truth values.
-    y_hat : np.array
-        The predicted values.
-
-    Returns
-    -------
-    np.array
-        The accuracy between labels and predictions
-    """
-    return np.mean(np.argmax(y_true, axis=1) == np.argmax(y_hat, axis=1))
-
-
-def binary_accuracy(y_true, y_hat, threshold=0.5):
-    """
-    Return how often predictions match binary labels.
+    Both input arrays should be 2D. If the problem is binary
+    classification (i.e. y_true.shape[1] == 1), then the predictions
+    are rounded to 0 or 1. Otherwise, the predictions are assumed to
+    be probabilities from a softmax layer and the index of the highest
+    probability is used as the predicted class.
 
-    This function provides an accuracy metric for binary
-    classification tasks. The predictions, y_hat, should
-    be probabilities between 0 and 1. The'threshold' argument
-    decides which prediction values are rounded to 0 or 1.
+    If arrays are different lengths then they are resized to the
+    minimum length.
 
     Parameters
     ----------
     y_true : np.array
         The ground truth values.
     y_hat : np.array
         The predicted values.
-    threshold : float,default=0.5
-        The threshold for deciding whether prediction values are 1 or 0.
 
     Returns
     -------
-    np.array
+    float
         The accuracy between labels and predictions
     """
-    assert y_true.shape == y_hat.shape
-    return np.mean((y_hat > threshold).astype(int) == y_true)
+    # If arrays are different lengths resize to minimum length
+    y_true, y_hat = _set_array_lengths(y_true, y_hat)
+    # Check if binary classification
+    if y_true.shape[1] == 1:
+        return np.mean(np.round(y_true) == np.round(y_hat))
+    else:
+        # Otherwise, assume multi-class classification
+        return np.mean(np.argmax(y_true, axis=1) == np.argmax(y_hat, axis=1))
 
 
 def confusion_matrix(y_true, y_hat, k):
     """
-    Return a 2D confusion matrix where the rows are the actual values
-    and columns are predicted values.
+    Return a 2D confusion matrix where the rows are the actual
+    values and columns are predicted values. If arrays are 
+    different lengths then they are resized to the minimum length.
 
     Parameters
     ----------
     y_true : np.array
         The ground truth values
     y_hat : np.array
         The predicted values.
@@ -132,14 +133,15 @@
     result : np.array
         Two dimensional array representing actual and predicted values
 
     References
     ----------
     - https://en.wikipedia.org/wiki/Confusion_matrix
     """
+    y_true, y_hat = _set_array_lengths(y_true, y_hat)
     # If arrays are one-hot-encoded convert to 1D arrays
     if len(y_true.shape) == 2:
         y_true = np.argmax(y_true, axis=1)
     if len(y_hat.shape) == 2:
         y_hat = np.argmax(y_hat, axis=1)
     # Initialize the empty array with zeros
     result = np.zeros((k, k), dtype=int)
```

### Comparing `deepthink-0.2.0/deepthink/model.py` & `deepthink-0.2.1/deepthink/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pickle
+
 import numpy as np
 from tqdm import tqdm
 
 from deepthink.history import History
 from deepthink.layers import Dropout, BatchNorm
 
 
@@ -330,32 +332,59 @@
                 layer.weights = weights_arr.reshape(layer.weights.shape)
                 idx += layer.weights.size
             if hasattr(layer, 'bias'):
                 bias_arr = params[idx:idx+layer.bias.size]
                 layer.bias = bias_arr.reshape(layer.bias.shape)
                 idx += layer.bias.size
 
-    def save(self, filepath):
+    def save(self, filepath, weights_only=False):
         """
-        Save the model's weights & biases to specified filepath.
+        Save the model's weights & biases (and optionally the entire model)
+        to the specified filepath.
 
-        File-type should be '.npy'.
+        File-type should be '.npy' for weights and biases, and '.pkl'
+        for the entire model.
 
         Parameters
         ----------
         filepath : str
             The location to save the model's parameters.
-        """
-        params = self.get_params()
-        np.save(filepath, params)
+        weights_only : bool, optional
+            Whether to save only the weights and biases or the entire model
+            (default is False).
+        """
+        if weights_only:
+            params = self.get_params()
+            np.save(filepath, params)
+        else:
+            with open(filepath, 'wb') as file:
+                pickle.dump(self, file)
 
-    def load(self, filepath):
+    def load_weights(self, filepath):
         """
-        Load model parameters from specified filepath.
+        Load model weights and biases from the specified filepath.
 
         Parameters
         ----------
         filepath : str
-            The location to load the model's parameters from.
+            The location to load the model's weights and biases from.
         """
         params = np.load(filepath)
         self.set_params(params)
+
+    @staticmethod
+    def load_model(filepath):
+        """
+        Load the entire model from the specified filepath.
+
+        Parameters
+        ----------
+        filepath : str
+            The location to load the entire model from.
+
+        Returns
+        -------
+        Model
+            The loaded model object.
+        """
+        with open(filepath, 'rb') as file:
+            return pickle.load(file)
```

### Comparing `deepthink-0.2.0/deepthink/optimizers.py` & `deepthink-0.2.1/deepthink/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepthink-0.2.0/deepthink/utils.py` & `deepthink-0.2.1/deepthink/utils.py`

 * *Files identical despite different names*

### Comparing `deepthink-0.2.0/deepthink.egg-info/PKG-INFO` & `deepthink-0.2.1/deepthink.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepthink
-Version: 0.2.0
+Version: 0.2.1
 Summary: Deep Learning library
 Home-page: https://github.com/Caff1982/DeepThink
 Author: Stephen Cafferty
 Author-email: stephencafferty@hotmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `deepthink-0.2.0/setup.py` & `deepthink-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='deepthink',
-    version='0.2.0 ',
+    version='0.2.1 ',
     description='Deep Learning library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Caff1982/DeepThink',
     author='Stephen Cafferty',
     author_email='stephencafferty@hotmail.com',
     license='MIT',
```

