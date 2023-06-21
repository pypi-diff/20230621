# Comparing `tmp/mmenot-0.9.2-py3-none-any.whl.zip` & `tmp/mmenot-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,24 @@
-Zip file size: 24434 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-May-23 15:58 mmenot/__init__.py
--rw-r--r--  2.0 unx     2977 b- defN 23-May-23 12:05 mmenot/exporter.py
--rw-r--r--  2.0 unx     5553 b- defN 23-May-23 12:05 mmenot/labels.py
--rw-r--r--  2.0 unx     6060 b- defN 23-May-23 12:05 mmenot/loops.py
--rw-r--r--  2.0 unx     1456 b- defN 23-May-23 12:05 mmenot/patches.py
--rw-r--r--  2.0 unx     5726 b- defN 23-May-23 12:05 mmenot/pruner.py
--rw-r--r--  2.0 unx      633 b- defN 23-May-23 12:05 mmenot/runner.py
--rw-r--r--  2.0 unx     3074 b- defN 23-May-23 12:05 mmenot/tester.py
--rw-r--r--  2.0 unx     5030 b- defN 23-May-23 12:05 mmenot/trainer.py
--rw-r--r--  2.0 unx    11727 b- defN 23-May-23 15:48 mmenot/utils.py
--rw-rw-rw-  2.0 unx    11338 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    14257 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1208 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/RECORD
-16 files, 69277 bytes uncompressed, 22482 bytes compressed:  67.5%
+Zip file size: 28770 bytes, number of entries: 22
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 07:40 __init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 07:40 mmenot/__init__.py
+-rw-r--r--  2.0 unx     2984 b- defN 23-Jun-06 11:15 mmenot/exporter.py
+-rw-r--r--  2.0 unx     4675 b- defN 23-Jun-20 02:58 mmenot/hyp_searcher.py
+-rw-r--r--  2.0 unx     5567 b- defN 23-Jun-06 11:15 mmenot/labels.py
+-rw-r--r--  2.0 unx     1454 b- defN 23-Jun-02 17:43 mmenot/patches.py
+-rw-r--r--  2.0 unx     5732 b- defN 23-Jun-05 06:33 mmenot/pruner.py
+-rw-r--r--  2.0 unx      689 b- defN 23-Jun-05 06:33 mmenot/runner.py
+-rw-r--r--  2.0 unx     3081 b- defN 23-Jun-06 11:15 mmenot/tester.py
+-rw-r--r--  2.0 unx     5044 b- defN 23-Jun-06 11:15 mmenot/trainer.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-02 17:47 mmenot/loops/__init__.py
+-rw-r--r--  2.0 unx     2700 b- defN 23-Jun-06 11:35 mmenot/loops/epoch_optuna.py
+-rw-r--r--  2.0 unx     6075 b- defN 23-Jun-06 11:15 mmenot/loops/epoch_pruning.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 07:40 mmenot/utils/__init__.py
+-rw-r--r--  2.0 unx    11727 b- defN 23-Jun-06 11:15 mmenot/utils/common.py
+-rw-r--r--  2.0 unx     1742 b- defN 23-Jun-20 02:58 mmenot/utils/hpo.py
+-rw-rw-rw-  2.0 unx    11338 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14279 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1693 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/RECORD
+22 files, 79187 bytes uncompressed, 26064 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,17 +1,20 @@
+Filename: __init__.py
+Comment: 
+
 Filename: mmenot/__init__.py
 Comment: 
 
 Filename: mmenot/exporter.py
 Comment: 
 
-Filename: mmenot/labels.py
+Filename: mmenot/hyp_searcher.py
 Comment: 
 
-Filename: mmenot/loops.py
+Filename: mmenot/labels.py
 Comment: 
 
 Filename: mmenot/patches.py
 Comment: 
 
 Filename: mmenot/pruner.py
 Comment: 
@@ -21,29 +24,44 @@
 
 Filename: mmenot/tester.py
 Comment: 
 
 Filename: mmenot/trainer.py
 Comment: 
 
-Filename: mmenot/utils.py
+Filename: mmenot/loops/__init__.py
+Comment: 
+
+Filename: mmenot/loops/epoch_optuna.py
+Comment: 
+
+Filename: mmenot/loops/epoch_pruning.py
+Comment: 
+
+Filename: mmenot/utils/__init__.py
+Comment: 
+
+Filename: mmenot/utils/common.py
+Comment: 
+
+Filename: mmenot/utils/hpo.py
 Comment: 
 
-Filename: mmenot-0.9.2.dist-info/LICENSE
+Filename: mmenot-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: mmenot-0.9.2.dist-info/METADATA
+Filename: mmenot-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: mmenot-0.9.2.dist-info/WHEEL
+Filename: mmenot-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: mmenot-0.9.2.dist-info/entry_points.txt
+Filename: mmenot-0.9.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: mmenot-0.9.2.dist-info/top_level.txt
+Filename: mmenot-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mmenot-0.9.2.dist-info/RECORD
+Filename: mmenot-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mmenot/exporter.py

```diff
@@ -8,15 +8,15 @@
 from mmdeploy.apis import torch2onnx
 from mmdeploy.codebase.base.task import BaseTask
 from mmdeploy.utils import get_ir_config
 from mmdeploy.utils import get_partition_config
 from mmdeploy.utils import get_root_logger
 from mmdeploy.utils import load_config
 
-from mmenot.utils import load_model_from_checkpoint
+from mmenot.utils.common import load_model_from_checkpoint
 
 BaseTask.build_pytorch_model = load_model_from_checkpoint
 
 
 def parse_args():  # pylint: disable=missing-function-docstring
     parser = argparse.ArgumentParser(description='Export model to ONNX.')
     parser.add_argument('deploy_cfg', help='deploy config path')
```

## mmenot/labels.py

```diff
@@ -11,16 +11,16 @@
 from enot.pruning.labels import Label
 from enot.pruning.prune import prune_model
 from enot.pruning.pruning_info import ModelPruningInfo
 from enot_latency_server.client import measure_latency_remote
 from mmengine.logging.logger import MMLogger
 from torch import nn
 
-from mmenot.utils import count_mmac
-from mmenot.utils import export_to_onnx
+from mmenot.utils.common import count_mmac
+from mmenot.utils.common import export_to_onnx
 
 
 def labels_equal(pruning_info: ModelPruningInfo, parameter: float, **kwargs) -> List[Label]:
     del kwargs
     if not 0 < parameter < 1:
         raise ValueError(f'Pruning parameter should be in range (0, 1), got {parameter}')
```

## mmenot/patches.py

```diff
@@ -4,15 +4,17 @@
 from torch import Tensor
 from torch import nn
 
 
 def loss_by_feat(self, seg_logits: Tensor, batch_data_samples: SampleList) -> dict:
     """
     Patch for mmseg.models.decode_heads.decode_head.BaseDecodeHead.loss_by_feat:
-        removed one line: loss['acc_seg'] = accuracy(seg_logits, seg_label, ignore_index=self.ignore_index)
+
+    removed one line: loss['acc_seg'] = accuracy(seg_logits, seg_label, ignore_index=self.ignore_index)
+
     """
     seg_label = self._stack_batch_gt(batch_data_samples)  # pylint: disable=W0212
     loss = {}
     seg_logits = resize(
         input=seg_logits,
         size=seg_label.shape[2:],
         mode='bilinear',
```

## mmenot/pruner.py

```diff
@@ -2,15 +2,15 @@
 import os.path as osp
 
 import torch
 from mmengine.config import Config
 from mmengine.config import DictAction
 
 from mmenot.loops import EpochBasedPruningLoop  # pylint: disable=unused-import
-from mmenot.runner import PruningRunner
+from mmenot.runner import CheckpointRunner
 
 # apply patches.
 try:
     # pylint: disable=C0412
     import mmseg.models.decode_heads.decode_head
 
     from mmenot.patches import loss_by_feat
@@ -139,13 +139,13 @@
     cfg['train_cfg']['port'] = args.port
     cfg['train_cfg']['endpoint'] = args.endpoint
     cfg['train_cfg']['deploy_cfg'] = args.deploy_cfg
     cfg['train_cfg']['model_cfg'] = args.config
     cfg['train_cfg']['type'] = 'EpochBasedPruningLoop'
     cfg['train_cfg'].pop('max_iters', None)  # remove max_iters for EpochBasedPruningLoop
 
-    runner = PruningRunner.from_cfg(cfg)
+    runner = CheckpointRunner.from_cfg(cfg)
     runner.train()
 
 
 if __name__ == '__main__':
     prune()
```

## mmenot/runner.py

```diff
@@ -8,16 +8,16 @@
 from mmengine.runner import Runner
 from torch import nn
 
 ConfigType = Union[Dict, Config, ConfigDict]
 
 
 @RUNNERS.register_module()
-class PruningRunner(Runner):
-    """Pruning runner"""
+class CheckpointRunner(Runner):
+    """Patched runner: it can load model from checkpoint (not state dict)."""
 
     def __init__(self, model: Union[nn.Module, Dict, str], *args, **kwargs):
         if isinstance(model, str):
             model = torch.load(model, map_location='cpu')
 
         assert isinstance(model, (nn.Module, Dict))
         super().__init__(model, *args, **kwargs)
```

## mmenot/tester.py

```diff
@@ -3,15 +3,15 @@
 import os.path as osp
 
 from mmengine.config import Config
 from mmengine.config import DictAction
 from mmengine.registry import RUNNERS
 from mmengine.runner import Runner
 
-from mmenot.utils import from_cfg
+from mmenot.utils.common import from_cfg
 
 Runner.from_cfg = classmethod(from_cfg)  # type: ignore
 
 
 def parse_args():  # pylint: disable=missing-function-docstring
     parser = argparse.ArgumentParser(description='Test (and eval) a model')
     parser.add_argument('config', help='test config file path')
```

## mmenot/trainer.py

```diff
@@ -5,16 +5,16 @@
 
 from mmengine.config import Config
 from mmengine.config import DictAction
 from mmengine.logging import print_log
 from mmengine.registry import RUNNERS
 from mmengine.runner import Runner
 
-from mmenot.utils import from_cfg
-from mmenot.utils import runner_save_checkpoint
+from mmenot.utils.common import from_cfg
+from mmenot.utils.common import runner_save_checkpoint
 
 Runner.from_cfg = classmethod(from_cfg)  # type: ignore
 Runner.save_checkpoint = runner_save_checkpoint
 
 
 def parse_args():  # pylint: disable=missing-function-docstring
     parser = argparse.ArgumentParser(description='Tune a model')
```

## Comparing `mmenot/loops.py` & `mmenot/loops/epoch_pruning.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 
 from mmenot.labels import labels_equal
 from mmenot.labels import labels_global_channels
 from mmenot.labels import labels_global_mmacs
 from mmenot.labels import labels_global_ratio
 from mmenot.labels import labels_global_threshold
 from mmenot.labels import labels_optimal_hw_aware
-from mmenot.utils import check_latency_server
-from mmenot.utils import count_mmac
+from mmenot.utils.common import check_latency_server
+from mmenot.utils.common import count_mmac
 
 
 @LOOPS.register_module()
 class EpochBasedPruningLoop(EpochBasedTrainLoop):
     """
     Pruning loop.
 
     Calibrates and prunes model on one epoch.
+
     """
 
     _LABEL_SELECTOR_REGISTRY: Dict[str, Callable[..., List[Label]]] = {
         'equal': labels_equal,
         'global': labels_global_ratio,
         'global-mmacs': labels_global_mmacs,
         'optimal-hw-aware': labels_optimal_hw_aware,
```

## Comparing `mmenot/utils.py` & `mmenot/utils/common.py`

 * *Files identical despite different names*

## Comparing `mmenot-0.9.2.dist-info/LICENSE` & `mmenot-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mmenot-0.9.2.dist-info/METADATA` & `mmenot-0.9.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmenot
-Version: 0.9.2
+Version: 0.9.3
 Summary: ENOT Framework integration package for OpenMMLab codebase
 Author-email: ENOT LLC <enot@enot.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,14 +220,15 @@
 Requires-Dist: mmengine (>=0.7.2)
 Requires-Dist: mmcv (>=2.0.0)
 Requires-Dist: mmdeploy (>=1.0.0)
 Requires-Dist: onnx
 Requires-Dist: numpy
 Requires-Dist: enot-latency-server
 Requires-Dist: enot-autodl
+Requires-Dist: optuna
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Provides-Extra: mmdet
 Requires-Dist: mmdet (>=3.0.0) ; extra == 'mmdet'
```

