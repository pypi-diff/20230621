# Comparing `tmp/fl4health-0.1.5.tar.gz` & `tmp/fl4health-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl4health-0.1.5.tar", max compression
+gzip compressed data, was "fl4health-0.1.6.tar", max compression
```

## Comparing `fl4health-0.1.5.tar` & `fl4health-0.1.6.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     1073 2023-06-06 14:44:57.055997 fl4health-0.1.5/LICENSE
--rw-r--r--   0        0        0      439 2023-06-06 14:44:57.055997 fl4health-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/checkpointing/__init__.py
--rw-r--r--   0        0        0     2652 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/checkpointing/checkpointer.py
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/client_managers/__init__.py
--rw-r--r--   0        0        0     1645 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/client_managers/base_sampling_manager.py
--rw-r--r--   0        0        0     1355 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/client_managers/fixed_without_replacement_manager.py
--rw-r--r--   0        0        0     1724 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/client_managers/poisson_sampling_manager.py
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/__init__.py
--rw-r--r--   0        0        0     7832 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/apfl_client.py
--rw-r--r--   0        0        0     3824 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/clipping_client.py
--rw-r--r--   0        0        0     8540 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/fed_prox_client.py
--rw-r--r--   0        0        0     2953 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/numpy_fl_client.py
--rw-r--r--   0        0        0     9998 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/clients/scaffold_client.py
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/model_bases/__init__.py
--rw-r--r--   0        0        0     2487 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/model_bases/apfl_base.py
--rw-r--r--   0        0        0     2355 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/model_bases/fenda_base.py
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/__init__.py
--rw-r--r--   0        0        0     1067 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/full_exchanger.py
--rw-r--r--   0        0        0     1291 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/layer_exchanger.py
--rw-r--r--   0        0        0     1510 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/packing_exchanger.py
--rw-r--r--   0        0        0      483 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/parameter_exchange/parameter_exchanger_base.py
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/privacy/__init__.py
--rw-r--r--   0        0        0     8119 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/privacy/fl_accountants.py
--rw-r--r--   0        0        0    10562 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/privacy/moments_accountant.py
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/reporting/__init__.py
--rw-r--r--   0        0        0     6717 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/reporting/fl_wanb.py
--rw-r--r--   0        0        0     2402 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/server/polling.py
--rw-r--r--   0        0        0     2706 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/server/server.py
--rw-r--r--   0        0        0        0 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/__init__.py
--rw-r--r--   0        0        0    16868 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/client_dp_fedavgm.py
--rw-r--r--   0        0        0     5542 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/fedavg_sampling.py
--rw-r--r--   0        0        0     4448 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/noisy_aggregate.py
--rw-r--r--   0        0        0     7704 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/strategies/scaffold.py
--rw-r--r--   0        0        0     1154 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/config.py
--rw-r--r--   0        0        0     1271 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/dataset.py
--rw-r--r--   0        0        0     2437 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/load_data.py
--rw-r--r--   0        0        0     2768 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/metrics.py
--rw-r--r--   0        0        0     5399 2023-06-06 14:44:57.519998 fl4health-0.1.5/fl4health/utils/sampler.py
--rw-r--r--   0        0        0     1035 2023-06-06 14:44:57.519998 fl4health-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 fl4health-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-21 21:26:39.609131 fl4health-0.1.6/LICENSE
+-rw-r--r--   0        0        0      439 2023-06-21 21:26:39.609131 fl4health-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/checkpointing/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/checkpointing/checkpointer.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/client_managers/__init__.py
+-rw-r--r--   0        0        0     1645 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/client_managers/base_sampling_manager.py
+-rw-r--r--   0        0        0     1355 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/client_managers/fixed_without_replacement_manager.py
+-rw-r--r--   0        0        0     1724 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/client_managers/poisson_sampling_manager.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/clients/__init__.py
+-rw-r--r--   0        0        0     7840 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/clients/apfl_client.py
+-rw-r--r--   0        0        0     3824 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/clients/clipping_client.py
+-rw-r--r--   0        0        0     9838 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/clients/fed_prox_client.py
+-rw-r--r--   0        0        0     3294 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/clients/numpy_fl_client.py
+-rw-r--r--   0        0        0    10006 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/clients/scaffold_client.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/model_bases/__init__.py
+-rw-r--r--   0        0        0     2493 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/model_bases/apfl_base.py
+-rw-r--r--   0        0        0     2355 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/model_bases/fenda_base.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/parameter_exchange/__init__.py
+-rw-r--r--   0        0        0     1067 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/parameter_exchange/full_exchanger.py
+-rw-r--r--   0        0        0     3528 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/parameter_exchange/layer_exchanger.py
+-rw-r--r--   0        0        0     2792 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/parameter_exchange/packing_exchanger.py
+-rw-r--r--   0        0        0      483 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/parameter_exchange/parameter_exchanger_base.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/privacy/__init__.py
+-rw-r--r--   0        0        0     8119 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/privacy/fl_accountants.py
+-rw-r--r--   0        0        0    10562 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/privacy/moments_accountant.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/reporting/__init__.py
+-rw-r--r--   0        0        0     6717 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/reporting/fl_wanb.py
+-rw-r--r--   0        0        0     2402 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/server/polling.py
+-rw-r--r--   0        0        0     2872 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/server/server.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/strategies/__init__.py
+-rw-r--r--   0        0        0    16868 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/strategies/client_dp_fedavgm.py
+-rw-r--r--   0        0        0     4005 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/strategies/fedavg_dynamic_layer.py
+-rw-r--r--   0        0        0     5542 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/strategies/fedavg_sampling.py
+-rw-r--r--   0        0        0     4448 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/strategies/noisy_aggregate.py
+-rw-r--r--   0        0        0     7704 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/strategies/scaffold.py
+-rw-r--r--   0        0        0     1154 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/utils/config.py
+-rw-r--r--   0        0        0     1271 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/utils/dataset.py
+-rw-r--r--   0        0        0     2437 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/utils/load_data.py
+-rw-r--r--   0        0        0     6236 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/utils/metrics.py
+-rw-r--r--   0        0        0     5399 2023-06-21 21:26:40.045138 fl4health-0.1.6/fl4health/utils/sampler.py
+-rw-r--r--   0        0        0     1035 2023-06-21 21:26:40.045138 fl4health-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 fl4health-0.1.6/PKG-INFO
```

### Comparing `fl4health-0.1.5/LICENSE` & `fl4health-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/checkpointing/checkpointer.py` & `fl4health-0.1.6/fl4health/checkpointing/checkpointer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 
         # If best metric is none, then this is the first checkpoint
         return True
 
     def maybe_checkpoint(self, model: nn.Module, comparison_metric: Optional[float] = None) -> None:
         assert comparison_metric is not None
         if self._should_checkpoint(comparison_metric):
-            self.best_metric = comparison_metric
             log(
                 INFO,
                 f"Checkpointing the model: Current metric ({comparison_metric}) "
                 f"{self.comparison_str} Best metric ({self.best_metric})",
             )
+            self.best_metric = comparison_metric
             torch.save(model, self.best_checkpoint_path)
         else:
             log(
                 INFO,
                 f"Not checkpointing the model: Current metric ({comparison_metric}) is not "
                 f"{self.comparison_str} Best metric ({self.best_metric})",
             )
```

### Comparing `fl4health-0.1.5/fl4health/client_managers/base_sampling_manager.py` & `fl4health-0.1.6/fl4health/client_managers/base_sampling_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/client_managers/fixed_without_replacement_manager.py` & `fl4health-0.1.6/fl4health/client_managers/fixed_without_replacement_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/client_managers/poisson_sampling_manager.py` & `fl4health-0.1.6/fl4health/client_managers/poisson_sampling_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/clients/apfl_client.py` & `fl4health-0.1.6/fl4health/clients/apfl_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from logging import INFO
 from pathlib import Path
-from typing import Dict, List, Tuple
+from typing import Dict, Sequence, Tuple
 
 import torch
 from flwr.common.logger import log
 from flwr.common.typing import Config, NDArrays, Scalar
 from torch.nn.modules.loss import _Loss
 from torch.utils.data import DataLoader
 
@@ -13,15 +13,15 @@
 from fl4health.utils.metrics import AverageMeter, Metric
 
 
 class ApflClient(NumpyFlClient):
     def __init__(
         self,
         data_path: Path,
-        metrics: List[Metric],
+        metrics: Sequence[Metric],
         device: torch.device,
     ) -> None:
         super().__init__(data_path, device)
         self.metrics = metrics
         self.model: APFLModule
         self.train_loader: DataLoader
         self.val_loader: DataLoader
```

### Comparing `fl4health-0.1.5/fl4health/clients/clipping_client.py` & `fl4health-0.1.6/fl4health/clients/clipping_client.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/clients/fed_prox_client.py` & `fl4health-0.1.6/fl4health/clients/fed_prox_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from logging import INFO
 from pathlib import Path
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Sequence, Tuple
 
 import torch
 import torch.nn as nn
 from flwr.common.logger import log
 from flwr.common.typing import Config, NDArrays, Scalar
 from torch.nn.modules.loss import _Loss
 from torch.utils.data import DataLoader
 
 from fl4health.clients.numpy_fl_client import NumpyFlClient
-from fl4health.utils.metrics import AverageMeter, Metric
+from fl4health.utils.metrics import AverageMeter, Meter, Metric
+
+FedProxTrainStepOutputs = Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]
 
 
 class FedProxClient(NumpyFlClient):
     """
     This client implements the FedProx algorithm from Federated Optimization in Heterogeneous Networks. The idea is
     fairly straightforward. The local loss for each client is augmented with a norm on the difference between the
     local client weights during training (w) and the initial globally shared weights (w^t).
     """
 
     def __init__(
         self,
         data_path: Path,
-        metrics: List[Metric],
+        metrics: Sequence[Metric],
         device: torch.device,
     ) -> None:
         super().__init__(data_path, device)
         self.metrics = metrics
         self.model: nn.Module
         self.train_loader: DataLoader
         self.val_loader: DataLoader
@@ -35,14 +37,15 @@
         # This should be the "basic loss function" to be optimized. We'll add in the proximal term to this base
         # loss. That is, the FedProx loss becomes criterion + \mu \Vert w - w^t \Vert ^2
         self.criterion: _Loss
         self.optimizer: torch.optim.Optimizer
         self.proximal_weight: float = 0.1
         self.initial_tensors: List[torch.Tensor]
         self.total_epochs = 0
+        self.total_steps = 0
 
     def get_proximal_loss(self) -> torch.Tensor:
         assert self.initial_tensors is not None
         # Using state dictionary to ensure the same ordering as exchange
         model_weights = [layer_weights for layer_weights in self.model.parameters()]
         assert len(self.initial_tensors) == len(model_weights)
 
@@ -64,104 +67,147 @@
             initial_layer_weights.detach().clone() for initial_layer_weights in self.model.parameters()
         ]
 
     def fit(self, parameters: NDArrays, config: Config) -> Tuple[NDArrays, int, Dict[str, Scalar]]:
         if not self.initialized:
             self.setup_client(config)
 
+        meter = AverageMeter(self.metrics, "train_meter")
         self.set_parameters(parameters, config)
         local_epochs = self.narrow_config_type(config, "local_epochs", int)
         current_server_round = self.narrow_config_type(config, "current_server_round", int)
-        metric_values = self.train(current_server_round, local_epochs)
+        # Currently uses training by epoch.
+        metric_values = self.train_by_epochs(current_server_round, local_epochs, meter)
         # FitRes should contain local parameters, number of examples on client, and a dictionary holding metrics
         # calculation results.
         return (
             self.get_parameters(config),
             self.num_examples["train_set"],
             metric_values,
         )
 
     def evaluate(self, parameters: NDArrays, config: Config) -> Tuple[float, int, Dict[str, Scalar]]:
         if not self.initialized:
             self.setup_client(config)
 
         self.set_parameters(parameters, config)
         current_server_round = self.narrow_config_type(config, "current_server_round", int)
-        loss, metric_values = self.validate(current_server_round)
+        meter = AverageMeter(self.metrics, "val_meter")
+        loss, metric_values = self.validate(current_server_round, meter)
         # EvaluateRes should return the loss, number of examples on client, and a dictionary holding metrics
         # calculation results.
         return (
             loss,
             self.num_examples["validation_set"],
             metric_values,
         )
 
-    def _maybe_log_train_metrics(
-        self, server_round: int, losses: Dict[str, float], metrics: Dict[str, Scalar]
-    ) -> None:
-        if self.wandb_reporter:
-            to_log: Dict[str, Any] = {"epoch": self.total_epochs}
-            to_log["server_round"] = server_round
-            to_log.update(losses)
-            to_log.update(metrics)
-            self.wandb_reporter.report_metrics(to_log)
-
-    def _maybe_log_eval_metrics(self, server_round: int, losses: Dict[str, float], metrics: Dict[str, Scalar]) -> None:
-        if self.wandb_reporter:
-            to_log: Dict[str, Any] = {"server_round": server_round}
-            to_log.update(losses)
-            to_log.update(metrics)
-            self.wandb_reporter.report_metrics(to_log)
+    def _handle_reporting(
+        self,
+        to_log: Dict[str, Any],
+        meter: Meter,
+        loss_dict: Dict[str, float],
+        steps_taken: int,
+        is_validation: bool = False,
+    ) -> Tuple[Dict[str, Scalar], Dict[str, float]]:
+        # Average loss per step per loss component
+        loss_dict = {key: val / steps_taken for key, val in loss_dict.items()}
+
+        metrics = meter.compute()
+        loss_string = "\t".join([f"{key}: {str(val)}" for key, val in loss_dict.items()])
+        metric_string = "\t".join([f"{key}: {str(val)}" for key, val in metrics.items()])
+        metric_prefix = "Validation" if is_validation else "Training"
+        log(
+            INFO,
+            f"Client {metric_prefix} Losses: {loss_string} \n" f"Client {metric_prefix} Metrics: {metric_string}",
+        )
+        to_log.update(loss_dict)
+        to_log.update(metrics)
+        self._maybe_log_metrics(to_log)
+        return metrics, loss_dict
+
+    def train_step(self, input: torch.Tensor, target: torch.Tensor) -> FedProxTrainStepOutputs:
+        # forward pass on the model
+        preds = self.model(input)
+        vanilla_loss = self.criterion(preds, target)
+        proximal_loss = self.get_proximal_loss()
+        fed_prox_loss = vanilla_loss + proximal_loss
+
+        self.optimizer.zero_grad()
+        fed_prox_loss.backward()
+        self.optimizer.step()
+
+        return vanilla_loss, proximal_loss, fed_prox_loss, preds
 
-    def train(
+    def train_by_steps(
+        self,
+        current_server_round: int,
+        steps: int,
+        meter: Meter,
+    ) -> Dict[str, Scalar]:
+        self.model.train()
+        loss_dict = {"train_vanilla_loss": 0.0, "train_proximal_loss": 0.0, "train_total_loss": 0.0}
+        train_iterator = iter(self.train_loader)
+
+        for _ in range(steps):
+            self.total_steps += 1
+            try:
+                input, target = next(train_iterator)
+            except StopIteration:
+                # StopIteration is thrown if dataset ends
+                # reinitialize data loader
+                train_iterator = iter(self.train_loader)
+                input, target = next(train_iterator)
+
+            input, target = input.to(self.device), target.to(self.device)
+            vanilla_loss, proximal_loss, fed_prox_loss, preds = self.train_step(input, target)
+
+            loss_dict["train_vanilla_loss"] += vanilla_loss.item()
+            loss_dict["train_proximal_loss"] += proximal_loss.item()
+            loss_dict["train_total_loss"] += fed_prox_loss.item()
+
+            meter.update(preds, target)
+
+        custom_log: Dict[str, Any] = {"step": self.total_steps, "server_round": current_server_round}
+        metrics, _ = self._handle_reporting(custom_log, meter, loss_dict, steps)
+
+        # return final training metrics
+        return metrics
+
+    def train_by_epochs(
         self,
         current_server_round: int,
         epochs: int,
+        meter: Meter,
     ) -> Dict[str, Scalar]:
-        for epoch in range(epochs):
+        self.model.train()
+
+        for local_epoch in range(epochs):
+            meter.clear()
             self.total_epochs += 1
-            meter = AverageMeter(self.metrics, "train_meter")
             loss_dict = {"train_vanilla_loss": 0.0, "train_proximal_loss": 0.0, "train_total_loss": 0.0}
             for input, target in self.train_loader:
                 input, target = input.to(self.device), target.to(self.device)
-                # forward pass on the model
-                preds = self.model(input)
-                vanilla_loss = self.criterion(preds, target)
-                proximal_loss = self.get_proximal_loss()
-                fed_prox_loss = vanilla_loss + proximal_loss
-
-                self.optimizer.zero_grad()
-                fed_prox_loss.backward()
-                self.optimizer.step()
+                vanilla_loss, proximal_loss, fed_prox_loss, preds = self.train_step(input, target)
 
                 loss_dict["train_vanilla_loss"] += vanilla_loss.item()
                 loss_dict["train_proximal_loss"] += proximal_loss.item()
                 loss_dict["train_total_loss"] += fed_prox_loss.item()
 
                 meter.update(preds, target)
 
-            # Average loss per step per loss component
-            loss_dict = {key: val / len(self.train_loader) for key, val in loss_dict.items()}
-
-            training_metrics = meter.compute()
-            metrics: Dict[str, Scalar] = {**training_metrics}
-            train_loss_string = "\t".join([f"{key}: {str(val)}" for key, val in loss_dict.items()])
-            train_metric_string = "\t".join([f"{key}: {str(val)}" for key, val in metrics.items()])
-            log(
-                INFO,
-                f"Epoch: {epoch}\n"
-                f"Client Training Losses: {train_loss_string} \n"
-                f"Client Training Metrics: {train_metric_string}",
-            )
-            self._maybe_log_train_metrics(current_server_round, loss_dict, metrics)
+            log(INFO, f"Local Epoch: {local_epoch}")
+            custom_log: Dict[str, Any] = {"epoch": self.total_epochs, "server_round": current_server_round}
+            metrics, _ = self._handle_reporting(custom_log, meter, loss_dict, len(self.train_loader))
 
+        # Return final training metrics
         return metrics
 
-    def validate(self, current_server_round: int) -> Tuple[float, Dict[str, Scalar]]:
-        meter = AverageMeter(self.metrics, "val_meter")
+    def validate(self, current_server_round: int, meter: Meter) -> Tuple[float, Dict[str, Scalar]]:
+        self.model.eval()
         loss_dict = {"val_vanilla_loss": 0.0, "val_proximal_loss": 0.0, "val_total_loss": 0.0}
 
         with torch.no_grad():
             for input, target in self.val_loader:
                 input, target = input.to(self.device), target.to(self.device)
 
                 preds = self.model(input)
@@ -171,19 +217,16 @@
 
                 loss_dict["val_vanilla_loss"] += vanilla_loss.item()
                 loss_dict["val_proximal_loss"] += proximal_loss.item()
                 loss_dict["val_total_loss"] += fed_prox_loss.item()
 
                 meter.update(preds, target)
 
-        # Average loss per step per loss component
-        loss_dict = {key: val / len(self.val_loader) for key, val in loss_dict.items()}
-        validation_metrics = meter.compute()
-        metrics: Dict[str, Scalar] = {**validation_metrics}
-        val_loss_string = "\t".join([f"{key}: {str(val)}" for key, val in loss_dict.items()])
-        val_metric_string = "\t".join([f"{key}: {str(val)}" for key, val in metrics.items()])
-        log(
-            INFO,
-            "\n" f"Client Validation Losses: {val_loss_string} \n" f"Client validation Metrics: {val_metric_string}",
+        custom_log: Dict[str, Any] = {"server_round": current_server_round}
+        metrics, loss_per_step = self._handle_reporting(
+            custom_log, meter, loss_dict, len(self.val_loader), is_validation=True
         )
-        self._maybe_log_eval_metrics(current_server_round, loss_dict, metrics)
-        return loss_dict["val_total_loss"], metrics
+
+        val_loss_per_step = loss_per_step["val_total_loss"]
+        self._maybe_checkpoint(val_loss_per_step)
+
+        return val_loss_per_step, metrics
```

### Comparing `fl4health-0.1.5/fl4health/clients/numpy_fl_client.py` & `fl4health-0.1.6/fl4health/clients/numpy_fl_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import string
 from pathlib import Path
-from typing import Optional, Type, TypeVar
+from typing import Any, Dict, Optional, Type, TypeVar
 
 import torch
 import torch.nn as nn
 from flwr.client import NumPyClient
 from flwr.common import Config, NDArrays
 
 from fl4health.checkpointing.checkpointer import TorchCheckpointer
@@ -27,14 +27,22 @@
         self.initial_weights: Optional[NDArrays] = None
         self.wandb_reporter: Optional[ClientWandBReporter] = None
         self.checkpointer: Optional[TorchCheckpointer] = None
 
     def generate_hash(self, length: int = 8) -> str:
         return "".join(random.choice(string.ascii_lowercase) for i in range(length))
 
+    def _maybe_log_metrics(self, to_log: Dict[str, Any]) -> None:
+        if self.wandb_reporter:
+            self.wandb_reporter.report_metrics(to_log)
+
+    def _maybe_checkpoint(self, comparison_metric: float) -> None:
+        if self.checkpointer:
+            self.checkpointer.maybe_checkpoint(self.model, comparison_metric)
+
     def setup_client(self, config: Config) -> None:
         """
         This method should be used to set up all of the required components for the client through the config passed
         by the server and need only be done once. The quintessential example is data loaders with a batch size set by
         the server in the config. The parameter initialized should be set to true when this function is finished.
         Overriding this class and calling super is the preferred flow.
         """
```

### Comparing `fl4health-0.1.5/fl4health/clients/scaffold_client.py` & `fl4health-0.1.6/fl4health/clients/scaffold_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from logging import INFO
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, Optional, Sequence, Tuple
 
 import numpy as np
 import torch
 import torch.nn as nn
 from flwr.common.logger import log
 from flwr.common.typing import Config, NDArrays, Scalar
 from torch.nn.modules.loss import _Loss
@@ -18,15 +18,15 @@
 class ScaffoldClient(NumpyFlClient):
     """
     Federated Learning Client for Scaffold strategy.
 
     Implementation based on https://arxiv.org/pdf/1910.06378.pdf.
     """
 
-    def __init__(self, data_path: Path, metrics: List[Metric], device: torch.device) -> None:
+    def __init__(self, data_path: Path, metrics: Sequence[Metric], device: torch.device) -> None:
         super().__init__(data_path, device)
         self.metrics = metrics
         self.client_control_variates: Optional[NDArrays] = None  # c_i in paper
         self.client_control_variates_updates: Optional[NDArrays] = None  # delta_c_i in paper
         self.server_control_variates: Optional[NDArrays] = None  # c in paper
         self.model: nn.Module
         self.train_loader: DataLoader
```

### Comparing `fl4health-0.1.5/fl4health/model_bases/apfl_base.py` & `fl4health-0.1.6/fl4health/model_bases/apfl_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         grad_alpha: float = 0.0
         for local_p, global_p in zip(self.local_model.parameters(), self.global_model.parameters()):
             local_grad = local_p.grad
             global_grad = global_p.grad
             assert local_grad is not None and global_grad is not None
             dif = local_p - global_p
             grad = torch.tensor(self.alpha) * local_grad + torch.tensor(1.0 - self.alpha) * global_grad
-            grad_alpha += torch.mul(dif, grad).sum().detach().numpy()
+            grad_alpha += torch.mul(dif, grad).sum().detach().cpu().numpy()
 
         # This update constant of 0.02 is not referenced in the paper
         # but is present in the official implementation and other ones I have seen
         # Not sure its function, just adding a number proportional to alpha to the grad
         # Leaving in for consistency with official implementation
         grad_alpha += 0.02 * self.alpha
         alpha = self.alpha - self.alpha_lr * grad_alpha
```

### Comparing `fl4health-0.1.5/fl4health/model_bases/fenda_base.py` & `fl4health-0.1.6/fl4health/model_bases/fenda_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/parameter_exchange/full_exchanger.py` & `fl4health-0.1.6/fl4health/parameter_exchange/full_exchanger.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/parameter_exchange/packing_exchanger.py` & `fl4health-0.1.6/fl4health/parameter_exchange/packing_exchanger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from typing import Tuple, Union
+from typing import Optional, Tuple, Union
 
 import numpy as np
-from flwr.common.typing import NDArrays
+import torch
+import torch.nn as nn
+from flwr.common.typing import Config, List, NDArrays
 
 from fl4health.parameter_exchange.full_exchanger import FullParameterExchanger
 
 
 class ParameterExchangerWithPacking(FullParameterExchanger):
     def pack_parameters(self, model_weights: NDArrays, additional_parameters: Union[NDArrays, float]) -> NDArrays:
         if isinstance(additional_parameters, float):
@@ -26,7 +28,30 @@
 class ParameterExchangerWithClippingBit(ParameterExchangerWithPacking):
     def unpack_parameters(self, packed_parameters: NDArrays) -> Tuple[NDArrays, float]:
         # The last entry in the parameters list is assumed to be a clipping bound (even if we're evaluating)
         split_size = len(packed_parameters) - 1
         model_parameters = packed_parameters[:split_size]
         clipping_bound = float(packed_parameters[split_size:][0])
         return model_parameters, clipping_bound
+
+
+class ParameterExchangerWithLayerNames(ParameterExchangerWithPacking):
+    def pack_parameters(self, model_weights: NDArrays, weights_names: Union[NDArrays, float, List[str]]) -> NDArrays:
+        return model_weights + [np.array(weights_names)]
+
+    def unpack_parameters(self, packed_parameters: NDArrays) -> Tuple[NDArrays, List[str]]:
+        """
+        Assumption: packed_parameters is a list containing model parameters followed by an NDArray that contains the
+        corresponding names of those parameters.
+        """
+        split_size = len(packed_parameters) - 1
+        model_parameters = packed_parameters[:split_size]
+        param_names = packed_parameters[split_size:][0].tolist()
+        return model_parameters, param_names
+
+    def pull_parameters(self, parameters: NDArrays, model: nn.Module, config: Optional[Config] = None) -> None:
+        current_state = model.state_dict()
+        # update the correct layers to new parameters
+        layer_params, layer_names = self.unpack_parameters(parameters)
+        for layer_name, layer_param in zip(layer_names, layer_params):
+            current_state[layer_name] = torch.tensor(layer_param)
+        model.load_state_dict(current_state, strict=True)
```

### Comparing `fl4health-0.1.5/fl4health/privacy/fl_accountants.py` & `fl4health-0.1.6/fl4health/privacy/fl_accountants.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/privacy/moments_accountant.py` & `fl4health-0.1.6/fl4health/privacy/moments_accountant.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/reporting/fl_wanb.py` & `fl4health-0.1.6/fl4health/reporting/fl_wanb.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/server/polling.py` & `fl4health-0.1.6/fl4health/server/polling.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/server/server.py` & `fl4health-0.1.6/fl4health/server/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from flwr.common.logger import log
 from flwr.server.client_manager import ClientManager
 from flwr.server.history import History
 from flwr.server.server import Server
 from flwr.server.strategy import Strategy
 
+from fl4health.checkpointing.checkpointer import TorchCheckpointer
 from fl4health.reporting.fl_wanb import ServerWandBReporter
 from fl4health.server.polling import poll_clients
 from fl4health.strategies.client_dp_fedavgm import ClientLevelDPFedAvgM
 
 
 class FlServer(Server):
     """
@@ -18,17 +19,19 @@
     """
 
     def __init__(
         self,
         client_manager: ClientManager,
         strategy: Optional[Strategy] = None,
         wandb_reporter: Optional[ServerWandBReporter] = None,
+        checkpointer: Optional[TorchCheckpointer] = None,
     ) -> None:
         super().__init__(client_manager=client_manager, strategy=strategy)
         self.wandb_reporter = wandb_reporter
+        self.checkpointer = checkpointer
 
     def fit(self, num_rounds: int, timeout: Optional[float]) -> History:
         history = super().fit(num_rounds, timeout)
         if self.wandb_reporter:
             # report history to W and B
             self.wandb_reporter.report_metrics(num_rounds, history)
         return history
```

### Comparing `fl4health-0.1.5/fl4health/strategies/client_dp_fedavgm.py` & `fl4health-0.1.6/fl4health/strategies/client_dp_fedavgm.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/strategies/fedavg_sampling.py` & `fl4health-0.1.6/fl4health/strategies/fedavg_sampling.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/strategies/noisy_aggregate.py` & `fl4health-0.1.6/fl4health/strategies/noisy_aggregate.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/strategies/scaffold.py` & `fl4health-0.1.6/fl4health/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/utils/config.py` & `fl4health-0.1.6/fl4health/utils/config.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/utils/dataset.py` & `fl4health-0.1.6/fl4health/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/utils/load_data.py` & `fl4health-0.1.6/fl4health/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/fl4health/utils/sampler.py` & `fl4health-0.1.6/fl4health/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.5/pyproject.toml` & `fl4health-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fl4health"
-version = "0.1.5"
+version = "0.1.6"
 description = "Federated Learning for Health"
 authors = ["Vector AI Engineering <fl4health@vectorinstitute.ai>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `fl4health-0.1.5/PKG-INFO` & `fl4health-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl4health
-Version: 0.1.5
+Version: 0.1.6
 Summary: Federated Learning for Health
 License: MIT
 Author: Vector AI Engineering
 Author-email: fl4health@vectorinstitute.ai
 Requires-Python: >=3.9.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

