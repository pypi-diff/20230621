# Comparing `tmp/featurelayers-1.0.5.tar.gz` & `tmp/featurelayers-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.0.5.tar", last modified: Wed Jun 21 12:11:30 2023, max compression
+gzip compressed data, was "featurelayers-1.0.6.tar", last modified: Wed Jun 21 17:05:50 2023, max compression
```

## Comparing `featurelayers-1.0.5.tar` & `featurelayers-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 12:11:30.708572 featurelayers-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-06-21 12:11:30.698014 featurelayers-1.0.5/FeatureLayers/
-drwxrwxrwx   0        0        0        0 2023-06-21 12:11:30.700557 featurelayers-1.0.5/FeatureLayers/Layers/
--rw-rw-rw-   0        0        0     3131 2023-06-21 10:29:31.000000 featurelayers-1.0.5/FeatureLayers/Layers/LBC.py
--rw-rw-rw-   0        0        0        0 2023-06-21 12:11:05.000000 featurelayers-1.0.5/FeatureLayers/Layers/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-21 11:37:38.000000 featurelayers-1.0.5/FeatureLayers/__init__.py
--rw-rw-rw-   0        0        0       53 2023-06-21 12:11:20.000000 featurelayers-1.0.5/FeatureLayers/example.py
--rw-rw-rw-   0        0        0      391 2023-06-21 12:11:30.708572 featurelayers-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-21 10:03:40.000000 featurelayers-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 12:11:30.706560 featurelayers-1.0.5/featurelayers.egg-info/
--rw-rw-rw-   0        0        0      391 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-21 12:11:30.000000 featurelayers-1.0.5/featurelayers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 12:11:30.709574 featurelayers-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-21 12:11:29.000000 featurelayers-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:05:50.596350 featurelayers-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 17:05:32.000000 featurelayers-1.0.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:05:50.592350 featurelayers-1.0.6/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 17:05:32.000000 featurelayers-1.0.6/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-21 17:05:32.000000 featurelayers-1.0.6/.idea/FeatureLayers.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:05:50.592350 featurelayers-1.0.6/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 17:05:32.000000 featurelayers-1.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-21 17:05:32.000000 featurelayers-1.0.6/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 17:05:32.000000 featurelayers-1.0.6/.idea/modules.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:05:50.592350 featurelayers-1.0.6/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-21 17:05:32.000000 featurelayers-1.0.6/.idea/runConfigurations/run.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 17:05:32.000000 featurelayers-1.0.6/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 17:05:50.596350 featurelayers-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 17:05:32.000000 featurelayers-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-21 17:05:32.000000 featurelayers-1.0.6/beforebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:05:50.596350 featurelayers-1.0.6/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 17:05:32.000000 featurelayers-1.0.6/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:05:50.596350 featurelayers-1.0.6/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 17:05:32.000000 featurelayers-1.0.6/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 17:05:32.000000 featurelayers-1.0.6/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:05:50.596350 featurelayers-1.0.6/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 17:05:32.000000 featurelayers-1.0.6/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 17:05:32.000000 featurelayers-1.0.6/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:05:50.596350 featurelayers-1.0.6/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 17:05:50.000000 featurelayers-1.0.6/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-21 17:05:50.000000 featurelayers-1.0.6/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:05:50.000000 featurelayers-1.0.6/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 17:05:50.000000 featurelayers-1.0.6/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 17:05:50.000000 featurelayers-1.0.6/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:05:50.596350 featurelayers-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-21 17:05:32.000000 featurelayers-1.0.6/setup.py
```

### Comparing `featurelayers-1.0.5/FeatureLayers/Layers/LBC.py` & `featurelayers-1.0.6/featurelayers/layers/LBC.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-# Imports
-from scipy.stats import bernoulli
-import joblib
-import numpy as np
-import tensorflow as tf
-import keras
-from keras.layers import Conv2D
-from keras import backend as K
-from keras.engine.base_layer import Layer
-
-
-# Non-trainable filters initialized with distribution
-# of Bernoulli as in article and then it's non-trainable
-def new_weights_non_trainable(h, w, num_input, num_output, sparsity=0.5):
-    # Extract integer values from the tuples
-    h_val, w_val = h
-    num_input_val, num_output_val = num_input, num_output
-
-    # Number of elements
-    num_elements = h_val * w_val * num_input_val * num_output_val
-    # Create an array with n number of elements
-    array = np.arange(num_elements)
-    # Random shuffle it
-    np.random.shuffle(array)
-    # Fill with 0
-    weight = np.zeros([num_elements])
-    # Get the number of elements in the array that need to be non-zero
-    ind = int(sparsity * num_elements + 0.5)
-    # Get a piece of it as indexes for the weight matrix
-    index = array[:ind]
-
-    for i in index:
-        # Fill those indexes with Bernoulli distribution
-        # Method rvs = random variates
-        weight[i] = bernoulli.rvs(0.5) * 2 - 1
-    # Reshape weights array for the matrix that we need
-    weights = weight.reshape(h_val, w_val, num_input_val, num_output_val)
-    return weights
-
-
-class LBC(Layer):
-    def __init__(self, filters, kernel_size, stride=1, padding='same', activation='relu', dilation=1, sparsity=0.9,
-                 name="khengyun"):
-        super(LBC, self).__init__()
-        self.nOutputPlane = filters
-        self.kW = kernel_size
-        self.sparsity = sparsity
-        self.LBC = Conv2D(filters, kernel_size=kernel_size, strides=stride, padding=padding,
-                          dilation_rate=dilation, activation=activation, use_bias=False, name=name)
-
-    def build(self, input_shape):
-        nInputPlane = input_shape[-1]
-
-        with K.name_scope(self.LBC.name):
-            self.LBC.build(input_shape)
-        anchor_weights = tf.Variable(new_weights_non_trainable(h=self.kW, w=self.kW, num_input=nInputPlane,
-                                                               num_output=self.nOutputPlane,
-                                                               sparsity=self.sparsity).astype(np.float32),
-                                     trainable=False)
-        self.LBC.kernel = anchor_weights
-        super(LBC, self).build(input_shape)
-
-    def call(self, x):
-        return self.LBC(x)
-
-    def compute_output_shape(self, input_shape):
-        return self.LBC.compute_output_shape(input_shape)
-
-    def get_config(self):
-        config = super(LBC, self).get_config()
-        config.update({
-            'filters': self.nOutputPlane,
-            'kernel_size': self.kW,
-            'stride': self.LBC.strides[0],
-            'padding': self.LBC.padding,
-            'activation': self.LBC.activation,
-            'dilation': self.LBC.dilation_rate[0],
-            'sparsity': self.sparsity,
-            'name': self.LBC.name
-        })
-        return config
+# Imports
+from scipy.stats import bernoulli
+import joblib
+import numpy as np
+import tensorflow as tf
+import keras
+from keras.layers import Conv2D
+from keras import backend as K
+from keras.engine.base_layer import Layer
+
+
+# Non-trainable filters initialized with distribution
+# of Bernoulli as in article and then it's non-trainable
+def new_weights_non_trainable(h, w, num_input, num_output, sparsity=0.5):
+    # Extract integer values from the tuples
+    h_val, w_val = h
+    num_input_val, num_output_val = num_input, num_output
+
+    # Number of elements
+    num_elements = h_val * w_val * num_input_val * num_output_val
+    # Create an array with n number of elements
+    array = np.arange(num_elements)
+    # Random shuffle it
+    np.random.shuffle(array)
+    # Fill with 0
+    weight = np.zeros([num_elements])
+    # Get the number of elements in the array that need to be non-zero
+    ind = int(sparsity * num_elements + 0.5)
+    # Get a piece of it as indexes for the weight matrix
+    index = array[:ind]
+
+    for i in index:
+        # Fill those indexes with Bernoulli distribution
+        # Method rvs = random variates
+        weight[i] = bernoulli.rvs(0.5) * 2 - 1
+    # Reshape weights array for the matrix that we need
+    weights = weight.reshape(h_val, w_val, num_input_val, num_output_val)
+    return weights
+
+
+class LBC(Layer):
+    def __init__(self, filters, kernel_size, stride=1, padding='same', activation='relu', dilation=1, sparsity=0.9,
+                 name="khengyun"):
+        super(LBC, self).__init__()
+        self.nOutputPlane = filters
+        self.kW = kernel_size
+        self.sparsity = sparsity
+        self.LBC = Conv2D(filters, kernel_size=kernel_size, strides=stride, padding=padding,
+                          dilation_rate=dilation, activation=activation, use_bias=False, name=name)
+
+    def build(self, input_shape):
+        nInputPlane = input_shape[-1]
+
+        with K.name_scope(self.LBC.name):
+            self.LBC.build(input_shape)
+        anchor_weights = tf.Variable(new_weights_non_trainable(h=self.kW, w=self.kW, num_input=nInputPlane,
+                                                               num_output=self.nOutputPlane,
+                                                               sparsity=self.sparsity).astype(np.float32),
+                                     trainable=False)
+        self.LBC.kernel = anchor_weights
+        super(LBC, self).build(input_shape)
+
+    def call(self, x):
+        return self.LBC(x)
+
+    def compute_output_shape(self, input_shape):
+        return self.LBC.compute_output_shape(input_shape)
+
+    def get_config(self):
+        config = super(LBC, self).get_config()
+        config.update({
+            'filters': self.nOutputPlane,
+            'kernel_size': self.kW,
+            'stride': self.LBC.strides[0],
+            'padding': self.LBC.padding,
+            'activation': self.LBC.activation,
+            'dilation': self.LBC.dilation_rate[0],
+            'sparsity': self.sparsity,
+            'name': self.LBC.name
+        })
+        return config
```

