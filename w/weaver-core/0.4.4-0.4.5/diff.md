# Comparing `tmp/weaver-core-0.4.4.tar.gz` & `tmp/weaver-core-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaver-core-0.4.4.tar", last modified: Tue Jun 20 14:44:26 2023, max compression
+gzip compressed data, was "weaver-core-0.4.5.tar", last modified: Tue Jun 20 23:53:51 2023, max compression
```

## Comparing `weaver-core-0.4.4.tar` & `weaver-core-0.4.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.742385 weaver-core-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 14:43:35.000000 weaver-core-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-20 14:44:26.742385 weaver-core-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-06-20 14:43:35.000000 weaver-core-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:44:26.742385 weaver-core-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 14:43:35.000000 weaver-core-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.734385 weaver-core-0.4.4/weaver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.734385 weaver-core-0.4.4/weaver/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.734385 weaver-core-0.4.4/weaver/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/loss/focal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.734385 weaver-core-0.4.4/weaver/nn/model/
--rw-r--r--   0 runner    (1001) docker     (123)    35306 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/model/ParticleNeXt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/model/ParticleNet.py
--rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/model/ParticleTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45296 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.738385 weaver-core-0.4.4/weaver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.738385 weaver-core-0.4.4/weaver/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/import_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/lr_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.738385 weaver-core-0.4.4/weaver/utils/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.738385 weaver-core-0.4.4/weaver/utils/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/optimizer/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/optimizer/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/optimizer/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.742385 weaver-core-0.4.4/weaver_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.732155 weaver-core-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 23:53:08.000000 weaver-core-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-20 23:53:51.732155 weaver-core-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-06-20 23:53:08.000000 weaver-core-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:53:51.732155 weaver-core-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 23:53:08.000000 weaver-core-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.728155 weaver-core-0.4.5/weaver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.728155 weaver-core-0.4.5/weaver/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.728155 weaver-core-0.4.5/weaver/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/nn/loss/focal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.728155 weaver-core-0.4.5/weaver/nn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    35306 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/nn/model/ParticleNeXt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/nn/model/ParticleNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/nn/model/ParticleTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/nn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45625 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.728155 weaver-core-0.4.5/weaver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.728155 weaver-core-0.4.5/weaver/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/data/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/data/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/data/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17958 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/import_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/lr_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.728155 weaver-core-0.4.5/weaver/utils/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/nn/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.728155 weaver-core-0.4.5/weaver/utils/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/nn/optimizer/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/nn/optimizer/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/nn/optimizer/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-06-20 23:53:08.000000 weaver-core-0.4.5/weaver/utils/nn/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:51.732155 weaver-core-0.4.5/weaver_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-20 23:53:51.000000 weaver-core-0.4.5/weaver_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-20 23:53:51.000000 weaver-core-0.4.5/weaver_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:53:51.000000 weaver-core-0.4.5/weaver_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 23:53:51.000000 weaver-core-0.4.5/weaver_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:53:51.000000 weaver-core-0.4.5/weaver_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 23:53:51.000000 weaver-core-0.4.5/weaver_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 23:53:51.000000 weaver-core-0.4.5/weaver_core.egg-info/top_level.txt
```

### Comparing `weaver-core-0.4.4/LICENSE` & `weaver-core-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/PKG-INFO` & `weaver-core-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaver-core
-Version: 0.4.4
+Version: 0.4.5
 Summary: A streamlined deep-learning framework for high energy physics
 Home-page: https://github.com/hqucms/weaver-core
 Author: H. Qu, C. Li
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `weaver-core-0.4.4/README.md` & `weaver-core-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/setup.py` & `weaver-core-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         if not line:
             continue
         if line.startswith('#'):
             continue
         install_requires.append(line)
 
 setup(name="weaver-core",
-      version='0.4.4',
+      version='0.4.5',
       description="A streamlined deep-learning framework for high energy physics",
       long_description_content_type="text/markdown",
       author="H. Qu, C. Li",
       url="https://github.com/hqucms/weaver-core",
       long_description=long_desc,
       entry_points={'console_scripts':
                     ['weaver = weaver.train:main']},
```

### Comparing `weaver-core-0.4.4/weaver/nn/loss/focal.py` & `weaver-core-0.4.5/weaver/nn/loss/focal.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/nn/model/ParticleNeXt.py` & `weaver-core-0.4.5/weaver/nn/model/ParticleNeXt.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/nn/model/ParticleNet.py` & `weaver-core-0.4.5/weaver/nn/model/ParticleNet.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/nn/model/ParticleTransformer.py` & `weaver-core-0.4.5/weaver/nn/model/ParticleTransformer.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/train.py` & `weaver-core-0.4.5/weaver/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -700,14 +700,19 @@
             _logger.info(f'Using distributed PyTorch with {args.backend} backend')
         else:
             gpus = [int(i) for i in args.gpus.split(',')]
             dev = torch.device(gpus[0])
     else:
         gpus = None
         dev = torch.device('cpu')
+        try:
+            if torch.backends.mps.is_available():
+                dev = torch.device('mps')
+        except AttributeError:
+            pass
 
     # load data
     if training_mode:
         train_loader, val_loader, data_config, train_input_names, train_label_names = train_load(args)
     else:
         test_loaders, data_config = test_load(args)
 
@@ -904,20 +909,22 @@
         args.log += '.%03d' % args.local_rank
         if args.local_rank != 0:
             stdout = None
     _configLogger('weaver', stdout=stdout, filename=args.log)
 
     if args.cross_validation:
         model_dir, model_fn = os.path.split(args.model_prefix)
+        predict_output_base, predict_output_ext = os.path.splitext(args.predict_output)
         load_model = args.load_model_weights or None
         var_name, kfold = args.cross_validation.split('%')
         kfold = int(kfold)
         for i in range(kfold):
             _logger.info(f'\n=== Running cross validation, fold {i} of {kfold} ===')
             args.model_prefix = os.path.join(f'{model_dir}_fold{i}', model_fn)
+            args.predict_output = f'{predict_output_base}_fold{i}' + predict_output_ext
             args.extra_selection = f'{var_name}%{kfold}!={i}'
             args.extra_test_selection = f'{var_name}%{kfold}=={i}'
             if load_model and '{fold}' in load_model:
                 args.load_model_weights = load_model.replace('{fold}', f'fold{i}')
 
             _main(args)
     else:
```

### Comparing `weaver-core-0.4.4/weaver/utils/data/config.py` & `weaver-core-0.4.5/weaver/utils/data/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     def __init__(self, print_info=True, **kwargs):
 
         opts = {
             'treename': None,
             'branch_magic': None,
+            'file_magic': None,
             'selection': None,
             'test_time_selection': None,
             'preprocess': {'method': 'manual', 'data_fraction': 0.1, 'params': None},
             'new_variables': {},
             'inputs': {},
             'labels': {},
             'observers': [],
@@ -205,25 +206,27 @@
     def dump(self, fp):
         with open(fp, 'w') as f:
             yaml.safe_dump(self.options, f, sort_keys=False)
 
     @classmethod
     def load(cls, fp, load_observers=True, load_reweight_info=True, extra_selection=None, extra_test_selection=None):
         with open(fp) as f:
-            options = yaml.safe_load(f)
+            _opts = yaml.safe_load(f)
+            options = copy.deepcopy(_opts)
         if not load_observers:
             options['observers'] = None
         if not load_reweight_info:
             options['weights'] = None
         if extra_selection:
-            options['selection'] = '(%s) & (%s)' % (options['selection'], extra_selection)
+            options['selection'] = '(%s) & (%s)' % (_opts['selection'], extra_selection)
         if extra_test_selection:
-            if 'test_time_selection' not in options:
-                raise RuntimeError('`test_time_selection` is not defined in the yaml file!')
-            options['test_time_selection'] = '(%s) & (%s)' % (options['test_time_selection'], extra_test_selection)
+            if 'test_time_selection' not in options or options['test_time_selection'] is None:
+                options['test_time_selection'] = '(%s) & (%s)' % (_opts['selection'], extra_test_selection)
+            else:
+                options['test_time_selection'] = '(%s) & (%s)' % (_opts['test_time_selection'], extra_test_selection)
         return cls(**options)
 
     def copy(self):
         return self.__class__(print_info=False, **copy.deepcopy(self.options))
 
     def __copy__(self):
         return self.copy()
```

### Comparing `weaver-core-0.4.4/weaver/utils/data/fileio.py` & `weaver-core-0.4.5/weaver/utils/data/fileio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import awkward as ak
 import tqdm
 import traceback
 from .tools import _concat
-from ..logger import _logger
+from ..logger import _logger, warn_n_times
 
 
 def _read_hdf5(filepath, branches, load_range=None):
     import tables
     tables.set_blosc_max_threads(4)
     with tables.open_file(filepath) as f:
         outputs = {k: getattr(f.root, k)[:] for k in branches}
@@ -72,15 +72,15 @@
     if load_range is not None:
         start = math.trunc(load_range[0] * len(outputs))
         stop = max(start + 1, math.trunc(load_range[1] * len(outputs)))
         outputs = outputs[start:stop]
     return outputs
 
 
-def _read_files(filelist, branches, load_range=None, show_progressbar=False, **kwargs):
+def _read_files(filelist, branches, load_range=None, show_progressbar=False, file_magic=None, **kwargs):
     import os
     branches = list(branches)
     table = []
     if show_progressbar:
         filelist = tqdm.tqdm(filelist)
     for filepath in filelist:
         ext = os.path.splitext(filepath)[1]
@@ -98,14 +98,25 @@
             elif ext == '.parquet':
                 a = _read_parquet(filepath, branches, load_range=load_range)
         except Exception as e:
             a = None
             _logger.error('When reading file %s:', filepath)
             _logger.error(traceback.format_exc())
         if a is not None:
+            if file_magic is not None:
+                import re
+                for var, value_dict in file_magic.items():
+                    if var in a.fields:
+                        warn_n_times(f'Var `{var}` already defined in the arrays '
+                                     f'but will be OVERWRITTEN by file_magic {value_dict}.')
+                    a[var] = 0
+                    for fn_pattern, value in value_dict.items():
+                        if re.search(fn_pattern, filepath):
+                            a[var] = value
+                            break
             table.append(a)
     table = _concat(table)  # ak.Array
     if len(table) == 0:
         raise RuntimeError(f'Zero entries loaded when reading files {filelist} with `load_range`={load_range}.')
     return table
```

### Comparing `weaver-core-0.4.4/weaver/utils/data/preprocess.py` & `weaver-core-0.4.5/weaver/utils/data/preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import time
 import glob
 import copy
 import numpy as np
 import awkward as ak
 
-from ..logger import _logger
+from ..logger import _logger, warn_n_times
 from .tools import _get_variable_names, _eval_expr
 from .fileio import _read_files
 
 
-def _apply_selection(table, selection):
+def _apply_selection(table, selection, funcs={}):
     if selection is None:
         return table
+    new_vars = {k: funcs[k] for k in _get_variable_names(selection) if k not in table.fields and k in funcs}
+    _build_new_variables(table, new_vars)
     selected = ak.values_astype(_eval_expr(selection, table), 'bool')
     return table[selected]
 
 
 def _build_new_variables(table, funcs):
     if funcs is None:
         return table
@@ -27,15 +29,15 @@
 
 
 def _clean_up(table, drop_branches):
     columns = [k for k in table.fields if k not in drop_branches]
     return table[columns]
 
 
-def _build_weights(table, data_config, reweight_hists=None, warn=_logger.warning):
+def _build_weights(table, data_config, reweight_hists=None):
     if data_config.weight_name is None:
         raise RuntimeError('Error when building weights: `weight_name` is None!')
     if data_config.use_precomputed_weights:
         return ak.to_numpy(table[data_config.weight_name])
     else:
         x_var, y_var = data_config.reweight_branches
         x_bins, y_bins = data_config.reweight_bins
@@ -57,15 +59,15 @@
             x_indices = np.clip(np.digitize(
                 rwgt_x_vals, x_bins) - 1, a_min=0, a_max=len(x_bins) - 2)
             y_indices = np.clip(np.digitize(
                 rwgt_y_vals, y_bins) - 1, a_min=0, a_max=len(y_bins) - 2)
             wgt[pos] = hist[x_indices, y_indices]
             sum_evts += np.sum(pos)
         if sum_evts != len(table):
-            warn(
+            warn_n_times(
                 'Not all selected events used in the reweighting. '
                 'Check consistency between `selection` and `reweight_classes` definition, or with the `reweight_vars` binnings '
                 '(under- and overflow bins are discarded by default, unless `reweight_discard_under_overflow` is set to `False` in the `weights` section).',
             )
         if data_config.reweight_basewgt:
             wgt *= ak.to_numpy(table[data_config.basewgt_name])
         return wgt
@@ -101,16 +103,17 @@
                 else:
                     self.load_branches.add(k)
         if self._data_config.selection:
             self.load_branches.update(_get_variable_names(self._data_config.selection))
         _logger.debug('[AutoStandardizer] keep_branches:\n  %s', ','.join(self.keep_branches))
         _logger.debug('[AutoStandardizer] load_branches:\n  %s', ','.join(self.load_branches))
         table = _read_files(filelist, self.load_branches, self.load_range, show_progressbar=True,
-                            treename=self._data_config.treename, branch_magic=self._data_config.branch_magic)
-        table = _apply_selection(table, self._data_config.selection)
+                            treename=self._data_config.treename,
+                            branch_magic=self._data_config.branch_magic, file_magic=self._data_config.file_magic)
+        table = _apply_selection(table, self._data_config.selection, funcs=self._data_config.var_funcs)
         table = _build_new_variables(
             table, {k: v for k, v in self._data_config.var_funcs.items() if k in self.keep_branches})
         table = _clean_up(table, self.load_branches - self.keep_branches)
         return table
 
     def make_preprocess_params(self, table):
         _logger.info('Using %d events to calculate standardization info', len(table))
@@ -175,16 +178,17 @@
             else:
                 self.load_branches.add(k)
         if self._data_config.selection:
             self.load_branches.update(_get_variable_names(self._data_config.selection))
         _logger.debug('[WeightMaker] keep_branches:\n  %s', ','.join(self.keep_branches))
         _logger.debug('[WeightMaker] load_branches:\n  %s', ','.join(self.load_branches))
         table = _read_files(filelist, self.load_branches, show_progressbar=True,
-                            treename=self._data_config.treename, branch_magic=self._data_config.branch_magic)
-        table = _apply_selection(table, self._data_config.selection)
+                            treename=self._data_config.treename,
+                            branch_magic=self._data_config.branch_magic, file_magic=self._data_config.file_magic)
+        table = _apply_selection(table, self._data_config.selection, funcs=self._data_config.var_funcs)
         table = _build_new_variables(
             table, {k: v for k, v in self._data_config.var_funcs.items() if k in self.keep_branches})
         table = _clean_up(table, self.load_branches - self.keep_branches)
         return table
 
     def make_weights(self, table):
         x_var, y_var = self._data_config.reweight_branches
```

### Comparing `weaver-core-0.4.4/weaver/utils/data/tools.py` & `weaver-core-0.4.5/weaver/utils/data/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import numpy as np
 import math
 
 import awkward as ak
 
 
+def _hash(*args):
+    return np.array([x.__hash__() for x in zip(*args)])
+
+
 def _concat(arrays, axis=0):
     if len(arrays) == 0:
         return np.array([])
     if isinstance(arrays[0], np.ndarray):
         return np.concatenate(arrays, axis=axis)
     else:
         return ak.concatenate(arrays, axis=axis)
@@ -115,22 +119,22 @@
 
 def _p4_from_ptetaphim(pt, eta, phi, mass):
     import vector
     vector.register_awkward()
     return vector.zip({'pt': pt, 'eta': eta, 'phi': phi, 'mass': mass})
 
 
-def _get_variable_names(expr, exclude=['awkward', 'ak', 'np', 'numpy', 'math']):
+def _get_variable_names(expr, exclude=['awkward', 'ak', 'np', 'numpy', 'math', 'len']):
     import ast
     root = ast.parse(expr)
     return sorted({node.id for node in ast.walk(root) if isinstance(
         node, ast.Name) and not node.id.startswith('_')} - set(exclude))
 
 
 def _eval_expr(expr, table):
     tmp = {k: table[k] for k in _get_variable_names(expr)}
-    tmp.update({'math': math, 'np': np, 'numpy': np, 'ak': ak, 'awkward': ak,
+    tmp.update({'math': math, 'np': np, 'numpy': np, 'ak': ak, 'awkward': ak, 'len': len, '_hash': _hash,
                 '_concat': _concat, '_stack': _stack, '_pad': _pad, '_repeat_pad': _repeat_pad, '_clip': _clip,
                 '_batch_knn': _batch_knn, '_batch_permute_indices': _batch_permute_indices,
                 '_batch_argsort': _batch_argsort, '_batch_gather': _batch_gather, '_p4_from_pxpypze': _p4_from_pxpypze,
                 '_p4_from_ptetaphie': _p4_from_ptetaphie, '_p4_from_ptetaphim': _p4_from_ptetaphim})
     return eval(expr, tmp)
```

### Comparing `weaver-core-0.4.4/weaver/utils/dataset.py` & `weaver-core-0.4.5/weaver/utils/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import numpy as np
 import awkward as ak
 import torch.utils.data
 
 from functools import partial
 from concurrent.futures.thread import ThreadPoolExecutor
-from .logger import _logger, warn_once
+from .logger import _logger
 from .data.tools import _pad, _repeat_pad, _clip
 from .data.fileio import _read_files
 from .data.config import DataConfig, _md5
 from .data.preprocess import _apply_selection, _build_new_variables, _build_weights, AutoStandardizer, WeightMaker
 
 
 def _finalize_inputs(table, data_config):
@@ -78,40 +78,42 @@
             raise RuntimeError('Inconsistent label definition: some of the entries are not assigned to any classes!')
         if np.any(table['_labelcheck_'] > 1):
             raise RuntimeError('Inconsistent label definition: some of the entries are assigned to multiple classes!')
 
 
 def _preprocess(table, data_config, options):
     # apply selection
-    table = _apply_selection(table, data_config.selection if options['training'] else data_config.test_time_selection)
+    table = _apply_selection(
+        table, data_config.selection if options['training'] else data_config.test_time_selection,
+        funcs=data_config.var_funcs)
     if len(table) == 0:
         return []
     # define new variables
     table = _build_new_variables(table, data_config.var_funcs)
     # check labels
     if data_config.label_type == 'simple' and options['training']:
         _check_labels(table)
     # compute reweight indices
     if options['reweight'] and data_config.weight_name is not None:
-        wgts = _build_weights(table, data_config, warn=warn_once)
+        wgts = _build_weights(table, data_config)
         indices = _get_reweight_indices(wgts, up_sample=options['up_sample'],
                                         weight_scale=options['weight_scale'], max_resample=options['max_resample'])
     else:
         indices = np.arange(len(table[data_config.label_names[0]]))
     # shuffle
     if options['shuffle']:
         np.random.shuffle(indices)
     # perform input variable standardization, clipping, padding and stacking
     table = _finalize_inputs(table, data_config)
     return table, indices
 
 
 def _load_next(data_config, filelist, load_range, options):
-    table = _read_files(filelist, data_config.load_branches, load_range,
-                        treename=data_config.treename, branch_magic=data_config.branch_magic)
+    table = _read_files(filelist, data_config.load_branches, load_range, treename=data_config.treename,
+                        branch_magic=data_config.branch_magic, file_magic=data_config.file_magic)
     table, indices = _preprocess(table, data_config, options)
     return table, indices
 
 
 class _SimpleIter(object):
     r"""_SimpleIter
```

### Comparing `weaver-core-0.4.4/weaver/utils/flops_counter.py` & `weaver-core-0.4.5/weaver/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/utils/logger.py` & `weaver-core-0.4.5/weaver/utils/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import sys
 import os
-from functools import lru_cache
 
 
 def _configLogger(name, stdout=sys.stdout, filename=None, loglevel=logging.INFO):
     # define a Handler which writes INFO messages or higher to the sys.stdout
     logger = logging.getLogger(name)
     logger.setLevel(loglevel)
     if stdout:
@@ -72,12 +71,16 @@
         if color:
             msg = self.colorize(msg, color)
         self.logger.error(msg, *args, **kwargs)
 
 
 _logger = ColoredLogger('weaver')
 
+_warning_counter = {}
 
-@lru_cache(10)
-def warn_once(msg, logger=_logger):
-    # Keep track of 10 different messages and then warn again
-    logger.warning(msg)
+
+def warn_n_times(msg, n=10, logger=_logger):
+    if msg not in _warning_counter:
+        _warning_counter[msg] = 0
+    if _warning_counter[msg] < n:
+        logger.warning(msg)
+    _warning_counter[msg] += 1
```

### Comparing `weaver-core-0.4.4/weaver/utils/lr_finder.py` & `weaver-core-0.4.5/weaver/utils/lr_finder.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/utils/nn/metrics.py` & `weaver-core-0.4.5/weaver/utils/nn/metrics.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/utils/nn/optimizer/lookahead.py` & `weaver-core-0.4.5/weaver/utils/nn/optimizer/lookahead.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/utils/nn/optimizer/radam.py` & `weaver-core-0.4.5/weaver/utils/nn/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver/utils/nn/tools.py` & `weaver-core-0.4.5/weaver/utils/nn/tools.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.4/weaver_core.egg-info/PKG-INFO` & `weaver-core-0.4.5/weaver_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaver-core
-Version: 0.4.4
+Version: 0.4.5
 Summary: A streamlined deep-learning framework for high energy physics
 Home-page: https://github.com/hqucms/weaver-core
 Author: H. Qu, C. Li
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `weaver-core-0.4.4/weaver_core.egg-info/SOURCES.txt` & `weaver-core-0.4.5/weaver_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

