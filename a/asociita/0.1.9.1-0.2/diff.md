# Comparing `tmp/asociita-0.1.9.1.tar.gz` & `tmp/asociita-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.9.1.tar", max compression
+gzip compressed data, was "asociita-0.2.tar", max compression
```

## Comparing `asociita-0.1.9.1.tar` & `asociita-0.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.1.9.1/LICENSE
--rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.1.9.1/README.md
--rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.1.9.1/asociita/__init__.py
--rw-r--r--   0        0        0     3881 2023-05-29 08:30:33.477904 asociita-0.1.9.1/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0     6970 2023-06-05 13:24:07.885952 asociita-0.1.9.1/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.1.9.1/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0     9972 2023-06-05 09:45:20.347198 asociita-0.1.9.1/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     2106 2023-06-05 13:51:59.255884 asociita-0.1.9.1/asociita/components/evaluator/sample_evaluator.py
--rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.1.9.1/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7549 2023-06-06 11:41:23.091887 asociita-0.1.9.1/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6226 2023-06-06 11:42:03.726476 asociita-0.1.9.1/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11069 2023-06-06 11:35:25.808272 asociita-0.1.9.1/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.1.9.1/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.1.9.1/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.1.9.1/asociita/datasets/load_fmnist.py
--rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.1.9.1/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.1.9.1/asociita/datasets/save_blueprint.py
--rw-r--r--   0        0        0     6838 2023-06-09 14:54:11.498938 asociita-0.1.9.1/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     5962 2023-05-30 10:15:28.967345 asociita-0.1.9.1/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.1.9.1/asociita/exceptions/evaluatorexception.py
--rw-r--r--   0        0        0      322 2023-05-29 08:30:33.477904 asociita-0.1.9.1/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    14810 2023-06-06 11:35:25.808272 asociita-0.1.9.1/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.1.9.1/asociita/models/pytorch/fmnist.py
--rw-r--r--   0        0        0      934 2023-05-31 13:26:40.943955 asociita-0.1.9.1/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     5918 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/computations.py
--rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/handlers.py
--rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.1.9.1/asociita/utils/loggers.py
--rw-r--r--   0        0        0     7791 2023-06-05 13:21:15.847962 asociita-0.1.9.1/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.1.9.1/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/showcase.py
--rw-r--r--   0        0        0      680 2023-06-09 14:54:34.742141 asociita-0.1.9.1/pyproject.toml
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 asociita-0.1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.2/LICENSE
+-rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.2/asociita/__init__.py
+-rw-r--r--   0        0        0     4435 2023-06-16 21:02:52.738641 asociita-0.2/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0    15227 2023-06-21 15:13:38.758846 asociita-0.2/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.2/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0     9972 2023-06-16 21:38:55.086092 asociita-0.2/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0    18039 2023-06-21 14:31:19.790585 asociita-0.2/asociita/components/evaluator/sample_evaluator.py
+-rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.2/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     8760 2023-06-21 09:00:59.361644 asociita-0.2/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6992 2023-06-21 09:00:53.701835 asociita-0.2/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    10764 2023-06-21 09:00:46.666073 asociita-0.2/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     4414 2023-06-16 21:28:46.480533 asociita-0.2/asociita/components/settings/settings.py
+-rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.2/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.2/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.2/asociita/datasets/load_fmnist.py
+-rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.2/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.2/asociita/datasets/save_blueprint.py
+-rw-r--r--   0        0        0     6838 2023-06-09 14:54:11.498938 asociita-0.2/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     5962 2023-06-14 13:53:33.877567 asociita-0.2/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.2/asociita/exceptions/evaluatorexception.py
+-rw-r--r--   0        0        0       93 2023-06-16 11:49:20.285800 asociita-0.2/asociita/exceptions/modelexception.py
+-rw-r--r--   0        0        0      420 2023-06-15 21:36:35.590719 asociita-0.2/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.2/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    16485 2023-06-16 11:50:05.308269 asociita-0.2/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.2/asociita/models/pytorch/fmnist.py
+-rw-r--r--   0        0        0     5260 2023-06-14 08:05:45.666579 asociita-0.2/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6097 2023-06-21 09:19:46.159500 asociita-0.2/asociita/utils/computations.py
+-rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.2/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.2/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.2/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.2/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     7791 2023-06-05 13:21:15.847962 asociita-0.2/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.2/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.2/asociita/utils/showcase.py
+-rw-r--r--   0        0        0      676 2023-06-21 15:19:28.527006 asociita-0.2/pyproject.toml
+-rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 asociita-0.2/PKG-INFO
```

### Comparing `asociita-0.1.9.1/LICENSE` & `asociita-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/README.md` & `asociita-0.2/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/components/archiver/archive_manager.py` & `asociita-0.2/asociita/components/archiver/archive_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from asociita.models.pytorch.federated_model import FederatedModel
 from asociita.utils.handlers import Handler
 import os
 
 class Archive_Manager():
     def __init__(self,
                  archive_manager: dict,
-                 logger) -> None:
+                 logger = None) -> None:
         try:
             # Modes
             self.orchestrator_metrics = archive_manager["orchestrator"]
             self.clients_on_central = archive_manager["clients_on_central"]
             self.central_on_local = archive_manager["central_on_local"]
             self.save_results = archive_manager["save_results"]
             if self.save_results:
@@ -28,17 +28,20 @@
             self.central_on_local_file = archive_manager["central_on_local_filename"]
 
             # Paths for preserving models
             self.orchestrator_save_path = archive_manager["orchestrator_model_save_path"]
             self.nodes_save_path = archive_manager["nodes_model_save_path"]
 
         except ArchiverSettingsException:
-            raise ArchiverSettingsException
+            raise ArchiverSettingsException('The dictionary passed to the Archiver does not contain all the necessary key-words '/
+                                            "The Dictionary should contain following key-items pairs: {orchestrator: bool," /
+                                            "clients_on_central: bool, central_on_local: bool, save_results: bool, log_results: bool}")
         
-        self.logger = logger
+        if logger != None:
+            self.logger = logger
     
     def archive_training_results(self,
                         iteration: int,
                         central_model: FederatedModel,
                         nodes: list[FederatedModel]
     ):
         if self.orchestrator_metrics:
@@ -72,8 +75,14 @@
                                               model = node.model,
                                               logger = self.logger)
                 
                 if self.nodes_save_path:
                     for node in nodes:
                         node.store_model_on_disk(iteration = iteration,
                                                  path = self.nodes_save_path)
+    
+    def archive_contribution_results(self,
+                                     results: dict,
+                                     mapping: list):
+        pass
+
```

### Comparing `asociita-0.1.9.1/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.2/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/components/evaluator/or_evaluator.py` & `asociita-0.2/asociita/components/evaluator/or_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,25 +127,25 @@
                 subset_with_i = tuple(sorted(subset + (node, )))
 
                 if subset_without_i in self.recorded_values:
                     score_without_i = self.recorded_values[subset_without_i]
                 else:
                     print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_without_i}")
                     model_without_i = self.shapley_or_recon[subset_without_i]
-                    score_without_i = model_without_i.evaluate_model()[1]
+                    score_without_i = model_without_i.quick_evaluate()[1]
                     self.recorded_values[subset_without_i] = score_without_i
                     print(f"Coalition of {subset_without_i} scored {self.recorded_values[subset_without_i]}")
                     operation_counter += 1
 
                 if subset_with_i in self.recorded_values:
                     score_with_i = self.recorded_values[subset_with_i]
                 else:
                     print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
                     model_with_i = self.shapley_or_recon[subset_with_i]
-                    score_with_i = model_with_i.evaluate_model()[1]
+                    score_with_i = model_with_i.quick_evaluate()[1]
                     self.recorded_values[subset_with_i] = score_with_i
                     print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
                     operation_counter += 1
                 
                 summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
                 shapley_value += summand
```

### Comparing `asociita-0.1.9.1/asociita/components/nodes/federated_node.py` & `asociita-0.2/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.2/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,135 +1,137 @@
-# PARENT CLASS IMPORT
-from asociita.components.orchestrator.generic_orchestrator import Orchestrator # Parent class import
-# LIBRARY MODULES IMPORT
-from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
+import datasets
+import copy
+from asociita.components.orchestrator.generic_orchestrator import Orchestrator
 from asociita.utils.computations import Aggregators
-from asociita.utils.handlers import Handler
 from asociita.utils.loggers import Loggers
 from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
 from asociita.utils.optimizers import Optimizers
-from asociita.components.evaluator.evaluation_manager import Evaluation_Manager
 from asociita.components.archiver.archive_manager import Archive_Manager
-# ADDITIONAL IMPORTS
-import datasets, copy
 from multiprocessing import Pool, Manager
+from asociita.components.settings.settings import Settings
+from torch import nn
 
-
+# set_start_method set to 'spawn' to ensure compatibility across platforms.
 orchestrator_logger = Loggers.orchestrator_logger()
+from multiprocessing import set_start_method
+set_start_method("spawn", force=True)
 
 
-class Evaluator_Orchestrator(Orchestrator):
-    def __init__(self, settings: dict) -> None:
-        """Orchestrator is a central object necessary for performing the simulation.
+class Fedopt_Orchestrator(Orchestrator):
+    """Orchestrator is a central object necessary for performing the simulation.
         It connects the nodes, maintain the knowledge about their state and manages the
-        multithread pool. generic_orchestrator.orchestrator is a parent to all more
-        specific orchestrators. Evaluator_Orchestrator additionally performs a 
-        evaluation of the clients contribution, according to the passed settings.
-        
-        -------------
-        Args
-            settings (dict): dictionary object cotaining all the settings of the orchestrator.
-       -------------
-         Returns
-            None"""
+        multithread pool. Fedopt orchestrator is a child class of the Generic Orchestrator.
+        Unlike its parent, FedOpt Orchestrator performs a training using Federated Optimization
+        - pseudo-gradients from the models and momentum."""
+    
+
+    def __init__(self, 
+                 settings: Settings) -> None:
+        """Orchestrator is initialized by passing an instance
+        of the Settings object. Settings object contains all the relevant configurational
+        settings that an instance of the Orchestrator object may need to complete the simulation.
+        FedOpt orchestrator additionaly requires a configuration passed to the Optimizer upon
+        its initialization.
+        
+        Parameters
+        ----------
+        settings : Settings 
+            An instance of the Settings object cotaining all the settings of the orchestrator.
+            The FedOpt orchestrator additionaly requires the passed object to contain a 
+            configuration for the Optimizer.
+       
+       Returns
+       -------
+       None
+       """
         super().__init__(settings)
     
 
     def train_protocol(self,
                 nodes_data: list[datasets.arrow_dataset.Dataset, 
                 datasets.arrow_dataset.Dataset]) -> None:
         """"Performs a full federated training according to the initialized
         settings. The train_protocol of the fedopt.orchestrator.Fedopt_Orchestrator
         follows a popular FedAvg generalisation, FedOpt. Instead of weights from each
         clients, it aggregates gradients (understood as a difference between the weights
         of a model after all t epochs of the local training) and aggregates according to 
         provided rule.
         SOURCE: Adaptive Federated Optimization, S.J. Reddi et al.
 
-        -------------
-        Args:
-            nodes_data(list[..., ....]): list containing train set and test set
-                wrapped in a hugging facr arrow_dataset.Dataset containers.
-        -------------
-        Returns:
-            None"""
-        
-        # 1. SETTINGS -> CHANGE IF NEEDED
-        # GENERAL SETTINGS
-        iterations = self.settings['iterations'] # Number of iterations of the Fed training, int.
-        nodes_number = self.settings['number_of_nodes'] # Number of nodes prepared for sampling, int.
-        local_warm_start = self.settings["local_warm_start"] # Local warm start for pre-trained models - not implemented yet.
-        nodes = self.settings["nodes"] # List of nodes, list[int]
-        sample_size = self.settings["sample_size"] # Size of the sample, int.
-        # OPTIMIZER SETTINGS
-        optimizer_settings = self.settings["optimizer"] # Dict containing instructions for the optimizer, dict.
-        
-
-        # 2. SET-UP PHASE -> CHANGE IF NEEDED
-        # SETTING-UP EVALUATION MANAGER
-        evaluation_manager = Evaluation_Manager(settings = self.settings,
-                                                model = self.central_model,
-                                                nodes = nodes,
-                                                iterations = iterations)
-        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
-                                          logger = orchestrator_logger)
-        # CREATING FEDERATED NODES
-        nodes_green = create_nodes(nodes, self.node_settings)
-        # CREATING LOCAL MODELS (that will be loaded onto nodes)
+        Parameters
+        ----------
+        nodes_data: list[datasets.arrow_dataset.Dataset, datasets.arrow_dataset.Dataset]: 
+            A list containing train set and test set wrapped 
+            in a hugging face arrow_dataset.Dataset containers.
+        
+        Returns
+        -------
+        int
+            Returns 0 on the successful completion of the training.
+        """
+        # Initializing all the attributes using an instance of the Settings object.
+        iterations = self.settings.iterations
+        nodes_number = self.settings.number_of_nodes
+        local_warm_start = self.settings.local_warm_start
+        nodes = [node for node in range(nodes_number)]
+        sample_size = self.settings.sample_size
+        
+        # Initializing an instance of the Archiver class if enabled in the settings.
+        if self.settings.enable_archiver == True:
+            archive_manager = Archive_Manager(
+                archive_manager = self.settings.archiver_settings,
+                logger = orchestrator_logger)
+        
+        # Initializing an instance of the Optimizer class object.
+        optimizer_settings = self.settings.optimizer_settings
+        Optim = Optimizers(weights = self.central_model.get_weights(),
+                           settings=optimizer_settings)
+        
+        # Creating (empty) federated nodes.
+        nodes_green = create_nodes(nodes, self.settings.nodes_settings)
+        
+        # Creating a list of models for the nodes.
         model_list = self.model_initialization(nodes_number=nodes_number,
                                                model=self.central_net)
-        # INITIALIZING ALL THE NODES
+        
+        # Initializing nodes -> loading the data and models onto empty nodes.
         nodes_green = self.nodes_initialization(nodes_list=nodes_green,
                                                 model_list=model_list,
-                                                data_list=nodes_data,
-                                                nodes_number=nodes_number)
-        # SETTING UP THE OPTIMIZER
-        Optim = Optimizers(weights = self.central_model.get_weights(),
-                           settings=optimizer_settings)
-
+                                                data_list=nodes_data)
 
         # 3. TRAINING PHASE ----- FEDOPT
         with Manager() as manager:
+            queue = manager.Queue() # creates a shared queue
             # create the pool of workers
             with Pool(sample_size) as pool:
                 for iteration in range(iterations):
                     orchestrator_logger.info(f"Iteration {iteration}")
                     gradients = {}
-                    evaluation_manager.preserve_previous_model(previous_model = self.central_model) # Preserving last central model
-                    evaluation_manager.preserve_previous_optimizer(previous_optimizer = Optim) # Preserving last optimizer settings (together with momentum)
                     # Sampling nodes and asynchronously apply the function
-                    sampled_nodes, sampled_idx = sample_nodes(nodes_green, 
+                    sampled_nodes = sample_nodes(nodes_green, 
                                                  sample_size=sample_size,
                                                  orchestrator_logger=orchestrator_logger,
-                                                 return_aux=True) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+                                                 return_aux=False) # SAMPLING FUNCTION -> CHANGE IF NEEDED
                     results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
                     # consume the results
                     for result in results:
                         node_id, model_gradients = result.get()
                         gradients[node_id] = copy.deepcopy(model_gradients)
-                    
                     # Computing the average of gradients
                     grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
+                    # Upadting the weights using gradients and momentum
                     updated_weights = Optim.fed_optimize(weights=self.central_model.get_weights(),
                                                          delta=grad_avg)
-                    self.central_model.update_weights(updated_weights) # Updating the central model
-                    evaluation_manager.preserve_updated_model(updated_model = self.central_model)
-
-                    # TRACKING GRADIENTS FOR EVALUATION
-                    evaluation_manager.track_results(gradients = gradients,
-                                                     nodes_in_sample = sampled_nodes,
-                                                     iteration = iteration,
-                                                     optimizer = Optim) # TRACKING FUNCTION -> CHANGE IF NEEDED
-                    
-                    ### WEIGHTS UPDATE
+                    # Updating the orchestrator
+                    self.central_model.update_weights(updated_weights)
                     # Updating the nodes
                     for node in nodes_green:
-                        node.model.update_weights(updated_weights)
-                    # Upadting the orchestrator                 
-                    archive_manager.archive_training_results(iteration = iteration,
-                                                             central_model=self.central_model,
-                                                             nodes=nodes_green)
-        # 4. FINALIZING PHASE
-        # EVALUATING THE RESULTS
-        psi = evaluation_manager.finalize_tracking()
-        print(psi)
-        orchestrator_logger.critical("Training complete")
+                        node.model.update_weights(updated_weights)         
+                   
+                    # Passing results to the archiver -> only if so enabled in the settings.
+                    if self.settings.enable_archiver == True:
+                        archive_manager.archive_training_results(iteration = iteration,
+                                                                central_model=self.central_model,
+                                                                nodes=nodes_green)
+
+        orchestrator_logger.critical("Training complete")
+        return 0
```

### Comparing `asociita-0.1.9.1/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.2/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,83 @@
-import datasets, copy
-from typing import Any, Union
+import datasets 
+import copy
+from typing import Union
 from asociita.components.nodes.federated_node import FederatedNode
 from asociita.models.pytorch.federated_model import FederatedModel
 from asociita.utils.computations import Aggregators
-from asociita.utils.handlers import Handler
 from asociita.utils.loggers import Loggers
-from asociita.utils.orchestrations import prepare_nodes, create_nodes, check_health, sample_nodes, train_nodes
+from asociita.utils.orchestrations import create_nodes, check_health, sample_nodes, train_nodes
 from asociita.components.archiver.archive_manager import Archive_Manager
+from asociita.components.settings.settings import Settings
 from multiprocessing import Pool, Manager
 from torch import nn
 
-
+# set_start_method set to 'spawn' to ensure compatibility across platforms.
 orchestrator_logger = Loggers.orchestrator_logger()
 from multiprocessing import set_start_method
 set_start_method("spawn", force=True)
 
+
 class Orchestrator():
-    def __init__(self, 
-                 settings: dict) -> None:
-        """Orchestrator is a central object necessary for performing the simulation.
+    """Orchestrator is a central object necessary for performing the simulation.
         It connects the nodes, maintain the knowledge about their state and manages the
         multithread pool. generic_orchestrator.orchestrator is a parent to all more
-        specific orchestrators.
-        
-        -------------
-        Args
-            settings (dict): dictionary object cotaining all the settings of the orchestrator.
-       -------------
-         Returns
-            None"""
-        self.settings = settings["orchestrator"] # Settings attribute (dict)
-        self.node_settings = settings["nodes"]
+        specific orchestrators."""
+    
+    
+    def __init__(self, 
+                 settings: Settings,
+                 **kwargs) -> None:
+        """Orchestrator is initialized by passing an instance
+        of the Settings object. Settings object contains all the relevant configurational
+        settings that an instance of the Orchestrator object may need to complete the simulation.
+        
+        Parameters
+        ----------
+        settings : Settings
+            An instance of thesettings object cotaining all the settings 
+            of the orchestrator.
+        **kwargs : dict, optional
+            Extra arguments to enable selected features of the Orchestrator.
+            passing full_debug to **kwargs, allow to enter a full debug mode.
+       
+       Returns
+       -------
+       None
+        """
+        self.settings = settings
         self.model = None
-        if self.settings.get('training_metrics'):
-            self.training_metrics_filename = self.settings['training_metrics']
-        else:
-            self.training_metrics_filename = 'training_metrics.csv'
-        if self.settings.get('nodes_metrics'):
-            self.nodes_metrics_filename = self.settings['nodes_metrics']
-        else:
-            self.nodes_metrics_filename = 'nodes_metrics.csv'
+        # Special option to enter a full debug mode.
+        if kwargs:
+            if kwargs.get("full_debug"):
+                self.full_debug = True
+            else:
+                self.full_debug = False
+    
     
-
     def prepare_orchestrator(self, 
-                             model: Any,
+                             model: nn,
                              validation_data: datasets.arrow_dataset.Dataset,
                              ) -> None:
-        """Loads the global model and validation data that will be used by the Orchestrator.
+        """Loads the orchestrator's test data and creates an instance
+        of the Federated Model object that will be used throughout the training.
         
-        -------------
-        Args
-        validation_data (datasets.arrow_dataset.Dataset): 
+        Parameters
+        ----------
+        validation_data : datasets.arrow_dataset.Dataset:
             Validation dataset that will be used by the Orchestrator.
-        model (Any): Compiled or pre-compiled model that will 
-            be used by the instance of the class.
-        -------------
+        model : torch.nn
+            Model architecture that will be used throughout the training.
+        
         Returns
-            None"""
+        -------
+        None"""
         self.validation_data = [validation_data]
         self.central_net = model
-        self.central_model = FederatedModel(settings = self.node_settings["model_settings"],
+        self.central_model = FederatedModel(settings = self.settings.model_settings,
                                         net=model,
                                         local_dataset=self.validation_data,
                                         node_name='orchestrator')
     
 
     def model_initialization(self,
                              nodes_number: int,
@@ -71,137 +85,129 @@
                              local_warm_start: bool = False,
                              ) -> list[nn.Module]:
         """Creates a list of neural nets (not FederatedModels!) that will be
         passed onto the nodes and converted into FederatedModels. If local_warm_start
         is set to True, the method call should be passed a list of models which
         length is equall to the number of nodes.
         
-        -------------
-        Args:
-            nodes_number (int): number of nodes that will participate in the
-                training.
-            model (Union[nn.Module, list]): a neural net schematic (if warm
-                start is set to False) or a number of different neural net schematics
-                (if warm start is set to True) that will prepared for the nodes to be
-                loaded as FederatedModels.
-            local_warm_start (bool): A boolean value for switching on/off the warm start
-                utility.
-        -------------
-        Returns:
-            tuple(node_id: str, weights)
+        Parameters
+        ----------
+        nodes_number: int 
+            number of nodes that will participate in the training.
+        model: Union[nn.Module, list[nn.Module]] 
+            a neural net schematic (if warm start is set to False) or 
+            a number of different neural net schematics
+            (if warm start is set to True) that 
+            are prepared for the nodes to be loaded as FederatedModels.
+        local_warm_start: bool, default False
+            boolean value for switching on/off the warm start utility.
+        
+        Returns
+        -------
+        list[nn.Module]
+            returns a list containing an instances of torch.nn.Module class.
+        
+        Raises
+        ------
+        NotImplemenetedError
+            If local_warm_start is set to True.
         """
         if local_warm_start == True:
-            raise("Beginning the training with different local models not implemented yet.")
+            raise NotImplementedError("Local warm start is not implemented yet.")
         else:
             model_list = [copy.deepcopy(model) for _ in range(nodes_number)]
-
         return model_list
 
 
     def nodes_initialization(self,
                              nodes_list: list[FederatedNode],
                              model_list: list[nn.Module],
                              data_list: list[datasets.arrow_dataset.Dataset, 
-                                    datasets.arrow_dataset.Dataset],
-                             nodes_number: int) -> list[FederatedNode]:
+                                    datasets.arrow_dataset.Dataset]
+                                    ) -> list[FederatedNode]:
         """Prepare instances of a FederatedNode object for a participation in 
-        the Federated Training.  Contrary to the  create nodes function, 
+        the Federated Training.  Contrary to the 'create nodes' function, 
         it accepts only already initialized instances of the FederatedNode
         object.
         
-        -------------
-        Args:
-            nodess_list (list[FederatedNode]): list containing all the initialized
-                FederatedNode instances.
-            model_list (list[nn.Module]): list containing all the initialized 
-                nn.Module objects. Note that conversion from nn.Module into the
-                FederatedModel will occur at the local node level.
-            data_list (list[..., ....]): list containing train set and test set
+        Parameters
+        ----------
+            nodess_list: list[FederatedNode] 
+                The list containing all the initialized FederatedNode instances.
+            model_list: list[nn.Module] 
+                The list containing all the initialized nn.Module objects. 
+                Note that conversion from nn.Module into the FederatedModel will occur 
+                at the local node level.
+            data_list (list[..., ....]): 
+                The list containing train set and test set 
                 wrapped in a hugging facr arrow_dataset.Dataset containers.
-            nodes_number (int): Number of nodes that will participate in the training.
-        -------------
-        Returns:
+        
+        Raises
+        ------
             list[FederatedNode]"""
         
         results = []
         for node, model, dataset in zip(nodes_list, model_list, data_list):
             node.prepare_node(model, dataset)
             results.append(node)
         nodes_green = []
         for result in results:
             if check_health(result,
                             orchestrator_logger=orchestrator_logger):
                 nodes_green.append(result)
         return nodes_green # Returning initialized nodes
 
-        
-        # # create the manager
-        # with Manager() as manager:
-        #     # create the shared queue
-        #     queue = manager.Queue()
-        #     # create a pool of workers
-        #     with Pool(nodes_number) as pool:
-        #         # asynchronously apply the function
-        #         results = [
-        #             pool.apply_async(prepare_nodes, (node, model, dataset, queue))
-        #             for node, model, dataset in zip(nodes_list, model_list, data_list)
-        #         ]
-        #         # consume the results
-        #         # Define a list of healthy nodes
-        #         nodes_green = []
-        #         for result in results:
-        #             # query for results
-        #             _ = result.get()
-        #             updated_node = queue.get()
-        #             # Adds to list only if the node is healthy
-        #             if check_health(updated_node,
-        #                             orchestrator_logger=orchestrator_logger):
-        #                 nodes_green.append(updated_node)
-        # return nodes_green # Returning initialized nodes
 
     def train_protocol(self,
                 nodes_data: list[datasets.arrow_dataset.Dataset, 
                 datasets.arrow_dataset.Dataset]) -> None:
         """Performs a full federated training according to the initialized
         settings. The train_protocol of the generic_orchestrator.Orchestrator
         follows a classic FedAvg algorithm - it averages the local weights
         and aggregates them taking a weighted average.
-        SOURCE: Communication-Efficient Learning of Deep Networks from Decentralized Data, H.B. McMahan et al.
+        SOURCE: Communication-Efficient Learning of
+        Deep Networks from Decentralized Data, H.B. McMahan et al.
 
-        -------------
-        Args:
-            nodes_data(list[..., ....]): list containing train set and test set
-                wrapped in a hugging facr arrow_dataset.Dataset containers.
+        Parameters
+        ----------
+        nodes_data: list[datasets.arrow_dataset.Dataset, datasets.arrow_dataset.Dataset] 
+            A list containing train set and test set
+            wrapped in a hugging face arrow_dataset.Dataset containers.
         -------------
         Returns:
-            None"""
+        Int
+            Returns 0 on the successful completion of the training."""
         
-        # SETTINGS -> CHANGE IF NEEDED
-        iterations = self.settings['iterations']
-        nodes_number = self.settings['number_of_nodes']
-        local_warm_start = self.settings["local_warm_start"]
-        nodes = self.settings["nodes"]
-        sample_size = self.settings["sample_size"]
-        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
-                                          logger = orchestrator_logger)
-
-        # CREATING FEDERATED NODES
-        nodes_green = create_nodes(nodes, self.node_settings) # Exterior method / function, can override in childr.
+        # Initializing all the attributes using an instance of the Settings object.
+        iterations = self.settings.iterations
+        nodes_number = self.settings.number_of_nodes
+        local_warm_start = self.settings.local_warm_start
+        nodes = [node for node in range(nodes_number)]
+        sample_size = self.settings.sample_size
+        
+        # Initializing an instance of the Archiver class if enabled in the settings.
+        if self.settings.enable_archiver == True:
+            archive_manager = Archive_Manager(
+                archive_manager = self.settings.archiver_settings,
+                logger = orchestrator_logger)
+
+        # Creating (empty) federated nodes.
+        nodes_green = create_nodes(nodes, 
+                                   self.settings.nodes_settings)
 
 
-        # CREATING LOCAL MODELS (that will be loaded onto nodes)
+        # Creating a list of models for the nodes.
         model_list = self.model_initialization(nodes_number=nodes_number,
-                                               model=self.central_net) # Exterior method / function, can overide in childr.
+                                               model=self.central_net)
         
-        # INITIALIZING ALL THE NODES
-        nodes_green = self.nodes_initialization(nodes_list=nodes_green, # Exterion method / function, can overide in child.
+        # Initializing nodes -> loading the data and models onto empty nodes.
+        nodes_green = self.nodes_initialization(nodes_list=nodes_green,
                                                 model_list=model_list,
-                                                data_list=nodes_data,
-                                                nodes_number=nodes_number)
-            
+                                                data_list=nodes_data)
+        
         # TRAINING PHASE ----- FEDAVG
         with Manager() as manager:
             queue = manager.Queue() # creates a shared queue
             # create the pool of workers
             with Pool(sample_size) as pool: 
                 for iteration in range(iterations):
                     orchestrator_logger.info(f"Iteration {iteration}")
@@ -219,13 +225,17 @@
                     avg = Aggregators.compute_average(weights) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
                     # Updating the nodes
                     for node in nodes_green:
                         node.model.update_weights(avg)
                     # Upadting the orchestrator
                     self.central_model.update_weights(avg)
 
-                    archive_manager.archive_training_results(iteration = iteration,
-                                                             central_model=self.central_model,
-                                                             nodes=nodes_green)
+                    # Passing results to the archiver -> only if so enabled in the settings.
+                    if self.settings.enable_archiver == True:
+                        archive_manager.archive_training_results(iteration = iteration,
+                                                                central_model=self.central_model,
+                                                                nodes=nodes_green)
+
 
         orchestrator_logger.critical("Training complete")
+        return 0
```

### Comparing `asociita-0.1.9.1/asociita/datasets/fetch_data.py` & `asociita-0.2/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/datasets/load_cifar.py` & `asociita-0.2/asociita/datasets/load_cifar.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/datasets/load_fmnist.py` & `asociita-0.2/asociita/datasets/load_fmnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/datasets/load_mnist.py` & `asociita-0.2/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/datasets/save_blueprint.py` & `asociita-0.2/asociita/datasets/save_blueprint.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/datasets/shard_splits.py` & `asociita-0.2/asociita/datasets/shard_splits.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/datasets/shard_transformation.py` & `asociita-0.2/asociita/datasets/shard_transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from torchvision.transforms import Compose, GaussianBlur, RandomRotation, ToTensor, ToPILImage, RandomPerspective
 from asociita.utils.custom_transformations import AddGaussianNoise
 from datasets import arrow_dataset
 
 
 def blur_img(shard: arrow_dataset.Dataset,
              kernel_size: tuple[int, int]=(1, 3),
-             sigma: tuple[float, float]=(3., 40.)) -> arrow_dataset.Dataset:
+             sigma: tuple[float, float]=(5., 30.)) -> arrow_dataset.Dataset:
     """Blurs the given dataset.
         -------------
         Args
             kernel_size (tuple[int, int]) - size of the Gaussian kernel
             sigma (tuple[float, float]) - SD to be used to creating kernel to perform blurring, uniformly at [min, max]
        -------------
          Returns
```

### Comparing `asociita-0.1.9.1/asociita/models/pytorch/cifar10.py` & `asociita-0.2/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/models/pytorch/federated_model.py` & `asociita-0.2/asociita/models/pytorch/federated_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections import Counter
 from typing import Any, Generic, Mapping, TypeVar, Union
 #from sklearn.metrics import confusion_matrix, f1_score, precision_score, recall_score
 from torch import nn, optim
 from torchvision import transforms
 from sklearn.metrics import f1_score, recall_score, confusion_matrix, precision_score
 import os
+from asociita.exceptions.modelexception import ModelException
 
 from asociita.utils.loggers import Loggers
 
 model_logger = Loggers.model_logger()
 
 class FederatedModel:
     """This class is used to encapsulate the (PyTorch) federated model that
@@ -74,26 +75,26 @@
         params_to_update = []
         for _, param in self.net.named_parameters():
             if param.requires_grad is True:
                 params_to_update.append(param)
 
         # Choosing an optimizer based on settings
         if self.settings['optimizer'] == "Adam":
-            raise "Using Adam Optimizer has not been implemented yet."
+            raise NotImplementedError("Using Adam Optimizer has not been implemented yet.")
             # TODO #self.optimizer = torch.optim.Adam(...
         elif self.settings['optimizer'] == "SGD":
-            raise "Using SGD Optimizer has not been implemented yet."
+            raise NotImplementedError("Using SGD Optimizer has not been implemented yet.")
             #TODO # self.optimizer = torch.optim.SGD(...
         elif self.settings['optimizer'] == "RMS":
             self.optimizer = optim.RMSprop(
                 params_to_update,
                 lr=self.settings["learning_rate"],)
         else:
-            raise "The provided optimizer name may be incorrect or not implemeneted.\
-            Please provide list[train_set, test_set] or list[test_set]"
+            raise ModelException("The provided optimizer name may be incorrect or not implemeneted.\
+            Please provide list[train_set, test_set] or list[test_set]")
 
 
     def prepare_data(
         self,
         local_dataset: list[arrow_dataset.Dataset, arrow_dataset.Dataset] |
                                 list[arrow_dataset.Dataset],
         only_test: bool = False
@@ -375,13 +376,50 @@
                     precision,
                     recall,
                     accuracy_per_class,
                     true_positive_rate,
                     false_positive_rate
                 )
 
+    def quick_evaluate(self) -> tuple[float, float]:
+        """Quicker version of the evaluate_model(function) 
+        Validate the network on the local test set returning only the loss and accuracy.
+            Raises
+            ------
+                Exception: Raises an exception when Federated Learning is not initialized
+            Returns
+            -------
+                Tuple[float, float]: loss and accuracy on the test set.
+            """
+        with torch.no_grad():
+            if self.net:
+                self.net.eval()
+                criterion = nn.CrossEntropyLoss()
+                test_loss = 0
+                correct = 0
+                total = 0
+                losses = []
+                with torch.no_grad():
+                    for _, dic in enumerate(self.testloader):
+                        data = dic['image']
+                        target = dic['label']
+                        data, target = data.to(self.device), target.to(self.device)
+                        output = self.net(data)
+                        total += target.size(0)
+                        test_loss = criterion(output, target).item()
+                        losses.append(test_loss)
+                        pred = output.argmax(dim=1, keepdim=True)
+                        correct += pred.eq(target.view_as(pred)).sum().item()
+                    test_loss = np.mean(losses)
+                    accuracy = correct / total
+
+                    return (
+                        test_loss,
+                        accuracy
+                    )
+
 
     def transform_func(self,
                        data):
         convert_tensor = transforms.ToTensor()
         data['image'] = [convert_tensor(img) for img in data['image']]
         return data
```

### Comparing `asociita-0.1.9.1/asociita/utils/computations.py` & `asociita-0.2/asociita/utils/computations.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,22 +129,25 @@
         if return_dict == True:
             loo_set = {tuple(coalition) : None for coalition in loo_set}
             return loo_set
         else:
             return loo_set
 
 
-    def select_subsets(coalitions: dict,
+    def select_subsets(coalitions: dict | list,
                        searched_node: int) -> dict[tuple : Any]:
-        """Given a list of possible coalitions and a searched node, will return
+        """Given a dict or list of possible coalitions and a searched node, will return
         every possible coalition which DO NOT CONTAIN the searche node.
         -------------
         Args
             coalitions (dict): a superset or a set of all possible coalitions, mapping
                 each coalition to some value, e.g. {(1, 2, 3,): None}
             searched_node (int): an id of the searched node.
        -------------
          Returns
             dict[tuple : Any]"""
-        subsets = {nodes: model for nodes, model in coalitions.items() 
-                  if searched_node not in nodes}
+        if type(coalitions) == dict:
+            subsets = {nodes: model for nodes, model in coalitions.items() 
+                    if searched_node not in nodes}
+        if type(coalitions) == list:
+            subsets = [nodes for nodes in coalitions if searched_node not in nodes]
         return subsets
```

### Comparing `asociita-0.1.9.1/asociita/utils/custom_transformations.py` & `asociita-0.2/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/utils/handlers.py` & `asociita-0.2/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/utils/helpers.py` & `asociita-0.2/asociita/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/utils/loggers.py` & `asociita-0.2/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/utils/optimizers.py` & `asociita-0.2/asociita/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/utils/orchestrations.py` & `asociita-0.2/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/asociita/utils/showcase.py` & `asociita-0.2/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9.1/pyproject.toml` & `asociita-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.1.9.1"
+version = "0.2"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.1.9.1/PKG-INFO` & `asociita-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.9.1
+Version: 0.2
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

